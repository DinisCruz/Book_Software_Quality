### Protecting Legal and Compliance Text on Websites

Find data on your websites that has to be signed off on by lawyers, for example, translations or legal notices.

You then assign Risks based on current QA's SDL maturity and capabilities (i.e. it's ability to protect/detect that text from changes).

What to look for:

 - very little control over the integrity of the code/content
 - several different developers accessing it without strong code review checks
 - loads of javascript being injected on the web application (namely ads)
 - small numbers of tests executed against live production systems
 - no ability to easily write tests that confirm the integrity of data

What usually happens is an inability to guarantee the integrity of the data that exists on the website, which for the lawyers that signed off those legal and compliance texts, is a BIG deal.

Asking the question _'can we run a test against production and check that the legal text is still there and hasn't been changed?'_ will highlight all sorts of gaps in a QA SDL workflow and environment.

What this means is that suddenly the security and QA capabilities of an application are important to the lawyers/compliance teams, who will ask for assurance on that content.

We will then have a situation where they are the ones that are putting pressure to have a much more solid SDL with a lot more testing.

This becomes very real, when the Risk caused by: rushed projects, weak briefs, code that is pushed into production with no security checks; is also assigned to lawyers.
