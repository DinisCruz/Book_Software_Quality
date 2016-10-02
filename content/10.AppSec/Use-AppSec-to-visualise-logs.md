### Use AppSec to visualise logs

Once you've got your logs, a typical challenge is how to process, and visualise them.

This usually happens when you try to address visualisation as a whole. But until good filters and multi-stage-analysis are in place, there is just too much data, too much information, and you will be left struggling with the sheer size of the data you are looking at.

The key is to create an environment where we are only querying an subset of the data, with fast queries and REPL like workflow.

One of the ways to manage this is to start with a small AppSec question (ideally codified as a Test).

For example, take an known exploit (_"here is an vulnerability being exploited, can you find it?"_) or a good active defence (_"we know the application is protecting from brute force attacks, what are the user accounts affected?"_), and use them to create visualisations of the answer(s).

Run the tests (i.e. exploits) every hour to generate enough log events, and then work on our dashboards and analysis scripts, until you have enough visibility in your log visualisations.

This is a much more efficient way to figure out how to visualise your logs.

**Other interesting AppSec Questions:**
  - How many attacks do we receive per day?
  - When does the CSRF token fail?
  - Are there POSTs submitted as GETs?
  - What headers or cookie values are being used on Injection attacks?
  - What pages/resources have triggered Authorisation exceptions?
  - ... see [AppSensor Detection Points points](https://www.owasp.org/index.php/AppSensor_DetectionPoints) for more important questions to ask (i.e. activities to detect)  


(todo: merge with diagram and text from [Test execution and lack of visibility](https://github.com/DinisCruz/Book_Software_Quality/blob/master/content/22.Diagrams/5.Test-execution-and-lack-of-visibility/5.Test-execution-and-lack-of-visibility.md))
