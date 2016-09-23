**Broken Tests Aren't The Problem**

It is quite worrying how many times you hear complains about test's execution (for example their speed or how hard they are to maintain)

These complains can be so strong, that they can even question if the tests are 'worth it'? (i.e. the negative sides of maintaining the tests are higher than its benefits)

This is very dangerous because it is promoting the idea that it is OK not to test your code. And that is just crazy!

Every code change has to be reflected in a test because it is key to understand their impact (see [Making Random Changes](2.Making-Random-Changes.md)).

If the solution to broken tests is to stop having those tests (or removing them), then that is literally throwing the baby with the bath water. That is basically saying, _"I have a problem here, and instead of addressing the root cause of the problem, I am going to get rid of the whole thing"_.

To tackle this issue, what we need are better ways to measure the effectiveness of tests (and spot problems before they become an issue). We need to understand when those tests are working, we need better metrics to known when they are effective, and make sure that we aren't basically solving the wrong problem.

A really good way to measure the effectiveness of the current test workflow, is to measure how empowering those tests are for developers (and for everybody involved in the development lifecycle).

Measure: 'Who writes the test?', 'Who runs the tests?', 'Who is able to quickly write tests for new issues?', 'Are tests used to communicate between teams?', 'How fast do those test execute?' ... and you will see how efficient the whole thing is.

This is connected to the idea that managers should also be writing code. Managers should be reviewing and writing tests, because that is something that they can do because they have technical ability.


_The more understanding there is of the impact of changes, the easier it is to refactor the code. With easy and productive refactoring, it is possible to 'lock down' the application and remove all sorts of un-intended behaviour/capabilities (which will make it a much more secure application)_
