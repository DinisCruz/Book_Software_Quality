**Network or browser based QA tests**

When talking about happy path tests to represent is do we do it for browser automation or network, key requirements is they have to be fast, they have to be easy to use, developers have to be able to run it, QA have to be able to run it, everybody needs to be able to run it.

Now, browser automation has the advantage that they represent more reality, they tend to have a problem because people tend to struggle with selenium, there is no very good APIs, and in a way phantom JS is probably very effective to do that for anything that requires dom manipulation and dom rendering.

I would also say that you also want to have a whole set of tests that run the network. They basically pure HTTP or whatever network protocol but for web it is ACP network requests. And they will represent all the functionality of the application.

And the logic is if the application talks to a server, there is going to be very key signatures and very key patterns that they use. So, eventually once you have a DSL for the application, now you know how to talk to the server. 

Then I actually found that network based tests are faster, they are more efficient, they do have a good level of obstruction because they allow existing code for the functionality and they force you to actually clean up a lot of your work flows.