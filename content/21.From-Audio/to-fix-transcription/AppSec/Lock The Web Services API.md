### Lock The Web Services API

The key problem web services consumers have is how to make sure that;

a] they fully understand what the web services API does and behave.

b] what happens when there are changes.

So this could be a website, could be a follow one web service, could be a mobile application, could be a desktop application, basically anything that consumes a web service or an API.

So the solution for that is to create a series of tests you could call mini tests, you could call integration tests, which evoke all the functionality, in fact the exact functionality that that particular client uses from that web service.

And what this does is this will lock in a way in those tests the current functionality that is being used by the application. Which has tremendous advantages. First of all, when there is changes that team will get advanced warning, because those tests start to fail but also it is very useful for the API designers, the people who actually developed and maintain that particular web service of API to know how it is being used.

So, this is a very powerful technique and one that I highly recommend which leads to something very powerful which is having a micro service that is dedicated to a particular client.

And what this allows, this allows a much better scale and security hardening of those particular clients because you can remove data, you can clean data, you can in a way customise a little bit that API for that particular client.

And this is something that is possible to do once you have a suite of tests, because a suite of tests becomes the contract between the client and the server, and the web service.
