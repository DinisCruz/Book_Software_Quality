###  Service To Replay Requests From API

Once you have a suite of tests that invokes a service that tests what that service does, a spectacularly powerful technique is to record the answers, for example in JSON or XML, Text or Binary and then build a re-player that will replay those answers based on similar inputs or even important inputs.

So what you are creating is basically an offline proxy for the main web service. And what this allows in practice, it allows client websites for example angular react based websites to run completely offline. Allows mobile apps to run offline, allows all sorts of powerful work flows because suddenly in a way you have a mock of a dependency.

So what you have done was you mocked that dependency by replaying it and you don't need to have it for development. And the power is that you have all these tests that will run against the real app and the mock dependency that you then expect to also pass when run against the real dependency in a more end-to-end integration test or when there is more moving parts going on.

This is a very powerful technique and one that dramatically improves the productivity of development testing, everything versioning, certainly you can have new APIs, you can test what a new API would actually do, you actually can in a way developer can already simulate and code against the next version of an API even maybe before that request has been made to the back end.

Which it is now very powerful because it means that by the time you go and make the request to the back end, you could say look this is exactly what we need to do, here are the tests that shows you what we want to do, here is how we use it, now you add that to your API.

So, instead of having a particular brief that goes to the back end, they implement it then you start using it then you realize it isn't good enough, you go back to it then you re-factor it, so usually you might do two, three, four or five times across the life cycle. If you control that particular proxy, and the re-player, you will do that a hundred times because you get to experiment, you get to understand, you get to re-factor, and re-factor and re-factor until you get it right.

So, creation of that proxy that re-player should be a high priority task in developer teams. And as long as the teams will have not seen it working then don't ask for it. So this is one of those that you really want to spend the time to figure it out, and you know also it is going to dramatically improve the quality and the capabilities of the tests.
