**Cassini Test Technique**

One of the problems I had when I was writing tests on asp.net was to render the page. The latest version has made it better with some of the various APIs but it is still very relevant.

So, the solution was to run Cassini which Cassini is a very light weight .net web server in memory in the actual test. So basically the solution was when the test starts, you would start Cassini which is a memory, load the application, and then you would communicate with it from your tests.

So this was spectacular because immediately it gave you full access to a writing server, the rendering was working, the the connection was working basically you just make request to the application and all the routes would work, all the views rendering would actually work and allows you to write much more interesting and powerful tests.

Now there was an interesting problem that occurred because the tests and Cassini were running on different app domains. So the way I solved that problem was by first of all creating a nice bridge using O2 platform but you are just using object by reference techniques and basically allowing me to actually start to talk directly to some of the or access some of the back end objects. 

So I would find ways to inject stuff and connect stuff because what I really wanted was to be able to for example write a test that sees what happens with the application when you modify certain config files. So let's say you have certain config files that are likely to access some stuff and others don't how do you make sure that that is actually still working?

So, that is a really good example of I would be able to start a test, Cassini would start and eventually we got Cassini to start literally in seconds, in fact it was milliseconds because we trimmed everything so we would just start the application with no state and then we would start to modify the config values because we exposed the config properties as much of our reference and then I would just go to the view and see what was there.

So that was really, really powerful because I was able to flick the different config options and confirm that the UI and the application still behaved in that particular way. 

And that sometimes, what will happen is you have all these security blind spots or all these business logic blind spots where you almost have this convention that things you work but they actually in practice don't really work or not being enforced.

So, you have these changes in settings that are supposed to determine if the user can click this or do this or perform this transaction or do this stuff directly and they are actually not enforced in the code. 