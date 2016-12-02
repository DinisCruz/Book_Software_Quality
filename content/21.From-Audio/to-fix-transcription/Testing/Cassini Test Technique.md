### Cassini Test Technique

One of the problems I had when I was writing tests on asp.net was to render the page. The latest version has made it better with the various APIs, but the issue of rendering is still very relevant.

I solved my problem with rendering by running Cassini in the actual test. Cassini is a very lightweight .net web server memory. When the test started, I started Cassini, loaded the application, and then I could communicate with it from my tests.

This was a spectacular result because it immediately gave me full access to a writing server. The rendering worked and the connection worked. By making the request to the application, all the routes would work, all the views rendering would work, and this allowed me to write much more interesting and powerful tests.

Another interesting problem occurred because the tests and Cassini were running on different app domains. I solved that problem first of all by creating a nice bridge using the O2 platform. I used reference techniques which allowed me to directly access some of the back end objects. 

So I found ways to inject stuff and connect stuff, because what I really wanted was to write a test that sees what happens with the application when you modify certain configuration files. So let's say you have certain configuration files that are likely to access some stuff, but others don't. How do you make sure the files are actually still working?

I would start a test, Cassini would start and eventually we got Cassini to start literally in seconds, in fact in milliseconds because we trimmed everything so we would just start the application with no state. Then we would start to modify the configuration values, because we exposed the configuration properties as much as our reference, and then I would just go to the view and see what was there.

So that was very powerful because I was able to flick the different configuration options and confirm that the UI and the application still behaved in that particular way. 

Sometimes, what will happen is you have all these security blind spots or all these business logic blind spots where you almost have this convention that things must work but they actually in practice they don't work or they aren't being enforced.

You have these changes in settings that are supposed to determine if the user can click this, or do this, or perform this transaction, but they are not enforced in the code. 
