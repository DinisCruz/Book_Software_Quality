**Describe risks as features**

Describing risks as features not wish lists. It is key to describe the exact behavior not what you think, so you don't say application should encode value, you say application doesn't encode value. 

You don't say application shouldn't be vulnerable to scripting or SQL injection, you say this application is SQL injection.

And that is key because what you are describing are...and vulnerabilities are features, and vulnerability is a feed of an application. If an application is direct opposite reference, then that is a feature. User A uses B data.

And that is the risk you open, so the idea the risks should represent the feature. And in fact, sometimes you open risks for the same feature because what you want, you want to make technical and business audiences understand what is going on.

Sometimes you have to say we have a direct opposite reference vulnerability here risk you also open to the one that says user A can access user. In a way they are dependent because one is caused by the other.

I remember this funny story where I had a SQL injection and the business would say well we have backups with good database backup. So, SQL injection is not our problem. And I can drop all tables and they go, yeah but we can recover from that very first problem. 

And they might argue well we can delete data they will go well we have read only access and we can protect it from there. Then I am sure well we can log in as end user with a typical you know single code as or 1=1...and then we will fix that.

Because suddenly I was able to show that I pass the business logic of the application using 02 and that is the big problem. It isn't about data corruption or deciality in this particular case, what it is about is business logic, the lack of rebiviation of knowing which user actually did what.