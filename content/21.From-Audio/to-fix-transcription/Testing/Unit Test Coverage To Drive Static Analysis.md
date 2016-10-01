**Units Code Coverage To Improve Static Analysis Coverage**

The fundamental problem with static analysis is understanding the code paths that in fact is one of the advantage of interactive analysis or even dynamic analysis because it actually runs with real code paths. 

But a good solution could be to use the results the paths created by code coverage. Because code coverage tells you what has been hit on an application. Now, in this case, you can't run the code coverage completely, you have to run the code coverage per method. 

So, in a way, it is a slice of code coverage per analysis. What that slice gives you is actually real code paths in the application, especially if you write tests the way I like to write which is the tests that have huge amount of code running at the same time. Which is where I don't mock methods or APIs I mock external dependencies.

So, you actually should see traces that flow from the beginning of the application for example an entry point all the way to an exit point of the application.

So what you then do is you could take this mapping, which is basically giving a road map giving in a way a map to the static analysis engine that say; hey data from here will be here, so then static analysis could follow the other code paths because now it can be way more clever of understanding actually where things fit to each other.

And I think with static analysis results that could be part of evidence that is shown why a particular vulnerability exists. So, you provide this evidence that says this is where I think the problem is here and that evidence is created by a mix of static analysis, unit test execution and other things.

The other thing you can do which is very interesting is you could also use this code path and this code coverage results to also expand on security unit tests. So, once we find sources that syncs, we should be able to create unit tests that evoke those. 

Once we find for example an authorization blind spot, we can have tests which basically be security focus tests that will prove that particular issues exists or will prove that particular issue doesn't exist which in essence is a regression test which is also very, very valuable.