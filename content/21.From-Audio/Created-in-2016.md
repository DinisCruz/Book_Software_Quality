## Created in 2016


### Versions in Sync

The hard challenges that exist when you have a website and a web service architecture or multiple web services depending on each other, you have to keep them all in sync. And web service depends on another web service, how do you make sure that a particular version, you don’t go into an incompatible is very important when, for example, your disaster recovery resilience strategy is to roll back into a previous version, which actually means that in reality there’s a limitation of how far you can roll back, unless you have all your versions in sync, because what happens is if you roll back into a particular version that is now incompatible with one of your dependencies, you have a problem. So this actually occurs normally in development where even sometimes when you push versions, they don’t happen at the same time and then you have these incompatibilities and crashes and problems. So one of the reasons why you need to have a very good disaster recovery and the ability to push code fixes to production is so that you have a very fluid understanding of where your blind spots are. One of the interesting things about security fixes versus normal bugs is that usually a new bug will be triggered by a recent code change, so it’s realistic to expect that a previous change that was done last day or week, it was actually responsible for the problem. Security problems, on the other hand, tend to exist there for a long time, which actually means that the option of rolling back is actually not possible, so the only solution is to actually do a fix, which actually means you actually need to fix codes and you might actually have to fix code in multiple APIs. So you need the ability to make code changes in every single thing that is a dependency from the application that’s being exploited.


### Power of Exploits

If you own a company that doesn’t have a strong application security team, or a company that has not seen powerful exploits of how they performed in their own environment, which basically means that one of what you need to do security jumping if you’re someone who wants to improve the security is to basically write to the exploits. And you underestimate the power of a good exploit. A good exploit will basically dramatically change people’s perception of what security actually means on the other company.

So it’s absolutely that you do that.

And they have to be professional, they have to look good, they have to look the part, they have to basically, ideally look from a kind of criminal business model point of view, where you actually show data being extracted, sold, being manipulated, remotely controlled systems are always very powerful.

Actually that’s what really will catch people’s imagination.

I think it’s important that you show those exploits from legal to business owners and to developers, because that breaks the whole kind of question of "why should we do security?"

Don’t underestimate the power of an exploit, and if you should find yourself having to justify security, then you’re really at the stage where you need some really good professional exploits that will allow people in the management area to ask the right question.

And that question is, "Can you fix it? Can you solve that security issue from hitting my company, because I don’t want 'that' (the demo you’ve done) to happen.”
