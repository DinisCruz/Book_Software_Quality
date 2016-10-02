### Using Micro Services As Proxies

A part on that I had to recommend is the creation of a micro service for each client. And this micro service is basically a proxy, is basically a wrapper around the original service which usually tends to be massive, very complex massive legacy issues, massive versionning issues.

So, in a way instead of a particular client like a mobile or desktop or website via ajax consuming the main web service directly, what they do is they consume a micro service.

And this micro service needs to be maintained and created by both teams. So basically it is a project that has in a way two owners, one owner is the client like the mobile team, the other owner is the actual web service team the original one or the one that you proxy.

And what this means, it means that now when the mobile team needs a new API or a new entry point, or needs to get data differently, or needs to version it they are able to because they control that web service.

And the logic is that the core functionality, let's say for example all dedication decisions, all transition decisions, business logic, any kind of major should be on the main web service.

The power of this work flow is that because you then have the unit test that lock the micro web service, you could move that new functionality in a way the web service, the main one on time. And what that means it means that you allow the main web service to be conservative in the making changes and sustainability, robustness, consolidation re-factoring knowing that the clients are the micro web services so there is a very tight relationship there which can then obstruct those and secure them and performance, and queue them and perform all sorts of stuff before it reaches the client.

So, a common problem is for example an API wasn't designed for a mobile use which basically means that the API provides more data than it should, provides data in a non scale able way and this micro service will now allow you to fix that because you can normalize the APIs, you can basically create multiple versions, you can much better support multiple types of clients, for example multiple versions to mobile which each one has different versions.

It is easy to depreciate those in a way API versionning becomes a much better thing and what you have is then the ability to run them in the containers because they become really easy to containerize because suddenly they are now in this environment where they could be run in multiple instances.

You can have multiple versions even running in parallel and you can have multiple instances of that particular micro service running on top of the whole stack. So, that allows you to use containers like docker and you have a much more scale able and robust in a way secure solutions.
