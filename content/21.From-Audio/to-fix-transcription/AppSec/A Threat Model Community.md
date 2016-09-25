**A Threat Model Community.**

There is currently space within the application security world to develop a community focus on threat modeling. Such a community would allow the many parties working on threat modeling to share information, and it would also allow the voices of all the different stakeholders to be mapped.

Questions to be considered by this community include: What do developers think? What do managers think? How, or what do we name an issue? These questions are important because they are the ones that really allow us to plan, and understand, the best way to structure threat modelings.

At the moment, 99.9% of threat modelings are processed within companies, in preparatory environments that don't share information. This doesn't always mean that the companies don't want to share their information. It may be that the information isn't easy to share and therefore not worth the effort. 

One of the advantages of approaching this as a community, in an open way, with clear licenses and clear open standards on how to communicate, is it forces us to solve the problem of separating confidential data from generic public data. A community focus will also help to resolve issues around versioning the data.

We know versioning is a very complex problem. Versioning using file names and other attributes often happens, but this doesn’t work effectively at scale. This way of versioning can prevent us from understanding the evolution of a threat model, for example, from something that is small, that grows bigger, then slows down, and then shrinks again, depending on whether threats get mapped or not. This kind of versioning is actually very important. 

For example, one of the visualizations I really like is the idea that you have a particular threat model of a particular feature of an application that is reasonably self-contained, or in a fairly good state. However, the addition of a new feature can cause the whole thing to explode. Essentially, what you are now dealing with is a situation where the new feature has either created a number of issues, or it hosts a number of vulnerabilities. These are much easier to visualize in a state where you can actually see the new connection, and the impact of that simple connection.
