**Describe Risks as Features Rather than Wish Lists**

It is key to describe the exact behavior and not just what you think; so instead of saying that an application should encode value, you should say that the application doesn't encode value. 

You don't say an application shouldn't be vulnerable to scripting or SQL injection, you say this application is vulnerable to SQL injection.

And that is key, because when you're describing vulnerabilities, you're describing features. Vulnerability is a feed of an application, and if an application is a direct opposite reference, then that is a feature. User A uses B data.

That is the risk you open, so the idea is that risks should represent the feature. And in fact, sometimes you open risks for the same feature, because what you want is to allow technical and business audiences to understand what is going on.

Sometimes you have to say we have a direct opposite reference vulnerability here risk you also open to the one that says user A can access user B. In a way they are dependent because one is caused by the other.

I remember this funny story where I had an SQL injection and the business would say, "Well, we have backups with good database backup, so SQL injection is not our problem." And I can drop all tables and they go, "Yeah but we can recover from that very first problem." 

And they might argue, "Well we can delete data." They will go, "Well we have read only access and we can protect it from there." Then I am sure they'd say, "Well we can log in as end user with a typical single code as or 1=1...and then we will fix that."

Because suddenly, I was able to show that I pass the business logic of the application using 02 and that is the big problem. It isn't about data corruption or deciality in this particular case. It's about business logic, the lack of rebiviation of knowing which user actually did what.
