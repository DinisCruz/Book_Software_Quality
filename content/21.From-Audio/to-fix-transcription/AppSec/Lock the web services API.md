### Lock the Web Services API

Two key problems web services consumers have is how to make sure that they fully understand:

  a] what the web services API does and how it behaves.

  b] what happens when there are changes.

The service in question could be a website, a follow-on web service, a mobile application, a desktop application; it could be anything that consumes a web service or an API.

The solution to these problems is to create a series of mini-tests or integration tests, which evoke the exact functionality of the web service the client uses.

This will lock in those tests that examine the current functionality being used by the application. The advantages of locking in the tests are twofold. First of all, the team will get advance warning when there are any changes, because those tests will start to fail. Secondly, it is also very useful for the API designers, who develop and then maintain a particular web service API, because the tests show the API designers how the service is being used.

This is a very powerful technique and one that I highly recommend. It leads to something very powerful: a micro-service that is dedicated to a particular client.

This allows a much better scale and security hardening of those particular clients because you can remove or clean data, and you can, to a degree, customize that API for that particular client.

This is possible to do once you have a suite of tests, because a suite of tests becomes the contract between the client and the server, and the web service.
