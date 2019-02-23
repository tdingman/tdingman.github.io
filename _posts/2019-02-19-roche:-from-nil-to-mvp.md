---
layout: post
title: "Roche: From Nil to MVP"
date: 2019-02-19
---
An exercise in autodidacticism and self-PM'ing

<!--more-->

Ultimate frisbee was a big part of my experience at Brown. It gave me a cultural home on campus, a welcome counterbalance to the stress of engineering coursework, and a network of friends I maintain to this day.

One essential piece of culture in the Brown Ultimate community is roching. For the uninitiated, roching combines rocks-paper-scissors with dares. (The name "roche" is short for [roshambo, an alternate name for rocks-paper-scissors](http://mentalfloss.com/article/80201/why-do-people-call-rock-paper-scissors-roshambo).) Here's how a roche typically works:

1. Someone in a group proposes a roche, ex. "Roche wear sunglasses for 24 hours." (Note: wearing sunglasses for 24 hours is harder than it sounds!)
1. The person proposing the roche specifies a number of wins or losses required to decide the performer. The default is one loss, i.e. the ultimate loser in the group has to do the dare.
1. After there are enough participants - at least two, oftentimes more - the first round of rocks-paper-scissors begins
1. The group plays rounds of rocks-paper-scissors until someone hits the specified number of wins or losses
1. The ultimate loser/winner performs the dare, much to the enjoyment of everyone around

People familiar with [Odds](https://what-are-the-odds.info) will recognize some similarities.

Roching is a mainstay of nearly every gathering of Brown Ultimate players, and anyone who has played at least one seasons can conjure up memories of favorite roches. In my research, I talked to alumni who graduated up to fifteen years ago, and all of them regaled me with at least one such tale. More about that in a minute.
<figure class="text-center">
  <blockquote class="twitter-tweet text-center" data-lang="en"><p lang="en" dir="ltr">Roche crab walk <a href="https://t.co/zWZM72p9Do">pic.twitter.com/zWZM72p9Do</a></p>&mdash; Senior Week 2011 (@ultimateseniors) <a href="https://twitter.com/ultimateseniors/status/736990491800129537?ref_src=twsrc%5Etfw">May 29, 2016</a></blockquote>
  <figcaption class="figure-caption">The author losing a crabwalk race as a result of a roche</figcaption>
  <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
</figure>

After I graduated in 2012, there was a lot less roching in my life. Sure, my friends from Brown Ultimate would roche with me at our various reunions over the years, but it wasn't part of my life like it once was. Turns out, it's hard to roche long-distance. As with relationships though, I think technology can help close the gap.

## The Self-PM Process
From the outset, I wanted to treat my side project like a real product. As a team of one, I would be product managing myself. Here was my plan:

1. Do user research on Brown Ultimate alumni to validate the need
1. Build a minimum viable product (MVP) from third-party tools to rapidly test my assumptions and ideas
1. Write a product vision document describing the tool I wanted to build
1. Write user stories representing all the functionality for the MVP of the tool I wanted to build
1. Point the user stories
1. Code the user stories in fortnightly sprints

As you'll see, I deviated in some places but generally stuck to the plan.

## User Research

The goal of user research is to validate hypotheses. Sometimes, you start from a place of general understanding and can use tailored questions to address specific ideas. Other times, you have no idea where to begin and prepare a loose set of questions to start a conversation that ends up guiding itself. Since I have years of first-hand knowledge of roching, I took the former approach.

I started by writing out a list of questions to ask during my interviews. I wanted to understand a few key things about my interview subjects:

* Their history with roching
* Their feelings about roching
* Their needs and wants regarding roching

My hypothesis, which I hoped to prove using the information I gathered, was that there exists a class of "power users" who still have a deep attachment to the game and would roche more if given the opportunity.

I ended up doing nine phone interviews with Brown Ultimate alumni who graduated within the last fifteen years, each about thirty minutes long. You can see the full, anonymized notes - plus my script and summary of results - [here](https://docs.google.com/document/d/1O0J4Js_HD1V0fi6NRY7iLn8jy3McN9LOEaa2D6ILANk/edit).

My research generally validated my hypothesis and allowed me to move on to the next step. One unexpected finding: Odds has become widespread at colleges and in social circles of new graduates across the country. If I were building a product purely to serve a market with an interest in a roche-like game, I would probably have pivoted to building an Odds web app instead of a roching web app. Since the project is partly a learning experience and partly a labor of love, not just about solving a problem for a set of users, I decided to forge ahead with roching.

## MVP

I'm a big believer in buying before building. Back in my [Castle](https://techcrunch.com/2016/02/29/castle-is-a-property-management-platform-from-the-future/) days, we often deployed "Ops solutions" before "Dev solutions," i.e. wrote a process or found a third-party tool to do a job before coding a tool ourselves. I often think back on a PM colleague from Atrium deciding to ship a custom Airtable setup as a product instead of deploying engineers to build one. It's fun and exciting to start building your own tool, but often you run into edge cases that the producers of similar third-party tools encountered and solved ages ago. Also, [comparative advantage](https://en.wikipedia.org/wiki/Comparative_advantage).

I took a crack at a MVP using Airtable, but quickly ran into features I absolutely needed that Airtable wouldn't support. The hardest part would have been the logic of the game - taking all the players' throws and deciding who was the winner/loser. However, the exercise of attempting the MVP with Airtable was still valuable; it uncovered edge cases I may not have considered until I was knee-deep in code, well beyond the design stage where it's easy to make revisions.

The biggest way my spreadsheet MVP saved me time was in database design. The first time I created tables to reflect my data model, I immediately uncovered several holes in my design. Once I actually started coding later on, I repeatedly recognized places where I would have wasted hours had I not tested my schema in spreadsheets.

Looking back, I could have done the whole thing in Google Sheets, which is easy to extend with Google App Script, but part of my goal was to learn some Django and PM myself like I would an engineer. If I were PMing for real, I would have given Google Sheets + Google App Script a serious go.

## PVD

A product vision document answers three questions about the product:

1. What is it?
2. Why are we doing it?
3. What does success look like?

A good PVD allows someone with little or no context to understand a problem and the proposed solution from 10,000 feet in the space of a page or two. In a real company, I would have circulated the PVD and asked for input from other stakeholders, but there's not much of that in a team of one!

After so much research and iterating, the What and the Why are usually easy to answer, although often need paring down to their essentials. However, the success criteria can still be difficult. I have a lot of experience setting OKRs, which are similar, but I still struggled with the success metrics. Check out the full PVD [here](https://docs.google.com/document/d/1KCPcIaPg9cG9SYVcfsVISdsw6-eUMbDgvX_tfMiRnqg/edit?usp=sharing).

## Intermission: Learning Django

Normally in the product development process, we'd move on to writing user stories and speccing them for development.

However, since I was the only engineer on the project, I had to first learn how to build a web app at all before I could move on to building the web app I wanted.

I was familiar with Node + Angular from Castle, but I always liked Python better than JavaScript, so I settled on Django as my framework. I went through the official [Django tutorial](https://www.djangoproject.com/start/) and the [Mozilla Developer Network tutorial](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django), taking notes as I came across functionality I knew I would need for my MVP. I threw in a tiny bit of Bootstrap for my frontend as well.

## Infrastructure and User Stories

Once I knew what I wanted to build, I started a [GitHub repo](https://github.com/tdingman/roche) and filed [issues](https://github.com/tdingman/roche/projects/2) for all the infrastructure it would require to be minimally functional ([example](https://github.com/tdingman/roche/issues/5)). For the other features I wanted, I filed issues as user stories.

For the uninitiated, user stories are feature ideas written in the following form:

> As a [type of user], I want [feature] so that I can [goal]

I have a soft spot in my heart for user stories from my days at Castle. I admire how such a simple trick of phraseology can clarify thinking, screen ideas, and communicate clearly what the story writer was thinking. Before we implemented user stories, people would submit ideas for features that weren't fleshed out or didn't have a clear purpose. After we implemented user stories, the reasons we should implement features became apparent at a glance.

Once you have a user story, you assign it a point value that represents the amount of work the user story will take to complete. Each "step" the user story takes to implement is one point. You're not writing code at this stage, but you're close - it's almost like pseudocode in some cases. A well-pointed user story makes coding a breeze; you've done all the thinking up front, so you don't get hung up halfway through writing a tricky method.

I deviated from best practice here by not writing all my infrastrucutre issues as user stories. However, I did point all of the issues, which helped me estimate the amount of work and forced me to confront further edge cases I had not caught in my initial design or in my third-party MVP.

## Coding
Having spent the better part of a month on research and prep, I finally started coding. I set up a two-week sprint with all the pointed issues, assigned myself to the issues, and got to work.

Much to my delight, Django and all my preparation made most of the coding a breeze. The tutorials had prepared me well, and I had most of a web app running in only a few days. (Keep in mind I was working normal hours at my day job.)

About three quarters of the way through my user story points, though, I ran into further complexities I hadn't accounted for. Instead of switching from coding back to pointing, though, I hacked my way through, writing and deleting various versions of solutions in about equal measure. After muddling my way through to the finish line, two notions struck me:

1. This is why so many software projects blow their deadlines
1. I should have used TDD (test-driven development)

## QA
When I read about TDD in the Django tutorial, I thought it was good best practice but not necessary for a team of one. After all, I should be able to keep the whole codebase in my head; why spend all that time writing out tests?

Turns out, I couldn't keep the whole codebase in my head. I realized after only a little bit of testing that I had [forgotten to implement half of a core feature](https://github.com/tdingman/roche/issues/18)! The app allowed the creator of a roche to specify a number of wins/losses to complete the roche, but all my logic assumed that number was always one.

I patched the bug, ruminated on my shortcomings, then put a fork in it - the MVP was done.

## What's Next
Now that the MVP exists and has no known bugs, it's time to recruit beta testers. You'll be able to read all about it (and get a link to the beta-tested version) in my next post. Until then, happy roching!
