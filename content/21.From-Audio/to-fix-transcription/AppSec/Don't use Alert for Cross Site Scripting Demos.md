**Don't use Alert for Cross Site Scripting Demos**

An alert should only be shown when the audience understands exactly what the alert means.

Popping up an alert is a very dangerous thing to show to a client or a business owner if that is the only demo you have. The problem is, an alert only means that there is a minor inconvenience on a particular application; an alert isn’t hugely significant in itself. Instead of popping up an alert, you need to create demos that exploit the business of the application, and that show how bad and how dangerous it can be if the application is running malicious JavaScript.

Your demo should do things like change the logo, add disclaimers that will alarm the legal department, do transactions on behalf of the users, modify the users' content, and prevent the users from doing things on the actual page.

By creating this kind of demo, you are translating what malicious JavaScript execution actually means in a particular business. The good news is; you don't need the cross-site scripting demo to do this because you can always simulate injecting JavaScript. Sometimes an easy way to do that is if there is any non-TLS traffic higher up that could be used. Alternatively,you could just inject it directly to the script on the browser, or on the server.

Once you have a cross-site scripting example on the application, you can use that same demo. This is very powerful because you are really showing the dangers of malicious JavaScript. At this point you could show the alert, because its appearance now proves your point. However, even if the pop up isn't easy to execute, you can still run arbitrary scripts, even JavaScripts.

Don't get too concerned with trying to show the pop-up; the point is to execute JavaScript. One interesting example is to look at angle applications that have some protection. The fact that you can do cold callbacks into the application means that sometimes, even if you don't have access to the full JavaScript suite of coding capabilities, you can still do a huge amount of damage, especially if you are now reusing tokens that have a lot of power in the back end. 

A script can invoke some command that is going to heat the back end as the current user. Although it isn't a full-blown remote code execution, it might be enough. A typical example is where you find putting a bit of payload on a page of an HR system that is supposed to improve a time sheet, and the only script you can run is script that exists on that page for the administrator to approve a particular time sheet. That is all the attacker needs to exploit that application.
