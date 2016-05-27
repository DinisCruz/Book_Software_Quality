**My development pipeline.**

Here is my current continuous integration work flow for the BSIMM graphs project. So, I have two main projects, I have the BSIMM graphs and the BSIMM QA. So, when I push so I make a code change on the BSIMM graphs project, when I push a code change I commit it locally, and I then push a code change to Git Hub.

Git Hub sends a web hook to Travis that triggers a build. Now, Travis will first build the application so build all the components make sure all the integration are up to date, everything from scratch is okay.

And then, it runs all the unit tests. So, these are the more traditional unit tests and component tests on the application. If they all pass, it then will run at docker build.

So the docker build will build the docker image...the docker build will build the docker container and the docker container is then pushed into docker hub. Now, when the container arrives at docker hub, I have configured docker cloud to monitor it and to deploy that to a docker host which is running in digital ocean. And will deploy that new version into digital ocean.

So, what it means is at this stage, as soon as my docker build is complete, within a minute or so, I have it deployed into production like environment. And then what also does at the end, it will do a push into a fork of the BSIMM QA in Git Hub. And this is Travis, so Travis will do a push into Git Hub to a particular fork and what happens is when that push hits Git Hub on the BSIMM- Graphs- QA Repo, that would trigger another Travis process.

And what this will do is this is a Travis process of the QA code which will run two sets of tests. It will run in fact three things, it will grab a copy of the docker image and it will run it locally. And basically what it means, it now means that in the inside the Travis build, there will be a docker container that is actually running locally.

And then what happens is that you are going to run two batches of tests, you are going to run HTTP driven tests, and browser based tests. The HTTP basically hits the network, they are bet to the metal, they directly it will request the application and they are very powerful to test specific things that don't require browser automation like APIs, heathers, the specific request authorization rules e.t.c. and easy security tests because they run very quickly.

Then you also have browser based tests which are equivalent to selenium but they are using electrium which is a new tool I will be working on which does browser automation using chrome. And that runs the whole typical browser automation tests which go to the normal user criteria tests all the way to [inaudible 00:05:50 H cases] all the way to security.

And after that, only after that you then are going to get another trigger which will basically push this code base into a pre prot base server which will contain principle, deploy able and ready to be go live application because at that stage it has passed all the tests all the way and it is all going okay.