### Application Security Testing Tools (SAST, DAST, IAST, RAST)

- Static analysis vs Dynamic analysis, which on is better?
 - that is the wrong question
- you need both types of analysis. You need static analysis to tell you how the app works and then you need dynamic analysis to take that information further to test and make sure the issues are actually exploitable.
 - these tools should be feeding into each other
 - some HP and IBM appscan teams tried to do this (and it worked okish), but a lot more is needed (for it to work in real world apps)

-  The goal is to find a way to leverage the best of both worlds - have tools that provide both environments or be able to consume each tool that provides every piece of the equation, because application security testing is very complex and requires two completely distinct sets of skills.

- we need to merge those two worlds and treat them as one and use those technologies to perform security analysis.
- we need common schemas to exchange data, knowledge and findings
  - for example the attack surface of an app

- the key here is to mention the need to have multiple tools running on the code
- mention IAST and RAST
- mention DHS project that runs multiple scanners on same codebase and consolidates reports
- mention ThreadFix (https://github.com/denimgroup/threadfix) and its capabilities to load multiple tools results and consolidate findings
