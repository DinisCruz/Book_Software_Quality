### Using Tests To Communicate

Teams should be talking to each other using tests because the reality is the way teams communicate, when they do it is usually teams have real issues communicating in among each other. You find that it is very inefficient it is an email here, it is a half baked bug tracking bug issue opened, some paragraphs, a screen shot, if you are lucky a movie.

So that is a horrible way to communicate, a bug, an issue, a feature...something. It isn't repeatable, you don't really have the context, you can't scale, you can't expand on that you can't run it automatically all the time to know if it is still there or not, and it basically is highly inefficient.

For me the way to do it is teams should be communicating using tests and this is a team member to team member but also up and down, manager to teams, testers to teams, across teams or in this case and even business mistake in programs or you have some [inaudible 00:01:17] programs to the teams.

So this way a test becomes the linko franca of companies, it becomes the method that they communicate. And this has tremendous advantages because for it to work, you need to have very good test APIs, you need to have very good execution environments. So you have to have easy to develop, easy to install and access development environment which very rarely occurs.

So, by doing that, by making tests the way teams communicate, you are creating this environment that rewards good APIs, rewards good solutions for how to test the application. And also, it has the advantage that you can measure because you can measure how many tests have been written across teams, you can see it, you can basically view the quality of it, and you see them across teams etcetera.

So, it is a major advantage. And finally, it is also a spectacular way to review changes. So, if you send a test that says, "hey I would like this", or "here is a problem" or basically "I would like XYZ to occur" then the best way to review that when it has been done is by reviewing that test. i.e. reviewing the test that had to be modified now that the thing is working.

So what happens is you have a passing test with the current behavior that maybe you want to change and then in that we are having a passing test that represents the fixed state. And by reviewing the delta, seeing the div between these two versions is sometimes the best way to evaluate if the bug or the fix that was requested or the feature that was requested is actually now working.
