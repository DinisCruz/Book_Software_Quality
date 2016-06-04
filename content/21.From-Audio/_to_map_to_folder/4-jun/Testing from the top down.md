**Security review from the top down and from the bottom up.**

A bug that exists, especially a bug that is fork able from the website. It is a great asset to try your current test environment in action. So what happens is when you get a bug treated from the website, you need to write tests from the top all the way to the bottom of your code stack.

So, you start to write the first test from the browser automation, so you replicate what happens then you write another test at network level and then you write another test, ideally that understands the code between the next level of inter phases.

So, you write a test that is able to run without actually in a way with marked or replaying the dependencies. And you do that for every layer, so if you write a test at a website layer then a web service layer then there is a business logic layer and then you write a database layer. And what you are trying to figure out is exactly where the vulnerability exists.

So, you go all the way down, and usually by the time you finish, you now have a great understanding of the root cause of the problem. So, the logic is that your fix will basically let some tests pass and break some. So, every test under the place of the fix will still pass, every test above the fix will now fail and what you do is you then change those tests that fail to now pass on the existing other fix but not the regression tests.

What is also interesting is when you go the bottom up. So when you find applicable place where you are vulnerable, the question is, who else is vulnerable? Who else also uses this?

So, the question here is you start to go up, so you go to the colors and you write tests that represent that. And this again is where code coverage becomes interesting because code coverage allows you to understand this because you can look at the code coverage and say, "hey I know that asset is used here, so I am not reaching here. So, it means my tests aren't good enough".

So these ways you are writing the test at the bottom up and the logic is as you write those tests, you eventually, if you reach a place where the attacker has direct control, you just found an exploitable vulnerability.

If the attacked to date doesn't have control over it, you might have a situation where you have a vulnerability in waiting i.e. you are one little degree of separation away from that vulnerability becoming weaponized. 

Which is kind of why this technique is so powerful, so in a way every bug that you have is an opportunity to really do a top down and a down up analysis of the issue and then really understand the root cause and really understand every place that that issue actually exists.