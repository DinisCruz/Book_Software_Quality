### InfoSec lack of respect for users

InfoSec (Information Security) tends to have a really bad attitude towards end-users of technology and developers, where they (the users) get blamed for doing 'insecure stuff' and causing 'security incidents'.

This is crazy, it is like health and safety officers complaining that people are 'doing things', so it puts them into danger.

The fundamental logic is that security is there to empower users, not to be a tax or dictatorship.

Information Security works best when it allows the users to go faster,better, safer, cheaper. Just like brakes in cars.

For example if users/developers run their desktops with admin privileges (required to install Dev tools, but not all the time) which causes an security incident. Who is responsible? In most cases it is actually InfoSec's problem (which should had provided better solutions and workflows).

This is not saying that the user is blameless. But that the user/developer should be given secure alternatives to do what they need to do in a day job in order to be productive (i.e. without needing admin rights, or be temporarily elevated).

Containers and Virtualization for example, allows a user that wants to run an application requiring admin privileges, to do so in a safer, isolated and disposable  environment. This can be done locally or in a VM (which the user can remotely desktop into).

It doesn't help that in our current IT infrastructure and development environment, large number os tools require admin privileges. But that doesn't prevent that we implement solutions to isolate them.

 - (add comment on [SmartOS](https://www.joyent.com/smartos) and the Windows Edge concept of [using containers](http://www.itworldcanada.com/article/microsoft-touts-container-protection-for-edge-browser/386876))

The bottom line is that InfoSec tends to really unfair approach to user's actions and behaviours.

Unfortunately the same happens in AppSec where developers are blamed for all sort of code issues (a lot outside their control) and are referred to with derogatory terms.

My experience is that most developers are very intelligent and knowledgeable. They deserve respect. In fact, in most cases the quality or security issues they code, aren't really created by them, but by the eco system and the environment that they are coding on.

- (add ideas from blog posts on the 'development environment needed for secure coding', 'making security invisible')
- (add comment about 'the crazy idea of telling users not to click on links' [#196](https://github.com/DinisCruz/Book_Software_Quality/issues/196))
