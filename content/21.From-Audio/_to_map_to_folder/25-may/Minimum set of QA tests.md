**Minimum set of QA tests**

Minimum set of tests for applications, for us to know is relevant a company there should be the minimum set of QA tests for the applications. They should either be browser automation or network based tests which have a DSL which invoke all the happy paths. i.e. this is everything that a normal user would be able to evoke.

And also this needs to include bugs because a bug is a happy path a user does X and something Y happens and basically what you do is you represent the functionality of that application.

What is key about these set of tests is not only they really show gaps in the current QA deployment test environment, they will represent the set of tests that confirm that a particular change can be pushed into production.

The logic is any code changes that happens, that doesn't touch those tests, first should be able to push to production kind of as quick as possible. And this also, some people call this smoke test for a very good visibility on what is going on with the application.

So, if the application is under load, the application has issues, then basically this will highlight those. The typical case of this test is this will be a test that invokes every single business functionality of the application, create something, edit something, delete something, modify something, view something, make it right etcetera  that is what these tests are.

And they are key for application security work flow because application security will use those tests and put the abuse cases on top of them.