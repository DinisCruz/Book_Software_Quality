###  Service To Replay Requests From API

Once you have a suite of tests that invoke a service, or test what that service does, a spectacularly powerful technique is to record the answers, for example in JSON or XML, Text or Binary, and then build a re-player that will replay those answers based on similar inputs.

By doing this you create an offline proxy for the main web service. In practice, this allows client websites, for example Angular or React based websites to run completely offline. It allows mobile apps to run offline, and it allows all sorts of powerful workflows because suddenly you have a mock of a dependency.

You have mocked that dependency by replaying it, but you don't need to have it for development. The power of this technique is that you have all these tests that will run against the real app and the mock dependency. Having done this, you can then expect them to pass when run against the real dependency in a more end-to-end integration test, or when there are more moving parts going on.

This technique dramatically improves the productivity of development testing and versioning. If you have new APIs, you can test what a new API would actually do. You can even develop, or simulate and code against the next version of an API, maybe even before that request has been made to the back end.

This means that by the time you go and make the request to the back end, you can say "Look, this is exactly what we need to do, here are the tests that show you what we want to do, here is how we use it, and now you can add that to your API".

So, instead of having a particular brief that goes to the back end, they can implement your tests, and if you then start using them and realize they aren't good enough, you can go back and re-factor them. Usually you might do this up to five times across the life cycle. In situations where you control a particular proxy, and the re-player, you will re-factor a hundred times because you get to experiment, understand, and then re-factor continuously until you get it right.

The creation of that proxy, or re-player, should be a high priority task in developer teams. However, teams that have not seen it working won't know to ask for it. So this is one of those techniques that you really want to spend the time figuring out, because you know it will dramatically improve the quality and the capabilities of the tests you run.
