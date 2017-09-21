---
layout: post  
title: Blogging About the PostgreSQL set_user Extension  
tags: PostgreSQL

---

For my day job, I've been posting about the set_user extension, which BigSQL now includes in our Postgres distros. 

Here is the first post (I'm writing a series and will add as I move along). It's a necessary enhancment to your PostgreSQL in today's world of data breaches.  Read on...

# BigSQL + set_user Extension

We are excited to announce our newest addition to the [available components][1] with BigSQL PostgreSQL Windows, Linux, and OSX distributions: [set_user 1.4.0][2]!

And... to kick it off, we will be writing multiple posts about this essential security extension.

But first (for the uninitiated) some context...

<img src="https://wwwres.openscg.com/wp-content/uploads/2017/09/14215449/enron.png" alt="" width="125" height="123" class="alignright size-full wp-image-13023" />

Since the [Sarbanes–Oxley Act][3] passed in 2002 as a response to the Enron/Tyco/WorldCom scandals, auditing a user's (esp. superuser's) access and interactions with data has become a requirement by law for publicly owned companies:

> Section 302.4.B – Establish verifiable controls to track data access. Requires internal controls over data, so that officers are aware of all relevant data for reporting purposes. Data must exist in a verifiably secure framework which is internally controlled.

Companies storing financial data are particularly vulnerable to hacking attempts as has been reiterated in the latest [Equifax breach][4].

In addition, organizations that deal with human subject data (e.g. health and research) are bound to [HIPAA][5] and/or [IRB][6] rules that if violated, can result in jail time.

<img src="https://wwwres.openscg.com/wp-content/uploads/2017/09/14215943/mr_robot.jpeg" alt="" width="200" height="113" class="alignleft size-full wp-image-13028" />

And.. as fear of hacking, invasion of privacy, and possibly worse in an uncertain technological future creeps into our collective consciousness... securing our data has become a top priority for all IT professionals.

No company (or DBA) wants to end up as a headline in the daily news or the inspiration for the plot of another modern day dystopian television show.

### set_user extension

Panicking yet? Well, you can take some proactive measures to better secure your data and avoid disaster. One component you can add to your security toolbox is the PostgreSQL set_user extension which provides:

> Privilege escalation control at a granular level; and the required audit trail of actions taken by a user while its privileges have been escalated.

<img src="https://wwwres.openscg.com/wp-content/uploads/2017/09/15021732/calm.png" alt="" width="76" height="131" class="alignright size-full wp-image-13037" />

Anyone who has worked on modern Linux distros is familiar with the use of sudo to control access to root (the OS superuser). set_user is the same, but for your database.

And... it is now available with [the BigSQL distribution][7].

So, are you sufficiently scared enough to stop procrastinating and take action? Are you ready to add enhanced logging and control on your superusers?

Over the next few days, we will be releasing a posts that cover installation, configuration, instruction, logging, and the advanced security options available.

Up first... Part 1: [set_user Installation and Set-Up][8].

 [1]: https://www.openscg.com/bigsql/components/
 [2]: https://github.com/pgaudit/set_user
 [3]: https://en.wikipedia.org/wiki/Sarbanes%E2%80%93Oxley_Act
 [4]: https://www.nytimes.com/2017/09/07/business/equifax-cyberattack.html
 [5]: https://www.hhs.gov/hipaa/index.html
 [6]: https://en.wikipedia.org/wiki/Institutional_review_board
 [7]: https://www.openscg.com/bigsql/postgresql/installers/
 [8]: https://www.openscg.com/2017/09/set_user-installation-and-set-up/

