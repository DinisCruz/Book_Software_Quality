### Developing Eclipse IDE Plug-in Story

This story is relevant in the context of the chapter when you code in that real time code coverage environment and test execution you cannot go back. And when you code in the environment while you are used to tests running in milliseconds, it is really painful like literally your brain will hurt if you try to do something that takes seconds to run.

So here is a scenario, I was a couple of years back I needed to program, to create and Eclipse plug-in. But, the problem with eclipse plug-in is how you test it, so there is a lot of things that really you can only test when the whole eclipse is there because especially it was one where we were integrating with other eclipse plug-ins so there was definitely some interesting dynamics.

So, I really needed to have an environment where my tests were running actually in eclipse. So I found I believe was SWT port which was really great, which allowed me to do all sorts of testing with EIE in a way I had access to the eclipse objects when I was running that test.

The only problem is the test took at least three to five seconds to start because eclipse had to boot, and I really tried to clean up eclipse but I could never get it to be fast.

So, basically I started to think I need to hot-start eclipse before I run my tests, and the question is how do you actually get your stuff in there? So then I found this amazing API called JRebel, and what JRebel does is hot swapping of java classes in memory. And that solved a lot of problem because actually both [inaudible 00:01:55] and java have a big problem that when you are debugging, there is only limited amount of changes you can actually make on the code.

So JRebel doesn't have that problem so you can add methods, you can make significant changes, and what it does is it does hot swapping of classes which is spectacular and to be honest I don't know how most devs in java can code without JRebel.

So the power of it is that what I was able to do is I was able to load eclipse, so I was able to start eclipse from basically the main eclipse. So I would start an eclipse system, I would run the plug in which is what you do normally. So in this case I am not even running the tests. So what I am doing is I will just keep starting a version of eclipse from the development eclipse.

And then what I will do is I will open the tests in the child eclipse which is running now the plug-in which means that all the APIs are there, everything is in place, the plug-in is installed, everything is good. And then I will run my tests from the child eclipse version.

So these are already very powerful because it means I can run my tests and I know that eclipse APIs will be available, I know that the plug-in will be available, I know everything is there.

The real amazing thing is I could then make a change on the code, on the tests on the main code of the plug-in and because I had compilation triggered on the host eclipse, it would pick up those changes, it would basically compile them, JRebel will pick up that compilation and will inject that into the child eclipse.

So, you had this spectacular environment where I was basically programming eclipse in real time, and I was writing my tests and making changes to code, and when I saved it, the change will be automatically compiled by the host eclipse and will be injected in that particular version of eclipse.

And suddenly I was back into that real time code execution because again eclipse had a way to run in this case. Eclipse has a way to run the tests quite quickly, so I was able to have that environment where my tests would basically run in real time. I believe I was using infinity tests for some of these things also which also works quite well in eclipse.
