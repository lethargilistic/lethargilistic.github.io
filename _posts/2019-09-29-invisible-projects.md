---
title: Invisible Projects
published: true
description: I finished a project and nobody will see it.
cover_image: https://thepracticaldev.s3.amazonaws.com/i/14viefk4b1aprxgrxvxp.jpg
tags: volunteering, career, opensource, living
---

*This has been sitting in my drafts since October 2018, so consider that "the present" while reading this.*

Over the last year, I've been doing some volunteer work on Wikipedia: improving their coverage of various Supreme Court cases involving copyright, a legal construction [I've loved learning more about](http://www.thepublicdomain.org/). Because our goals aligned, I involved myself with the United States Supreme Court WikiProject and started helping with some open tasks. As I read archived discussions, I found one issue came up consistently, over and over, for years.

Each article on a case has an infobox that includes a list of the justices serving at the time the Court decided it. Their system for populating this information [used a key-value pair](https://en.wikipedia.org/w/index.php?title=Template:Infobox_SCOTUS_case/doc&oldid=861422620#Court_composition_key) that matched the years of a particular court membership to the particular list of justice. Every time you had to change which list displayed, you had to look up the key on a different page and suss out which was correct yourself. The system did not cover gaps where the bench had empty seats, so cases would often list justices who weren't even involved. If the Court membership changed twice in a year, they used a "1969b" notation as a patch. This was dreadful and everybody hated it, again, for *years*.

I thought it would be fun to fix, so I started working on it in April. My new solution would automatically populate the correct Court membership based on the case's decision date (or, until then, the oral argument date), so later writers would never even have to think about this issue again.

I started by scraping a table with justices' names and the dates of their oaths of office from the web, then I rearranged them into proper lists of the Court's membership after every change that has ever happened. After that came a lot of tedious detail work like collecting all the proper links, separating the project into a subpage and rewriting the template as a call to that subpage, writing new error handling, or figuring out the often-strange constructions that Wikicode's designers used for conditional display. I'm not sure if this is making it sound like I'm downplaying the difficulty or puffering it up to sound more difficult than it was, but it was mostly just time-consuming and took even longer because I wasn't working on it continuously. Still, I enjoyed solving a problem for a good cause and making some nice people's lives easier. It was good work that I'm proud of and it finally [went live this afternoon in October](https://en.wikipedia.org/w/index.php?diff=863265125&oldid=861421637&title=Template%3AInfobox_SCOTUS_case%2Fcourts&type=revision). Yet, as I reflected on a job well done, I realized that I didn't feel particularly good about it. Why? Because my first thought was that nobody was going to give a shit.

If I was employed as a developer, this wouldn't bother me because people would assume my competence and I could do things like this as fun asides. Because I'm not, projects like this seem all for naught, proof that I can do my job that may as well be cast into a void.

Of course, there's satisfaction in solving a problem that had been plaguing a small community for years, and I'm happy to have done it. I just wish that the messaging from the software industry wasn't that my free time and good deeds must always be in service of my career.
