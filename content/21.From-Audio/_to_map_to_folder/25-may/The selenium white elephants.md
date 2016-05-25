**The selenium white elephants**

Selenium tends to create massive white elephants. So, in companies I usually see, either companies who don't do any kind of browser automation tests, and browser tests, or companies who have done selenium or spent considerable amount of effort doing selenium. And they spend huge amount of money and effort building selenium IPIs which tend to become these big white elephants who require a huge amount of maintenance and usually take hours and hours and hours to run.

And they are very hard to maintain and usually tend to start to have this creep of failed tests who just become bigger and bigger and bigger.

For me the problem is that in those cases, there tends to be a separation between the developers or the QA who write selenium and the actual developers. It also sometimes happens that you don't have experienced developers or I would say hard core developers writing those selenium tests.

But even when you do, you tend to create this massive, complicated solutions that very few people can maintain. So, the problem is you have the QA guys writing tests but they aren't executed by developers. Which actually means that there is a big gap between the developer making a change and the test being executed.

Which also means that every time the developers make a code change, by definition they are breaking selenium test which is kind of a loop. So, you have the developer makes an extra change, commits the change, goes in there, breaks the test, the QA guy fix the test which is a very annoying and recurring and soul destroying exercise because he is forever fixing tests that he had improved before.

What we are missing here is the opportunity that if the developers runs the test themselves, first of all the developer has added value to do that because it will make the development faster. Which basically means that when the developer makes a code change, he checks if the test fails, his code change was successful, he fixes test, he confirms the fix that he did in a certain place, and then he is happy and he can commit.

And more importantly, what the developer just have done is that he fixed the test for the QA. So, the QA job now is just to double check the tests, so he reads the tests. And just to make sure that for example the tests is performing the way it is supposed to be performing, but he doesn't have to write the test.

So, that means that by the test arrives at QA, it is already passing. So, in a way, he never commits code change with broken tests. So, either the talent is the problem in the first place or the test represents now the fix. So that is a very more efficient work flow.

It also means that the developers went back to source code, they will do something very interesting which is they will start to gain the system. So, they will realize that for example you need IDs on statements, they will realize that they can code things differently to make the test easier and more resilient.

So all in all you have this very interesting reward system where the developer starts to realize that the way they code will make a difference in the effectiveness and the quality of the tests. Which even creates a very crazy thing which means that the tests are easy to do, the tests are more maintainable, positive look.

The other interesting factor is to consider how much time developers spend clicking on things. How much time developers actually make account change, have to go to a site do a service or something, invoke it, figure out what happened, come back to it, and do that.

So, think about it, the selenium test already knows how to get there, the browser automation test already knows how to get to a particular location. So, what it means, it means that if you allow the developers to run this, then they are becoming more productive. The quality and the resilience and the effectiveness of the code just goes way up and they code way faster. And what this also leads to is eventually the creation of DSLs which is the main specific languages for the tests.
