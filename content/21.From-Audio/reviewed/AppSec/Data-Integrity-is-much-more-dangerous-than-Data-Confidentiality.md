### Data Integrity is much more dangerous than Data Confidentiality

Data Integrity is very difficult to manage and protect.

A large number of the current (public and newsworthy) AppSec problems are related to data confidentiality (i.e. data being disclosed or leaked on sites like PasteBin or credit cards being captured).  

But if you start to worry about data integrity (i.e. you lose trust on the status of the data that  hosted on your databases or static files), and you realize that the attack (i.e. the unauthorized/malicious changes) might have been going on for a while, you will have a massive problem of knowing where good data ends and the bad data begins.

It's very easy to recover if someone deletes data or does a mass modification (since there is a known good state and known bad state.). It is very difficult to recover if the data has been modified over time

Differentiating good data from bad data will be a very complex task, if not impossible. Specially when there might not be any alternative sources of truth (paper trails, logs of POST data, DB Transaction logs)

An added issue arises if you don't know what actually caused that change to occur.

Data confidentiality incidents can cause high profile embarrassment, some financial costs and some customer loses.

Data integrity incidents can bring the whole business down

- _find examples where data integrity has cause serious problems (for example the ISPs and financial companies that went bust (or were acquired in a fire sale))_
- _add note about how 'if the attackers tell you about it (the attack) then they are your friends' (in the long run, they will make you more secure))_
- _add information on how blockchain technology and encryption can help a lot with data integrity_
- _To review:_
 - _[Newest cyber threat will be data manipulation, US intelligence chief says](https://www.theguardian.com/technology/2015/sep/10/cyber-threat-data-manipulation-us-intelligence-chief)_
  - _[The next big threat in hacking — data sabotage](http://www.cnbc.com/2016/03/09/the-next-big-threat-in-hacking--data-sabotage.html)_
