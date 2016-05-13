## From Audio - Rewrite and map to chapters

### Bono’s Comments on the Music Industry

I think it was in Time Magazine or a New York Times article, Bono wrote about his wish list or predictions for 2010 in which he makes a claim that the lack of copyright protection mainly damages the little guys, where the big guys like him actually get protected. And I don’t really buy that argument, because I think the little guys have always been screwed by the music industry, which basically tries to exploit them as much as they can until they get big enough that they can actually get contracts, like Bono has. And in fact the music industry used to be so bad that I found out in the 80s, some of the contracts were considered to be unenforceable. When the judge actually looked at that things, he said “there’s no way you guys can do this.” So I don’t think the music industry has any credibility in claim to say that the privacy and the lack of copyright protection on music actually damages the little guys, and basically I think that’s still yet… to be proven a fact. It’ll be interesting to see them improve on that. I actually think the little guys can now be much more proactive and dynamic about the stuff they do. I actually remember reading an article ages ago, I think it was in the early 2000s, about how the real way to sell music online is if it's the easiest way to sell and buy music for the little one, and in some ways, that’s what iTunes did. iTunes basically realized that the price was reasonably decent and basically brought music, the little music, to the masses. What I still think the music industry has failed to capitalize on is the fact that as musicians or the music products they sell, they only sell one or two items I will buy a year, while in reality, for bands I like, I’ll spend a lot more money with them but they still are not able to sell those things to me. They are only able to sell me an album, which I’ll buy because I like the bands, and I like the previous ones. But they need to be much more sharp and sell me a lot more stuff, which in some ways is what the Guitar Hero guys did, because they were able to leverage a lot more revenue streams from those music.

### Versions in Sync

The difficult challenge that arises when you have a website and a web service architecture or multiple web services that depend on each other, is that you have to keep them all in sync. And when one web service depends on another web service, how do you make sure that you don’t go into incompatible versions? This is very important when, for example, your disaster recovery resilience strategy is to roll back into a previous version. This actually means that there’s a limitation of how far you can roll back, unless you have all your versions in sync, because what happens is if you roll back into a particular version that is now incompatible with one of your dependencies, you have a problem. This normally occurs in development where sometimes even when you push versions, they don’t happen at the same time and then you have these incompatibilities and crashes and problems. So one of the reasons why you need to have a very good disaster recovery and the ability to push code fixes to production is so that you have a very fluid understanding of where your blind spots are. One of the interesting things about security fixes versus normal bugs is that usually a new bug will be triggered by a recent code change, so it’s realistic to expect that a previous change that was done in the last day or week was actually responsible for the problem. Security problems, on the other hand, tend to exist for a long time, which means that the option of rolling back is not possible. So the only solution is to actually do a fix, which means you need to fix codes, and you might have to fix code in multiple APIs. So you need the ability to make code changes in every single thing that is a dependency from the application that’s being exploited.

### Application Security Testing (written in 2010)

There’s a lot of talk about if application security testing is a static analysis or dynamic analysis and how all that stuff works, and the reality is that in order to know that there’s a proper application on a website or system, you need both. You need static analysis to tell you how the app works and then you need dynamic analysis to figure out how it actually works and also to test and make sure the issues are exploitable and you actually have a problem with it. So what you really need is a way to leverage the best of both worlds -- either have tools that provide both environments or be able to consume each tool that provides every piece of the equation, because it’s a very complicated world and there’s completely different skills required around doing that. So what I really want is to be able to merge those two worlds and to treat them as one and really perform security analysis using those technologies.

