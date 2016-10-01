**The currency of AppSec is provability and assurance**

When we (AppSec) make a statement about a particular security issue, it always be clear and unambiguous.

We should never say "This might be a problem", or "That might be exploited". When it comes to problems or weaknesses in AppSec, we have to express ourselves with confidence.

In cases where we don't know something, then we must be confident that we don't know. We have to make sure people understand that if we can't prove exploitability, or if we have doubts for example that exploitability is even possible, then we must clearly state that we don't know that a problem exists.

I find that this uncertainty occurs especially in relation to static analysis results, or tools results. Sometimes the information and knowledge emerging aren't absolutely clear. We can look at these results and say "Oh, we think this is a problem", but that is just not good enough. We have to have assurance, and our currency has to be highly defensible findings. We need to be able to show that every time we speak about something, we have the data to support what we say. We have to provide assurance.

When something is potentially vulnerable, we have to prove it.

But even if something isn't a problem from an all accepted attack vector (like internet-based payloads), it might be a problem inside the application or exploitable from an internal . You need to follow the lines that show where something is exploitable, where it isn't, where there is a problem, and then where the dependencies are.

Demonstrating problems in this way puts you in a much stronger position than when you end up having a huge number of findings that are easy to dismiss, because people can't fully understand them, or don't really understand if a risk is probable or not.

Even in a worst case scenario where you don't have evidence, then your statement of fact must be that you don't have evidence. When you speak clearly like this you're not saying that no problem exists, you are saying that at this moment you don't have the time to make a decision, or that you don't have the time to research whether something is problematic or not.  Speaking clearly like this makes it easier to convince someone to accept risk.

What is absolutely key is all information and findings reported from AppSec is done in a way that is reproducible in both the dev's an the CI environments. This can only be achieved by Tests.
