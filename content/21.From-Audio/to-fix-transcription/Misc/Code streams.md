**Code Streams**

Once I had the method streams, I started to look at what else could I do with them. I realized that I could also start to follow the individual code assignment. I created what I call code streams, which is basically each individual path as I was able to calculate them. 

You follow variable assignments, you follow the variables being called and then you come up with a list of location source code and the exact locations in the column and line of where the call is. You now have the equivalent of what a lot of static analysis engines do: you have source to sync technology being followed.

The key power of this is both method streams and code streams have API so you can program them. The real value comes after you have developed this technique. I remember a case where I was able to glue calls. I was able to glue a particular web service's calls so I could create a method stream that would join them. The code stream now started on a website, then transversed to a web service, and ended on a SQL statement. 

I was able to do things where I would resolve SQL queries through procedure perimeters, and then inject the code of the start procedure in the actual file at a place where XML validation or parsing occurred before I hit the web service.  This allowed me to put that at the top so I was able to confirm which fields were tainted, even from the point of view of the web service.

That worked really well because, again from a code review perspective, I had all the information available. That is what we should aim for: we should aim to grab any point in the application, but namely the attack surface, or the methods that are exposed to attackers, and we should be able to say, "Show me all the code that goes from here, show me all the methods, all the variables, all the dependencies, all the filters. In short, show me every bit of line of code that passes through here". 

And that is when you really get a good sense of what is going on and what is really happening on the application.
