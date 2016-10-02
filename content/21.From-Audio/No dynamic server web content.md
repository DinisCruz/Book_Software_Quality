**No server site generation of dynamic web content.**

A very powerful design pattern can provide a huge amount of security for web applications if there is no server site generation of dynamic web content.

What we must avoid is breaking the code and data on the server site, sending it over an HTTP, and then rebuilding it on the client site; basically trying to reform the split code and data.

What should happen is that all your web pages should be static. They should all download as static resources, and they should all be locked down. All the data should be given to the UI in data objects like case and codes.

Alternatively, they could download as another static file which will be part of one of the resources downloaded as an adjacent object. The adjacent object is provided from the server site.

This allows for a very clean separation between code and data.
