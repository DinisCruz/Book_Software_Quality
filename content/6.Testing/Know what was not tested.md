**Know what was not tested**

When you're reading an application security report (like a pentest), one of the most important questions that you should get an answer to is _'What tests did they run?'_. This is especially important for the tests (i.e. exploits) they tried to run but were unsuccessful.

The report(s) will show what was successful, but that's only half (or potentially less than half) of what you want to know.

For example, if you get a report that doesn't have any findings, is that because:

1. the testers did not look at the application/feature at all?
2. the testers did not have enough 'state' to reach the important parts? (i.e. lack of coverage), or
3. there was nothing there? (i.e. it is secure)

What the (pen)testers actually did (namely what they tried and didn't work) are actually security regression tests. They are the confirmation that app XYZ doesn't have a particular vulnerability. They also allow you to see how much coverage they have on the application.

A very good set of questions are thus:

 - How many URLs did they find?
 - How many forms/ajax-endpoints did they submit data to?
 - How many types of data did they actually found and manipulated?
 - Where they able to map the discovered site's attack surface with the provided source code?

The answers will give you the information of how good or bad the tests were and how assured you can be of its findings.

Imagine you had a building and hire somebody to test its security. If they came back and said, _"Well, the building is okay, we couldn't get in, so it is secure!"_. But then you realise that they only covered twenty,thirty or fifty percent of the doors that actually existed. At that point, you know the quality of the test itself is poor.

> _todo: Add metro bank Oceans 11 example [#154](https://github.com/DinisCruz/Book_Software_Quality/issues/154)_

In conclusion, I think it's very important that you rate the security assessment on how sure you are of the quality/coverage of their tests (i.e. your level of confidence and assurance for the results). Ultimately, what you want to know is how protected you are from each of the kind of attackers that you will face (from a very non sophisticated attack to somebody who actually knows what it is doing will take the time to find vulnerabilities)
