**The business model of selling a fork**

An open source based business model that I really like, is the idea that the company (or team) behind a particular open source project, sells a fork of the master repository, that is customised and/or maintained for a particular customer.

What that means is the customer buys access to a fork, from the authors of that particular code/repo/project.

That way the company developing the application has a direct connection with the client, and a regular revenue stream.

This also creates a way for the main team to understand exactly how this software is being used and customised.

When there is a new release, the first step is to upgrade the client's forks (maintained by the main devs) and see what breaks. This process needs to be as transparent and smooth as possible (after all, that is what the client's are paying for).

The problem of having to maintain the different versions is now in the hands of the original developers. This  always leads to better designs and maintainability because it tends make customisation a first class citizen (vs an afterthought).

By making the developers responsible for maintaining the new versions, it forces a huge amount of thinking of how to actually maintain and upgrade all the different forks (i.e. the key users of that application/module/api).

This model is much more efficient because the cost of incompatibility and breaking changes is paid by the ones that make those changes.

Compare this with what happens in most other cases today, where it is the client's developers that pay that cost. This helps to explain why teams/companies don't like to upgrade their dependencies (which has enormous security implications)
