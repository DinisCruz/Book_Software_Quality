### Method Streams

Method streams are very powerful code review techniques I developed when I was building the O2 platform.  I created one file that holds all the methods and all the codes that I called from a particular method.

Imagine you have this stream of code which is all the code that is executed from a particular starting point. This is a very powerful code review, and security analysis, technique because you are able to follow the code quickly and understand what is going on.

I created method streams by using the code complete technology I had added to O2 which was based on a re-factor. This allowed me to know at every moment in time both the code I could transverse the AST, and which method was being called.

In a way, a method stream is a mixture between two code technologies. One technology is re-factoring, where I take one method and rewrite it into another file which is how re-factoring works. From there I have the ability to pick any method and just rewrite it in another file. And then I used code complete information to know the actual full type of the method being called. And then it was a case of putting them below and running that loop recursively until I had all the objects created.

So the workflow is you point to a method, then you are able to generate recursively in a reverse call graph of everything that is happening, and you use that to populate the re-factoring object which you can then print out as one file.

The power of this method is that instead of having multiple files with your code, and each file has a bit of code that you need, with a method stream you have created one file that contains all the code you need. This is a very powerful code review, and static analysis, technique. 
