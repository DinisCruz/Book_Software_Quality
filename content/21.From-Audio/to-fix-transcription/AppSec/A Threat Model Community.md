**A Threat Model Community.**

At the moment there is a space within the application security world for a community focus on threat modeling. This is a community where information from the multiple parties that are currently doing threat modeling are shared and important voices from all the different players are able to be mapped. 

For example what do developers think, what do managers think, how do we name or what do we name an issue. All those little things matter because they are the ones that really allow us to understand the best way to do threat modelings.

At the moment, 99.9% of threat models are done inside companies, in preparatory environments that don't share that information. And sometimes it isn't even that they don't want to share, it is just that information isn't any easy to share so it is a pain. And of course, what happens is things don't get shared. 

So, one of the advantage of doing this in a community, in an open way with clear licenses and clear open standards on how to communicate is it forces us to solve the problem of how do you separate confidential data from generic public data and also how you version it.

Because versioning is a massive problem, it is very complex you end up versioning using file names and all sorts of stuff which doesn't really work at scale. And that prevents us to for example understand the evolution of a threat model from something that is small, something that gets bigger, something that then slows down again, something that gets small again based on the fact whether threats get mapped or not. And that versioning is actually very important. 

For example one of the visualizations I really like is the idea that you have a particular threat model of a particular feature of application that is reasonably self-contained or kind of in a good state. And then suddenly you add a new feature and the whole thing explodes.

Because basically what you have is a situation where the new feature just created a bunch of issues or hosts a bunch of vulnerabilities which certainly are much more easy to visualize in a state where you can actually see the new connections and the impact of that simple connection. 