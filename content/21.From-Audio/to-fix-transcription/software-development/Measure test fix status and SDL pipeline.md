**Measure test fix status and SDL pipeline**

Your tests must follow the development life cycle. So, if you run a test about a particular issue which exists, let's say on a lab application, in the beginning you have a case that proves the problem that should be passing on three different levels.

It should be passing on development, it should be passing on QA, it should be passing on production, these are tests that represents the problem. You could also write if you want, a test that fails on development, QA and production which is a test that represents the fix. 

So, the logic will be when you fix the solution on development at that stage, the tests have swapped now. So what you have is a situation where the test from development is now passing on fix, failing on vulnerability, so passing for the regression test and then once it goes to QA, you do that one now reverse and eventually you have a situation where the tests that are in production tells you the fix has been deployed.

So, in a way you can go, you go from green, green, green, red, red, red, to eventually have red, red, red, green, green, green. Although of course usually by then you would remove the failed test, because you don't want failed tests in your build. 

But what is interesting about that is that you can actually see just by measuring test, am I measuring what test are you in, or what quantity of tests are passing in each of the areas, you can actually measure which state that a particular vulnerability is in your development pipeline.