---
title: Hello World, Again! I'm Back and Here with Rstudioconf Takeaways
author: Rosie
date: '2020-01-30'
slug: hello-world-again-i-m-back-and-here-with-rstudioconf-takeaways
categories:
  - R
  - Conference Report
tags:
  - rstudioconf
---

# A quick note before I start

I say, "Hello World, Again", because after my first immediate interest in starting a technical blog, I ended bogged down in work, an online course, and personal life things that required me to take some more breaks from my personal projects. I couldn't keep up with my goals of blogging in 2019, and although 2020 doesn't seem to be slowing down for me, I am currently sitting in my hotel room inspired and motivated to start up this blog again.

<!--more-->

# rstudio::conf Overall and TL;DR Takeaways

### R users have a lot in common

I have no statistics to back me up here, which isn't really kosher as a data person, but based on my interactions with R users over my career, it feels like a majority of R users are people that know math or statistics or have some field of research where they need to do some analysis and/or predictions, and R is just the tool they found to get their projects done. Some of us move on and we find ourselves in R-heavy programming roles at work or in academia, *feeling* like we're trying to be engineers, which isn't necessarily something that a ton of us really started using R for.

As a result, I feel like I have a lot in common with a lot of people that come by R conferences. I end up a lot more comfortable, knowing that other (really smart!) people are also interested in learning things that people at other tech conferences might find 'basic' or standard engineering workflows. Things aren't always basic to me! ;-; 

Actually, this seems to be what RStudio is trying to help us data scientists with, which makes the RStudio conference particularly relevant to me, as an analyst that wears many hats in my org.

### The R community is welcoming and surprisingly diverse

I tend to feel like the attendees of R conferences are the most welcoming of any technical crowd that I get to meet (besides PyLadies events in my area). 

I'm not sure exactly the reason, but R as a language seems to attract less of the 'stereotypical programming' crowd online and at conferences. This conference specifically gathered the most top tier people that could attract a diverse crowd, and it encourages an overall welcoming environment with less arrogance and elitism (that I sometimes notice in other places in tech. Obviously there's good people everywhere though! Not trying to knock on other languages as a whole.)

### Go to Birds of a Feather events, especially for an awkward turtle like me

At the Shiny Birds of Feather event I got to have some conversations with various people in different industries. Most exciting to me, though was that I got to talk to the creator of Shiny, Joe Cheng, briefly! He was super nice and actually asked *me* questions about what I do. I also met Dean Attali, writer of `shinyjs` and general `shiny` master on the Stack Overflow and Rstudio Community, who was also incredibly nice. 

It's a lot easier for me to socialize in a smaller setting like these, where there were maybe 50 people at most in a room, all brought together by a similar use of R.

I unfortunately had to miss both RLadies Birds of a Feather events, although I **REALLY** regret not going.

### I actually know a lot about R aka Imposter sydrome is a real thing

