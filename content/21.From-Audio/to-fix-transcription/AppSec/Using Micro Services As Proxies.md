### Using Micro Services as Proxies

Creating a micro service for each client is something I am happy to recommend. A micro service is basically a proxy, or a wrapper around the original service. The original service usually tends to be massive, with complex legacy and versioning issues.

So, instead of a particular client, such as a mobile, or desktop, or website, consuming the main web service directly via Ajax, the client consumes a micro service.

This micro service needs to be maintained and created by both teams. It is a project that in a way has two owners. One owner is the client (like the mobile team); the other owner is the actual web service team, which is the original one and therefore the one that you proxy.

This means that if the mobile team needs a new API, or a new entry point, or if it needs to get data differently, or needs to version it, they are able to because they now control that web service.

The logic is that the core functionality -- all the dedication decisions, all transition decisions, business logic, or any other kind of major decision-- should now be on the main web service.

The power of this workflow is that because you now have the unit test that locks the micro web service, you could move that new functionality to the micro service, and leave the main one online. This means that you allow the main web service to be conservative in making changes and sustainability. This supports robustness, consolidation, and re-factoring. Knowing that the clients are the micro web services, there is a very tight relationship between them which can secure, queue, and perform all sorts of tests before it reaches the client.

A common problem, for example, is an API that wasn't designed for mobile use. This means that the API provides more data than it should, and it provides data in a non-scalable way. The micro service will allow you to fix that because you can normalize the APIs, you can create multiple versions, and you can much better support multiple types of clients, such as multiple versions to mobile where each one has different versions.

With this workflow API versioning becomes much better. What you have then is the ability to run them in the containers. They become really easy to container-ize because they are now in this environment where they can be run in multiple instances.

You can even have multiple versions running in parallel, and you can have multiple instances of that particular micro service running on top of the whole stack. This allows you to use containers like Docker, and it gives you much more scalable, robust, and secure solutions.
