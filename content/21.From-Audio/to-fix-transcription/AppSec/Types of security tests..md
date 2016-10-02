**Types of security tests**

How to review a test and figure out if it is a network security assessment or an AppSec assessment. 

When you look at a pen test, you can tell very quickly if it was done by somebody who understands AppSec, i.e. somebody who can code, a programmer, or somebody who can run a very good external penetration test. The pen test might also have been done by somebody who most likely cannot really code very well, but might have a very good security instinct or security knowledge from the point of view of network security.

The first main points to notice are if they asked for the source code, and if they did a threat model on the application. If they didn't do that, then it is most likely going to be a network security assessment.

You can also learn a lot from the findings. If you see lots of network scans or ports open in the findings, if you see  something like Burp or another proxy being used a lot, and if the kind of findings tend to be more browser-based, these are very good clues that a network security test was actually carried out.

Clues from a stronger AppSec will be how many scripts, and how many tools were actually created during the test.

So, if you see lots of customization, custom scripts, and all sorts of tools that allowed them to really test the application, then it is  more likely to be somebody who is doing AppSec but couldn't have the code, so they had to come from the outside.