- the key here is to mention the need to have multiple tools running on the code
- mention IAST and RAST
- mention DHS project that runs multiple scanners on same codebase and consolidates reports
- mention ThreadFix (https://github.com/denimgroup/threadfix) and its capabilities to load multiple tools results and consolidate findings

### Cloud Security Part 1 (2010)

So one interesting thing about cloud security compared to the previous generations of security efforts, let’s say in compared to software security and website security, is that for both the software and website, security was almost a business disabler, which basically means the more features, the more security people added, the less attractive the product would be. And there are very few applications and websites that can actually make the client need more security in order to do more business, which results in the best return on investment. And what’s interesting about cloud security is that it might be one of the times where security is actually a business requirement, because a lack of security would slow down the adoption rate and prevent people from moving into the cloud, which basically means that people will care about it and invest in it. I was thinking about that and I realized that the problem with cloud security, or let’s say security vulnerabilities in the cloud, is that the compromise doesn’t just affect one company -- it affects all companies that are hosted there. This means that it’s a much, much bigger problem and, you know, where vulnerability or security incidents traditionally result in one company being affected and the people in that company all trying to solve the problem until it’s resolved, here, the companies affected or the assets affected are not under the control of their owners. And the people hosting them now have to manage all these external people who don’t have any control over their data and who can’t work because their service is down or it’s compromised, etc. That means that you have a much more horizontal kind of problem because you have not just, from Company A, let’s say, afac factor or Company A-driven attack affecting Company B, C, D, E, F, all the way to X, Y, Z. So it’s a much tougher problem to deal with. And the point here is that while catastrophic failures are acceptable or are tolerated, should I say, in normal websites and applications, cloud-based worlds are much less tolerant, because literally a catastrophic failure, one where everything fails or the whole data is compromised or removed, is potentially the loss of that business. And that hasn’t happened, but surely it will happen. And in some ways, companies will then have to show that they care more about security than the people who own that data.

### Cloud Security Part 2 (2010)

One of the concepts that Bruce Schneier talked about on this conference on the OWASP IBWAS conference in Spain is that a cloud or a service actually cares more about the security of their customers than the customer itself.

They should care more about security than the customers, because their loss there is potentially massive

That is a very good concept.

And I think in future it’s all going to be about companies being able to show that they do care more about their customers’ data and the customer information and the customer itself and basically being able to say “Look, I have better systems than you have in place, so you better trust me with your data because I’ll be able to manage more data for you than you are able to.” And what that really means is that it will be akin to regulatory compliance that some of this stuff is actually handled on the outside world because they’re able to control it better. So in some ways, you can see a credit card company doing that. But you can also see doing it in the medical industry or any kind of industry involving personal or relevant information; you can see it moving into that world where they say “Look, you can’t handle that, or if you handle it you have to have this type of insurance.” So you basically need to have this type of service, which you don’t have, so you better outsource that, but to do that we actually need a lot more visibility. We’ll need a lot more maturity in our industry, because companies actually need to be able to show that they have that kind of control. It’s not just that they are compliant by somebody who just basically go for the lowest beater and then pays and tells them they’re compliant. And I reckon that the only way we’re going to achieve that is by genuinely enhanced visibility into what’s going on so that people can actually measure what’s happening and then make the big, real decisions based on it. And in some ways, the proof of the pudding is going to be not how many vulnerabilities they have, but how they recover from incidents. Because in some ways, that’s the best good measure. The better a company is able to sustain attack is actually the better the company protects data, right? A company who says “I received x, y, z number of attacks and I was able to sustain them and protect them this way” is essentially a company that is more trustworthy than the company that is completely opaque. And I think that’s in some ways the key to making this work is to create either technology or standards of process that actually increase the visibility into what is going on.



### Technical Managers With Coding Skills

If you have technical managers with coding skills, it’s a waste of their talent if they’re not coding once they get promoted into a non-coding function like technical architect or business analyst or even manager.

One of the things they should be doing is actually reviewing the tests that are written by the application that they are managing, and the fact that they have technical skills and coding skills means they can do it, which is an asset that should be leveraged.

What they should be doing is that for every feature that they request or find a bug, they should be reviewing the tests that represent the fix for that particular feature. And if that’s not possible, that represents a gap in the current test environment, which needs to be addressed. So ideally what should happen is the test should be written in a DSL, which is domain specific language, which should be easy to read and should clearly describe the bug or feature that has been fixed.



### Hiring Games Developers

There’s a lot that the appsec industry can learn from gaming, because they really spend a lot of time thinking about visualization, how to understand highly complex sets of data, things about the maps they create, and the kinds of ways they map the games so that it's easy for the user to understand and play. I think there’s a lot of stuff we can learn from it.

They also have a lot of interesting attacks through the extra games business logic, which is something that we could learn from, too. And more importantly, they also have a lot of great hardware that is designed for high levels of processing and graphical visualization stuff. So there’s a lot of interesting application security analysis that can be done using the gaming industry's hardware, software visualization, and concepts.

So I wonder how many of the companies actually hire games developers because as I have said, they are big assets to have and can add quite a lot of value.



### Hosted services source code

*Need for companies that provide hosted web services to also provide the source code for their apps.*

So this is the need for companies that provide hosted solutions of applications need to provide their source code of their applications, and they need to do it for three reasons.

One of them is to allow the offload hosting of their data and the easy backup and the restore of their data.

The second one is to allow the emergence of third party companies and people who also provide those hosting services which is going to make the platform much more robust and much more effective.

And then the third one is for security, so people can key review it and the security assessments etcetera.

And this is basically interesting, this is basically arguing that amazon should open their code, and again it doesn't need to be open source it could just be a license not basically to disclose the code. Although I do think that open source has a lot of advantages in terms of being able to contribute and use and taking the technology forward.

But, the concept is that for us to be able to trust this and to be able to use those and even somehow be able to consume it in multiple different places, we need it to be open, we need it to be in a way that it can be consumable. And that basically is I think a big step that companies need to have.

And in some ways, it is already happening. If you actually look at some of the companies that are doing that, I think there is already a bunch of examples of companies who kind of provide a service and then they open source it.

And I think you already have two variations, you have companies who start as a tool, let's say hosting a tool, a blog engine and then eventually the owners of it realize that they also should provide hosting services, and that is natural, the code starts open source and just be able to provide hosting service on top of it.

The other one is code that actually starts some ways internal applications and then people release the code someway for the reasons I have already mentioned above.

And in fact the other thing that can happen is what happened currently with Etherpad, where after they were bought, basically Google who bought them made a decision of releasing the source code in a way to allow that technology to live, and in a way not to piss their customers.

So I think that way we are looking it in terms of open sourcing is that how much interesting development where companies actually provide the source code of these hosting apps.


### On Ideas

So part of the reason why I am trying to do more blog posts like this and more documenting is that there is a very interesting phenomenon that happens that once you start documenting ideas or exploring a particular idea, other ideas come out of it.

And in some ways, out of the noise of all this bunch of brainstorming and basically big ideas, that someways the good ones actually arrive at the end.

And for now I was just thinking of an interesting idea and I just forgot what it was and it is really, really frustrating because it is a bit like this little bird you had in your hand that you just let it fly.

And now, if I can remember what happened, or what that idea was then I am never going to have it again, at least not on that format. And it is a really, really frustrating exercise because sometimes not that particular idea that was good it was the one that I was going to create from that or the one that would...to write a blog about it or I was actually going to start you know document it then that is how it works.

So, one of the things I have done tens of times especially as I go into this sort of static analysis well is that I write basically notebooks, I write notebooks after notebooks, after notebooks just literally ideas. Everything that comes to my head I just start writing it down.

And in some ways some really, really interesting and powerful ideas come out of it and it is usually like the third phase when the real stuff comes out and you really come up with really, really interesting and simple ideas and ways to actually address the problem.

And in some ways if you look at my work on O2 platform it is all about coming up with ideas to solve particular problems and exploring tens of different directions until you are actually able to really figure out what is actually happening. And basically what is the best way to solve a particular problem, and of course it all comes down to ideas.



### On Lack of automation on the web world

One of the interesting things that is happening with the current if you look at the web world, is that we have a tremendous lack of automation.

It is really sort of amazing how little automation exists on websites and between websites and between the stuff that I do and the materials that I consume.

For example, if I want to move data from one provider to the other, there isn't an easy way to describe how that should happen. If I want to make a bunch of actions on a particular website or a couple of modifications on a particular web page, you know it is almost things like cruise monkey are the only small examples of what needs to happen.

But, I think the problem is that because we don't have web automation, you don't have services providing around these automations. And we don't have basically a healthy promotion and a healthy model that promotes the development of tools, API protocols for enabling that automation of web assets.

We are going a bit on the right direction because by creating the whole web services and AJAX and dynamic sort of content by the semantic web, the separation of coding data that is all good but I think we need a much more focus on this kind of automation of web process.

In fact, I think there is a lot of interesting businesses that you can actually develop and services you can charge by just enabling that and providing that.


### Openness level of a company

In terms of how open a company is, so if a company all its intellectual property and assets are open, for example open like open source, surely then in terms of level of transparency you are going to start to increase that to the stuff that is produced internally.

So all documents, or internal documents could be made public and eventually all emails, at least let's say a particular email account could be made public. Because we already have twitter messages and all that stuff public and blog posts so that would just be an extension of it.

In some way, that will allow customers to figure out what is going on, gain more visibility to what is happening in that particular company. And in some ways, it probably would allow the company to scale a million places, scale much more comfortably in the open informative way.

_(after all there are already a number of non-authorized parties that have access to the data)_


### SAST market value ###

_Question - how big would the static analysis market be if it actually worked?_

So here is a question, how big would the application security, the static analysis world would be if it actually worked? If we were actually able to look at one app, scan it and get a really in depth analysis of what the app does, what are the security side effects and what needs to be re-mediated in some ways, different information about what needed to be re-mediated?

And in fact one could argue that even if you already had full blown good samples and full blown examples of what should be changed, it still will take a bit of a while to fix.

But someways the question is, how big would that market be? And I think it will be enormous, because ultimately once we can do that, we are actually looking at business intelligence straight into the eye. And we actually have a massive market in front of us, because theoretically every single app, every iphone app, every firefox app, every windows app, every shareware app needs to basically go through one of these reviews.
