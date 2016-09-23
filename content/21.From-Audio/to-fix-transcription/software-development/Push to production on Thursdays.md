**Push to Production on Thursdays.**

One of the models I have seen that was very efficient for kind of delivery was this team that would meet with the stakeholders every Thursday to present the work that was ready to be released and had been done for the last week or even the last month. But basically whatever was ready at that time, that could have been pushed into production.

So what they would do is they would meet with the stakeholders, they would get to see if they were happy or not, whatever they agreed it was okay would go into service the following week. And they also asked them to plan for the features that they should be working next.

What is very good with this is that allows the customers to decide or the stakeholders to decide which are their top priority. Which is always very interesting because there were always things that they always thought that was very, very important, very, very key to do maximum urgency that when they had to pick five, somehow those things would always end up outside our top seventh or eighth or twelveth things to do next.

So there were always something more important to do in reality because there is always that kind of all these requests that actually aren't that urgent, aren't that important they just happen to have something.

But when you make them decide what to do, the business or the owners are much more focused and they pick that actually what really matters to them.

What is interesting about this system is that they also had kind of a hackathon, kind of peer review make sure that everything is fine, even from a security push on the following Monday and Tuesday, and then if everything was fine, the feature would go live on the Wednesday of that particular loop.

So, that means that the flow will be meet on Thursday, present, approve to go live, following Monday and Tuesday make sure everything is fine, final security push, every checks and then on Wednesday release it to production. 

And of course that will be kind of within the process of releasing first a couple of servers and then eventually pushing it out to all the live servers. And of course, if anything went bad in any of those releases, you would go back and roll it back. And then you solve it again. So by then you have a bunch of work so you meet again on Thursday and you can continue.

I found was this was a really interesting evolution from the big drop, the big kind of releases which also tend to be very painful in the past, but also tend to be a good compromise between products that cannot change that fast, products that do require hand on, products that have all sorts of interesting or complex requirements from liability, from maintenance, even from documentation, all sorts of things that needed to be taken into account.So, it a very good compromise.

So, the logic would be that this team can push to production in minutes, they can go all the way to production ultimated, but they choose to release in points in time which is basically quite important.

The other thing they had which was very interesting was also they had a bunch of simulants for quality issues and they did within that process, there were just bugs, there were maintenance, there were things that basically could be pushed into production very quickly. 

But they had no user impact, so the question so would be, if you have a particular set of tests that represent a user contract, if all of them were passive, you can make changes in a way without consulting any of the stakeholders because theoretically you shouldn't be changing the behavior.

And if something that is change in behavior, then what you need to do is the assumption is fix the tests to make sure then now you have that final smoke test.