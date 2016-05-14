### Versions in Sync

_(fixed and ready to move to main content)_

The difficult challenge that arises when you have a website and a web service architecture or multiple web services that depend on each other, is that you have to keep them all in sync. And when one web service depends on another web service, how do you make sure that you don’t go into incompatible versions?

This is very important when, for example, your disaster recovery resilience strategy is to roll back into a previous version.

This actually means that there’s a limitation of how far you can roll back, unless you have all your versions in sync, because what happens is if you roll back into a particular version that is now incompatible with one of your dependencies, you have a problem.

This normally occurs in development where sometimes even when you push versions, they don’t happen at the same time and then you have these incompatibilities and crashes and problems.

One of the reasons why you need to have a very good disaster recovery and the ability to push code fixes to production is so that you have a very fluid understanding of where your blind spots are.

One of the interesting things about security fixes versus normal bugs is that usually a new bug will be triggered by a recent code change, so it’s realistic to expect that a previous change that was done in the last day or week was actually responsible for the problem.

Security problems, on the other hand, tend to exist for a long time, which means that the option of rolling back is not possible. So the only solution is to actually do a fix, which means you need to fix codes, and you might have to fix code in multiple APIs. So you need the ability to make code changes in every single thing that is a dependency from the application that’s being exploited.
