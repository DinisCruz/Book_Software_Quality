**Can't Write Tests Because We Are Re-factoring**

To make changes you need tests. One reason I hear teams say that they don't have tests at a particular moment in time is because their APIs are still in a state of flux, they are still figuring out, they are still re-factoring a lot. 

That is actually the wrong reasons not to have tests because to make changes and to make changes comfortably, you really want to have tests, tests is what allows you to make changes, tests is what allows you to run multiple versions in parallel, have the confidence that something will work with a particular version or not and in a way tests is what allows you to make changes.

So, by using the excuse or the reason that you are making a lot of changes that you don't need tests because you have to maintain the tests that just shows that your tests aren't good enough, your test environment isn't good enough which is why you don't want to maintain it.

And what you are doing is you aren't spending the time fixing that test environment, improving that test environment, making basically that test environment really robust.

And it is a false economy because the amount of time you are going to be chasing ghosts, the amount of time you are going to spend dealing with all the side effects of all the lack of testing will pay itself basically more if you actually improve the test environment and you have that ability to code in this very robust and confident way. And that is what tests gives you.

And another very powerful or dangerous excuse I have heard was when teams say, "oh we can't do this", and maybe they are already in say new developments. And they are already saying we cannot do this test or we cannot do this particular improvement because we have a deadline.

And these are teams that haven't even shipped, they don't have real products, they are just doing the code of proof of concept point of view but they are already doing short cuts. They already don't have an environment where they can run tests very cleanly, very efficiently, and basically they are already coding in the same way that created the platform that they are trying to replace.