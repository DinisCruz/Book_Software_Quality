### Application Security Testing (written in 2010)

There’s a lot of talk about if application security testing is a static analysis or dynamic analysis and how all that stuff works, and the reality is that in order to know that there’s a proper application on a website or system, you need both. You need static analysis to tell you how the app works and then you need dynamic analysis to figure out how it actually works and also to test and make sure the issues are exploitable and you actually have a problem with it. So what you really need is a way to leverage the best of both worlds -- either have tools that provide both environments or be able to consume each tool that provides every piece of the equation, because it’s a very complicated world and there’s completely different skills required around doing that. So what I really want is to be able to merge those two worlds and to treat them as one and really perform security analysis using those technologies.

- the key here is to mention the need to have multiple tools running on the code
- mention IAST and RAST
- mention DHS project that runs multiple scanners on same codebase and consolidates reports
- mention ThreadFix (https://github.com/denimgroup/threadfix) and its capabilities to load multiple tools results and consolidate findings
