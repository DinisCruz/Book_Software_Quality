**Code Streams**

Once I had the method streams, I started to look at what else could I do with it and I realized that I could also start to follow the individual code assignment. So what I did was I created what I call code streams which is basically each individual path as I was basically able to calculate them. 

So, you follow variable assignments,you follow variable being called and then you come up with basically a list of location source code and the exact locations in the actual column and line of where the call is. And basically by that you actually have the equivalent of what a lot of static analysis engines actually do which you basically have source to sync technology being followed.

And the key power of this is both method streams and code streams have API so you can program it. So in a way the real value came after you had this technique. So I remember a case where I basically was able to glue calls. So for example a particular web services calls so I could create a method stream that would join them and where the code stream now would basically start on a website and then transverse to web service, ends on a SQL statement. 

I was able to do things where I would resolve SQL queries through procedure perimeters and then inject the code of the start procedure in the actual file at a place where there was XML validation or parsing occurring before you hit the web service, so I was able also to put that at the top so I was able to confirm which fields are actually tainted even from the point of view of the web service.

And that was something that actually worked really well because again from a code review point of view, you have all the information available. And I think that is what we should be able to aim, we should aim to grab any point in the application but namely the methods that are exposed to attackers so basically the attack surface and be able to say, "show me all the code that goes from here, show me all the methods, all the variables, all dependencies, all the filters in a way every bit of line of code that passes through here". 

And that is when you really get good sense of what is going on and actually what is really happening on the application.