**Passing Tests for Bugs.**

One topic that can break the head of somebody who has been doing tests even development for a while is the idea that when you have a test for a problem, a bug or even a security issue that test should fail.

My view is that the test should pass because a particular test represents a particular problem at the moment in time. So it represents a particular behavior at that moment in time. So that test should be a passing test, because even before you look at how to solve the issue, or what the issue actually is, you need to have a way to replicate the problem.

Because if you don't have an easy way to create a test that represents a problem or a security issue, what it means it means that the brief to the developer is much worse. Is much harder to actually understand what the real problem is, how to fix it if you don't negate a really good brief.

So the developer and the best brief to the developers are actually tests. So that is why even when we talk about security issues, you should also have a passing test. This now promotes the idea that everything that happens in application needs a test regardless if it will be fixed or not.

Which is really what we want, what we want is to have a very firm understanding of what is happening in the application so that we are able to then make good decisions whether what to fix, what not to fix and what is even implications of something.

And that is why the tests must be written to pass all the time even when they represent bugs or security vulnerabilities.