**The names of methods.**

The way I look at it, the key of a method's name it is its readability and it is maintainability. The key requirement is to make sure that when we look at the method implications we understand what it is going to do, and we understand its side effects.

So that means that in the method's name you should always err on the side of maintainability. I like to call it the Monday morning after hangover concept. Which basically means that when you arrived in your coding environment, and you are still a bit, not 100% and when you type on that dot, and the code complete turns up, whatever you feel should be the name of the method that should be the name of the method.

Now what this does is if you have a very flexible and easy to re-factor code base, is that the names of the methods will evolve. And they evolve because you experiment and you would start to understand better how that method is supposed to be called.

So if I for example have an object string or something that represents a folder, I should just be able to go dot[.] files and that should give me all the files, if I go dot [.] file names that should give me all the file names. If I type dot [.] folders, that gives me all the folders. 

But sometimes, I might want to change it, sometimes you might not feel right to say files, sometimes it might feel right to say items because that is what they represent.

So, the way I look at it is the name should be in context for the application that you are working on. And what that means, it means that sometimes you have multiple names for the same function. Because in a particular code path, there is a name that makes more sense, sometimes it is open, sometimes it is load, sometimes it is get, sometimes it is fetch, sometimes it is retrieve, sometimes it is whatever, right? 

It is basically it should be in context for that particular flow. And the idea is that should make the code easy to read, should make it easy to understand what is going on. Which basically means that you have to keep going on, it is constant re-factoring until the name of a method at a particular function is just right.

And in the beginning it takes a while, but after a while, you realize that when you are coding you just blew it because the name of the method is already there, it is already figured out how to represent what you want to represent.

The other key concept is the method should obstruct the complexity of what they try to do and you should keep re-factoring that. So, you see that in a lot of languages where ultimately you want to do something and it is very complex. You see the technicalities of what you are trying to do at that moment in time. And the way I look at it is that should be one level below or two.

So if I want to get for example some network request, I don't want to care about all sorts of technicalities about streams and error handling and all that jazz in the beginning. I just want to basically say give me this and come back. And if it doesn't work just give me a no, or no value.

Because that is what I want at that moment in time. Yes, there are cases where I might want to do something more specific, there are cases where that isn't good enough but we need to make sure that the use case that the user has or that that developer has at that moment in time is very, very easy to do and very straight forward.

So, going back to the names, the names should represent easily what the actions are that you are actually doing.