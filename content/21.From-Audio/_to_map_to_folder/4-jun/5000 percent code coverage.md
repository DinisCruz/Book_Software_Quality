**5000 percent code coverage.**

A big blind spot in development occurs with the idea that even a hundred percent code coverage is too much. The key concept is that 100% or 99% code coverage isn't the summit, isn't where you want to go. That is base camp, that is the beginning of a journey that allows you to do all sorts of other tests and all sorts of other analysis.

So, the logic is that you use code coverage as an analysis tools, you use code coverage as a way to understand what a particular question is actually doing.
So what you have is a code coverage allows you to much better answer questions. So, for example, I want to make sure that I have 100% code coverage on all my exposed controllers for example.

So, I want to make sure that if I look at my browser automation, or my network automation tests, they are hitting 100% of my controllers. Now, it doesn't matter to me if that moment in time I actually have point eyes or later tests for those controllers that actually checks something, that actually invoke that code, that might not be good enough.

I want to know what happens in that particular scenario which in this case is web based requests to a particular controller. So, in a way you don't need 100% code coverage, you need a thousand, you need two thousand, five thousand. You need a huge amount of code coverage because ultimately, each method should be hit more than once, each method should be hit from all sorts of different cases.

In fact, your code coverage should ultimately match your use cases, should match every work flow that exists because that is actually another very interesting question. If I take all your accepted use cases, and I have the said tests for the current user contract, i.e. everything the user expects to do when interacting application, and I look at the coverage of the application.

If I want to get 70% let's say on a web tier, what is the rest? What is the other code that currently cannot be invoked using normal piece of interaction? And in most cases what you find is that code or vulnerabilities actually that exist there just waiting one day to be invoked.

Same thing the next year, I have an API layer, okay so you find and invoke every single method on that API. If I don't get 100% code coverage on all my code, what else is there? What kind of scenario currently exists in the code that I am not able to replicate in my tests?

Because that is the big question, the big question is, is there any part of the code that will be triggered by some event, some scenario? And you need to understand where those scenarios are, I need to test it because especially if you want to fix it, how can you fix a scenario that you don't even understand?

So, ultimately what you want isn't 100% that is actually very narrowing, what you want is a thousand, five thousand percent code coverage.