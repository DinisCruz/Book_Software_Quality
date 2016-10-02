### No server-site generation of dynamic web content

A very powerful design pattern that can provide a huge amount of security for web applications, is when there is no server-site generation of dynamic web content.

This avoids the pattern of:
 - starting with clean data objects on the server
 - merging code and data on the server
 - sending it over to the client as HTML
 - rebuilding it on the browser site for rendering and execution

The way to make this happen is to make all your web pages and content to be downloaded as static resources. This is done from a locked down server, ideally using git as the deploy mechanism. Data is provided to the UI via AJAX requests from dedicated WebServices.

This provides a very clean separation of the multiple applications's components responsibilities, while solving the good-old problem of mixing code with data, which is the root cause of injection vulnerabilities.

This technique also has dramatic effects on testing and the developer's productivity.

Some modern frameworks (like AngularJS and ReactJS) promote this workflow, with a very clean separation (and hosting) of the UI code, and the data it consumers.

What makes this so problematic in HTML is the sheer number of places Javascript can be executed and the need by the browser to parse the content received in order to understand which parts are code, and which ones are data.

A typical blind spot is the insertion of JSON encoded values inside a Javascript block. The problem is that JSON encoding only handles double-quotes, which means that payloads like ```</script><svg/onload='{javascript}'/>``` will become active once rendered
