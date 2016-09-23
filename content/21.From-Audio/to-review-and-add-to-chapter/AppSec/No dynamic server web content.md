**No server site dynamically generated web content.**

A very powerful design pattern that will proof as a huge amount of security for web applications is if there is no server site generation of dynamic web content.

Basically, what we shouldn't do is break code and data on the server site and then send it over an HTTP and then rebuild that on the client site and basically trying to transform again and split code and data.

What should happen is that all your web pages should be static, they should all download as static resources, they all should be locked down and all the data should be given to the UI in basically data objects like case and codes.

Or, downloaded as another static file which will be part of one of the resources that gets downloaded and is basically downloaded as adjacent object which is provided from the server site.

And what this allows is it allows for a very clean separation between code and data.