At the conference, I learned new things about packages I use daily. But one thing that really resonated with me came up during a talk given by Heather and Jacqueline Nolis: sometimes I need to focus on what I know...and I know a lot! A lot of times it feels like I have an endless number of things to learn and I'm barely even getting started. It's the classic example of the [Dunning Kruger Effect](https://en.wikipedia.org/wiki/Dunning%E2%80%93Kruger_effect). 

A guy at the Shiny Birds of a Feather event asked me if I ever feel like I'm an analyst but really I'm being a subpar-data engineer & subpar-frontend designer & subpar-engineer & subpar-data scientist all at the same time. I realized at that moment that it's not abnormal for me to feel like I don't know anything. This is actually something I've talked to managers about before, and they've given me similar snippets of sage advice, but actually hearing things from speakers at Rstudio conference and fellow attendees made me feel more normal. I finally kind of feel like I'm in the right place. I feel like I can be more proud of what I've done so far even though I know that I can improve on things and make my work better - this is all part of my evolution.

### I need to use RMarkdown more, I want to build packages, and make plumber APIs!

I will go over some of this in my Individual Talk takeaways below.

# Individual Talk Takeaways - in possibly too much detail, and less proofread (just being honest)

I'm going to go over some key takeaways that I have from all of the talks that I went to. *These notes may vary in detail depending on how I was taking my notes at the time of the talk.* For those that couldn't make it, or for those who might have missed certain talks because they were elsewhere, I think RStudio will eventually post streams if they have not already (I will link if I can find them!). I also plan to eventually edit this post to add in twitter handles or conference slides/github repos if relevant/possible and I can find them! I've done my best for now, though.

**Keynote 1: Open Source Software for Data Science - J.J. Allaire** 

I was not prepared for the wonderful talk that JJ gave about open source tech and specifically, RStudio's position as a business and provider of open source technology. H also announced Rstudio as *Rstudio, PBC* (or Pulic Benefit Corporation). His experience as a programmer and a student of Political Science I think made him perfectly suited for this talk, and how to make corporate law interesting to a crowd of data scientists.

If you have not watched this talk but are interested in RStudio, I highly recommend watching the video. It makes me excited for the future of RStudio.

He also recommended two books that I have immediately thrown on my wish list:

- [Shop Craft as Soulcraft](https://www.amazon.com/Shop-Class-Soulcraft-Inquiry-Value-ebook/dp/B00273BHPU)

- [Fooled by Randomness](https://www.amazon.com/Fooled-Randomness-Hidden-Markets-Incerto/dp/0812975219)

Links: 

- [Slides are here (BUT PLEASE, watch a replay of the stream if you missed it)](https://rstudio.com/slides/rstudio-pbc/)

**Keynote 2: Data, Visualization, and designing with AI - Fernanda Viegas (@viegasf) & Martin Wattenberg** - 

- UMAP to view predictions in a multidimensional space
- TCAV to help explain why a model classifies things certain ways. 
- Both sound very cool and I'd have to read a lot more to understand them, but it is cool that Google has made tools that aim to make these things presentable to an average person. 
- This talk might be of extra interest to those who may rely on GCP for their machine learning deployments. 
- The talk also goes over some very important machine learning questions about fairness in models, human bias, and how models learn.

**Deploying End-To-End Data Science with Shiny, Plumber, and Pins - Alex Gold**

I learned that the `pins` package exists and seems to be a great way to 'cache' data and models, which seems especially handy for things like Shiny apps that need to be responsive. This seems to be a cool thing for me to explore, so I'll have to get back to the blog about this.

Links: 

- [Relevant tweets by the speaker](https://twitter.com/alexkgold/status/1222620041562058752)

**We're hitting R a million times a day so we made a talk about it - Jacqueline and Heather Nolis** 

This was a favorite of mine, mainly because I love talks about using R for production level activity (which R is usually shunned for). This talk really made me interested in serving R models with plumber, docker, and maybe even kubernetes some day? I've actually personally had a lot of fun working with docker before, so this is right up my alley.

Also:

- link to [https://putrinprod.com/](https://putrinprod.com/)

- keep track of issues

- define what 'done' means for deployment

- models aren't always the problem when people come to you with problems! it's just easy to blame the model because most people don't 'get' it

- use shiny apps to get buy in for your models

- apparently, `loadtest` is a package that exists, and sounds extremely useful!

**Styling Shiny apps with Sass and Bootstrap 4 - Joe Cheng**

Wow, if only I knew about this earlier. I've spent countless hours - days, honestly - trying to fiddle with selectors and change the default bootstrap CSS in some shiny apps for work. The package `bootstraplib` sounds like a HUGE time saver, that will use Sass (Super Powered CSS) to make important changes to shiny and rmarkdown reports. I have had to use UX designers' time before in order to get my dashboards in line with company policy or whatever, but I can't wait to play with this. Also Joe Cheng is very fun, so this talk was even more enjoyable as a result.

Links: 

- [Link to bootstraplib github page](https://rstudio.github.io/bootstraplib/)


**Reproducible Shiny Apps with `shinymeta` - Carson Sievert**

`shinymeta` is a package that seems like it could be incredibly helpful for me to add to some shiny pages where users might say that something "just seems wrong". Using this package seems like it'd save some time re-creating the issue.

Links: 

- [shinymeta package link](https://github.com/rstudio/shinymeta)

**Tech Debt is a Social Problem - Gordon Shotwell**

This talk really, really resonated with me. I really encourage people to watch it because it was really impactful on my thinking. 

Technical debt is often a result of bad communciation - it's not the code's fault, it's people. Docs might not be readable (or exist), testing could be insufficient, things just might not make sense. 

Why doesn't technical debt go away? Gordon mentioned Status Quo bias ("I learned this and I don't want it to change"), IKEA effect ("my thing is better than other person's thing"), and Parenting Effect ('it's better than it used to be/it's grown a lot at least"). These three things are ALL things that I've encountered when stepping into new roles and I didn't have any understanding before.

When approaching technical debt, find the right projects, separate user and maintainer, and *empathize* with the debtor. I definitely have probably been too hard on debtors when I encounter insane, janky code, and I realize now that that probably made me a lot less approachable, and isn't really too helpful to anyone. Empathy!

Links: 

- [Slides from this talk are here](https://techdebt.shotwell.ca/#1)

**Parallel computing with R using foreach, future, and other packages - Bryan Lewis** and **Future: Simple Async, Parallel & Distributed Processing in R - What's Next? - Henrik Bengtsson**

I really have to take advantage of `foreach` and `future` packages. I've seen them a bunch but they seem like they'd be incredibly helpful especially to help make my shiny dashboard experience a little bit better.

Also, a package called `progressr` now exists, and it sounds v cool!  

Links: 

- [progressr package github](https://github.com/HenrikBengtsson/rogressr)

**Object of type 'closure' is not subsettable - Jenny Bryan**

Jenny Bryan is my hero, seriously an inspiration to me. She's so great at helping the R community grow and be better. Her talk was engaging and her slides were great. This talk was about debugging and ways we can go about solving our problems when we are using R. Like, what is a `reprex` and what is the `browser()` function? I took a lot away from this talk, and it's stuff that I can really start using immediately in my work which is fantastic. And while the talk was about debugging she also talked about the importance of detering debugging but writing good tests and building packages. It was very inspiring to me.

I can't wait to debug now, I know that sounds a little bit strange.

Links: 

- [Talk github repo](https://github.com/jennybc/debugging#readme)

**RMarkdown Driven Development - - Emily Riederer**

I learned that RMarkdown Projects can really be thought of as packages. And that thought in itself is so revolutionary to me personally, that I just need to dive in a bit more before I can do it. But I am a lot more open to building some packages now, even if they're small and just for me and my manager.

Links: 

- [website link](https://emilyriederer.netlify.com/post/rmarkdown-driven-development/)

**One R Markdown Document, Fourteen Demos - Yihui Xie**

RMarkdown is incredible is my main takeaway. It can be used for so many things. I'm so thankful to Yihui for building such an awesome package.

My favorite thing that he showed (unfortunately I missed the first part of his talk), but it was the `Rolldown` package which looked so cool. I don't know if I have a use for this right now, but the link is here and I hope that people use this! 

Links: 

- [Rolldown](https://github.com/yihui/rolldown)

**Best practices for programming with ggplot2 -  Dewey Dunnington**

`ggplot2` can be used in packages and this can make it more obvious when you're making similar plots but just changing one variable. I learned that you can add `NULL` to a ggplot2 and there's no error and use `.data` to make it easier to programmatically call variables.

**Totally Tidy TUning Techniques - Max Kuhn**

This was a very machine learning centered talk about how to tune parameters in a model. To be honest in my experience, I've only done this kind of thing in python (where I personally think it's been easier to do stuff like this before), so seeing the R version that seems to be coming out is very exciting. The package called `tune` seems to be right in line with `recipes` and `parsnip` to really make a great and easy-to-implement modeling workflow.

Links: 

- [tidymodels tune package](https://tidymodels.github.io/tune/index.html)

**List-columns in data.table: Reducing the cognitive & computational burden of complex data - Tyson Barrett**

As someone who uses `data.table` a ton and who also enjoys the tidyverse, partly because of the functionality but also because of the community, this talk was incredibly relevant. Tyson Barrett showed really elegant ways of mixing `data,table` and tidyverse functions, like using `purrr` in list-columns of a data.table. I really want to try this out, since I've had trouble unnesting or nesting data in data.tables before.

Links: 

- [tidyfast package link](https://github.com/TysonStanley/tidyfast)

- [slides](https://tysonbarrett.com/assets/rstudio_conf_2020/Barrett_rstudioconf_2020.pdf)

**Career Advice for Data Scientists**

This was a panel and it was a nice listen towards the end of the day. Some advice was geared more towards entry level people, about their journeys into data.

I actually asked the most upvoted question on slido so that was very cool - they talked about how to approach the question of whether to give up some more technical role for more of a leadership role. While I'm still happy to be just doing technical role stuff for now, I can see myself wanting to be more of a leader in the future, and Gabriella talked a little bit about how she's approached it and how she's gotten better overall for going into a manager role. If anything, you can try it out, and go back to a technical role if it doesn't work out.

Also when talking about how to get into roles, there was very sage advice. Learn certain universal tools and brush up on math, but really you kind of have to put yourself out there, You have to apply, and you might never ever feel 'ready' for any job, but you have to apply and try. Job Descriptions are bad a lot of the times, and no human can really manage to fulfill all of the requirements anyway.

**Not So Standard Deviations with Hilary Parker and Roger Peng**

It was light hearted with talks about coffee and music, but also hit some data concepts that I've been somewhat agonizing over recently. As an analyst, what are the questions that people are trying to answer? And is giving them just a report an acceptable way to work? Hilary Parket was talking about Design Thinking and this is a subject I'm going to look more into. The only odd thing was that this was the last thing of the conference and it wasn't R or RStudio focussed, which kind of threw me off, but it was at least a fun way to end the day and I left feeling like I have to listen to this podcast a lot more.

# Wrap up

This post became VERY long but I just wanted to put all my notes out there, in case they help anyone decide what to do. 

Overall, I had a blast at RStudio conference. I had to miss parts because my phone got stolen while in San Francisco, but, what a great conference. A great environment, great talks, great networking. The night event was also a blast at the California Academy of Science - super super super cool. I'd love to come again!
