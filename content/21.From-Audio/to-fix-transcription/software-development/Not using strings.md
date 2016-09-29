**Not using strings.**

As a developer you are used to using strings for all sorts of stuff and all sorts of data transfer. The problem is the string, it is a monster, it is a four gigabytes thing that has every possible character and every possible combination which basically never happens.

So, what you really want is to have strongly typed or strongly mapped data models at all levels from the browser to the web services, to the back end, basically every moment that you cross a trees boundary. You need to apply a schemer, you need to apply a check to make sure that the data that you are receiving is in the format that you expect it to be.

And that gives you a lot of security because it means that you apply data validation and data sensitization very quickly and very soon in the application life cycle.

The other problem is when you look at the string on the field is we don't know this is the real security implications of that. So that means you are going to have to work harder, you have to go and research where is that used, who are its consumers, where does it come from, where is it going to go and it is much more hard to follow than if it is an int, or a date, or UID.

And ultimately with strings we have much less assurance of the data that we are processing. There is also a massive denial of service on performance implication because every single calculation you do, doubles the string length. And more importantly, you are generating huge amount of traffic in the back end if you allow large numbers of strings or large quantities of strings to be provided from the client brought from the attacker.


Concepts: 
- Strings are not strongly typed
- String is not a type
- add @johnwilander post on strings
