### Putting Data in PasteBin

One of the best ways to make Developers, Architects and Managers understand confidentiality of data hosted by their application, is to ask the question, _'Can we put all of the data on your database on PasteBin?'_' [^PasteBin]

That question makes all parties involved really think about what that database contains.

Ideally, the correct answer is yes, there is no problem. All that data could go to pastebin because the data shouldn't mean anything by itself.

That's what you really want, you want your database to be in a situation where there is nothing truly valuable in there when it exists by itself:
  - all the sensitive data is encrypted
  - all the ID are be tokenized
  - there is be way to de-anonymize that data
  - every single asset in there should be random from the point of view of the database itself

The Threat Model of a database with sensitive data vs one without is very different (which is another great way to visualize the differences)


[^PasteBin]: [Pastebin](http://pastebin.com/) is a website that allows anybody to paste data into it, and is a common location to dump confidential data, as can be seen by HaveIBeenPwned's collection of PasteBin data (https://haveibeenpwned.com/Pastes)
