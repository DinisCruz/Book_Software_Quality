**Method Streams**

Method streams are very powerful code review technique I developed when I was building the O2 platform where basically I create one file that has all the methods and all the codes that I called from a particular method.

So what it is, is imagine you have this stream of code which is basically all the code that is executed from a particular starting point. That is a very powerful code review technique and security analysis technique because you are able to quickly follow the code and understand what is going on.

The way it was made, it was by using the code complete technology I had added to O2 which was actually based on N-re factor if I remember which allowed me to know at every moment in time on the code I could transverse the AST and I could know which method was being called.

So, in a way it is a mixture between two code technologies, one technology is re-factoring where you can take one method and rewrite it into another file which is how re-factoring works. So, from that moment in time you have the ability to pick any method and just rewrite it in another file. And then I used code complete information to know the actual full type of the method being called. And then it was a case of putting them below and then running that loop recursively until you had all the objects created.

So the work flow was you point to a method and then you are able to generate recursively in a way a call graph, a reverse call graph of everything that is happening and then you just use that to populate the re-factoring object which then you just print out and you get a nice one file with all the code.

So what is powerful about this is what you are doing is you are creating instead of having multiple files with your code and each file has a bit of code that you need you have one file with everything and that is a very, very powerful code review and even static analysis technique. 