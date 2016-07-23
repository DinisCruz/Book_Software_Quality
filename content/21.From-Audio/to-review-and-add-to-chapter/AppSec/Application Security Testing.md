### Application Security Testing (written in 2010)

There’s a great deal of talk about whether application security testing is a static analysis or a dynamic analysis, and how all that stuff works. The reality is that in order to know that there’s a proper application on a website or system, you need both types of analysis. You need static analysis to tell you how the app works and then you need dynamic analysis to take that information further to test and make sure the issues are actually exploitable. The goal is to find a way to leverage the best of both worlds -- either have tools that provide both environments or be able to consume each tool that provides every piece of the equation, because application security testing is very complex and requires two completely distinct sets of skills. So ideally, I want to be able to merge those two worlds and treat them as one and use those technologies to perform security analysis.

- the key here is to mention the need to have multiple tools running on the code
- mention IAST and RAST
- mention DHS project that runs multiple scanners on same codebase and consolidates reports
- mention ThreadFix (https://github.com/denimgroup/threadfix) and its capabilities to load multiple tools results and consolidate findings
