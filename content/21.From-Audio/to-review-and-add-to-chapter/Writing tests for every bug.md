**Writing tests for every bug**

Every bug that exists should have a test that passes when the bug can be correctly replicated. So, this sometimes can be a bit weird for TDD developers which seems counter intuitive to them because they are used to writing tests that only pass.

The idea here is because it is a bug, the tests should represent the bug, i.e. whatever it is happening in application that isn't desired and it is the same thing for security issues. So, you need to have a test that actually describes the existing problem.

So, let's say that it is a vulnerability in applications that happens once you log in, you can see somebody else's customer details and the test needs to be able to hit the application and log in as a user, get the user's details, log out, log in as another user, confirm they can get the second user log in details, and then ask for the first user data. If that is possible, the test should pass.

So, what this allows is not only provides a much better brief for the tester, and description of the problem, it also presents an opportunity to understand when the actual issue is being addressed.

And what this is, it means that once the issue has been addressed, you can then change that test so that test is now a regression test. So, the test that originally was created to represent the bug, which should exist in a separate bug tracking project, now is modified after the fix so that now it becomes a regression test. Meaning that if the vulnerability of a bug is introduced in the future, then you will be able to catch it because this test will fail.

And this is what the architects and the business planners should be reviewing, is they should be reviewing the test that describes the particular fix, in a way the regression test of that particular problem.

This is also very important because if it isn't possible to create this test in an easy way, that represents big gaps in the test environment, because you need a situation where as soon as a bug is identified, or a security vulnerability is identified, a test to be created even before you think about fixing it.

Another advantage of doing these tests is that it really allows for the problem to be well described. So, it is really the best brief ever for a developer that is going to fix the stuff or even from a business to understand the risk, when you can actually read the exploit or read the problem in the DSL domain specific language of the application that explains clearly what the problem is, how to replicate it, words that concern are needed to execute it and then people can make good decisions.