**When The Tests Fail.**

If your tests are fragile, you need to spend more time re-factoring them and building the test infrastructure. Something key that your tests are super solid, your tests need to be rock solid, in fact every time a test fails you should be happy because it represents a change that you made on the application.

So what I found is that there has to be a direct correlation between the failing of the test and the change that you made. So, in a way the test failing it shouldn't be a fail, it should be seen as a confirmation of what you just changed.

And by changing the test you confirm that your expectations of your change match what happens. So I find situations where sometimes you make a change, and the tests that fail aren't the ones you were expecting. Now that sometimes can point to a gap of your understanding of the application but sometimes it might actually indicate that you changed the wrong thing. And that is actually very valuable. 

So, it is very valuable to have a very direct feedback between the changes that were done and the tests that broke including the code coverage. Code coverage is a massive part of this work flow because that also tells you the implications and the side effects of your code changes.

So, if you find yourself fixing a lot of tests that means your tests need to be re-factored. Your tests need to be basically seen as high quality code which you need to maintain and build focus of course. This means that you also need to have sometimes tests for your tests because you will build sometimes a test API which needs to be tested in itself. And that keeps the whole system very clean.

One element that I found makes some actual difference is when the developer or the person who is fixing the code or is looking at the code is able to run all the tests that are relevant to that part. So if they are QA tests that person is to run those QA tests because they should be fixing it.

One area that you tend to have a lot of fragile tests is when some developer makes a code change and he breaks tests but the developer doesn't fix those tests which basically means that in the QA your performance team is always fixing tests. Which basically means that they are always in this loop of actually fixing something that was broken in a way by design with the latest checks.

What you want is a situation where when the developers do fix you actually have a test that represents that fix. So, just by looking at the changes, you can see what actually happened and in fact if you need to do more testing or not, and it also goes the other way. The QA guy should also be writing tests and fixing tests for devs because that promotes collaboration and improves the whole system.
