**Developers run QA Tests**

Developers need to run QA performance tests. When companies have performance tests, for example using JMeter or SOAP UI or other tools, a big blind spot that occurs is when the developers don't run those tools.

So, not only that is highly inefficient because we aren't reusing the ability to execute tests, it also puts the developer in a position where it is really hard to replicate the issue. So, if you look at the normal work flow, is QA writes a JMeter test, runs it, finds the problem, replicates the problem, he has a test now to replicate the problem, writes an email, sometimes have to write an essay to explain the problem, take some screen shots hopefully. 

Eventually that hits the developer, the developer now has to try to replicate the thing, he might write some other scripts, he might not be able to replicate or he might think well here is the problem, he runs the fix, he commits the fix, goes back to QA, runs the thing, hopefully he fixed the problem but if he didn't you start the loop up all over again.

Even more interesting, it means the developer doesn't have the ability to actually see what the QA guy is seeing. And also start to tweak and test all sorts of different variations of solving the problems.

Even worse, when the developer fixes a problem, he doesn't write a regression test which basically means now that the QA guy has the regression test which he has to maintain. So, you have this very highly inefficient loop where ideally what should happen is the developer runs the JMeter test, figures out the problem, do some tweaks, plays around with it, eventually finds the root cause of it, maybe writes a bunch of more tests, fixes all the tests including the JMeter that are now moved into a regression tests pile and commits.

So, now if anything the only thing the QA guy needs to review is whether the regression test makes sense. And in fact, he should be receiving approval requests to his tests with the fix that the developer just committed.

And this is exactly the same thing that happens when we have a security issue that we report and then the developer on the site can replicate it. And is the same thing that happens when you have selenium tests which also tends to become white elephants.