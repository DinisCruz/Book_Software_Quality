### Debugging Using Code Coverage

When you have real time code coverage, one of the things that happens and it will happen even if the developer doesn't do it on purpose, is that he will start to debug using the code coverage. Because what will happen is you will start to see where your test fails. Just to be clear, this is the case where you see the code coverage and you see in different colors, the lines that were affected by the code coverage.

So, it isn't just pure vanilla code coverage, it is also you get to see usually in red the lines that actually contain the path that failed the test.

So what happens is when you have that, and you see exactly what is flying through the application, you don't need to debug anymore, i.e. flick the debugger, run the thing, press F7, F7, F7, and then wait and then see this bla, bla, bla. And then even though the problem with that system is that it is not repeatable. So, every time you debug you are going to have to do exactly the same thing, exact same break point, break points will change.

So, after a while you lose focus, you lose knowledge, you lose all sorts of things. With the test you don't have that, when you are writing a test you could basically evolve your test in a way that makes sense for almost sometimes debugging the issue that you are working on.

And what that means it means that you have a way better technique for finding what is going on with that particular app, with that particular version and that is what I mean by you debug using code coverage.

Another very powerful technique is when you just run one test, and you see what happens. So this will give you sometimes a much better understanding of what you are touching on the application. And especially when you talk about understanding the attack surface, understanding this particular pathode. It is really powerful to see only this particular slice of the application.

Which is also why you want to run the most App as possible because or else you know you are just going from a bit of code to a mock which isn't really what you want, you want to go much deeper into the application because that is where the issue tends to be.

So another very powerful technique is to run only the code coverage or only the method for example expose let's say the attack surface so now you see how deep the input reach to the application, you start to see that there is a gap, you look at your code and you go; "hold on I have a controller here, I have some code that takes data from the user but I am not testing it, or I am not reaching that".

And so that again itself is a massive powerful technique.
