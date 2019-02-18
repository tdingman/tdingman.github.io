---
layout: post
title: "Roche: From Nil to MVP"
date: 2019-02-06
---

Explain game + place in Brown ultimate community

Explain self-PM

Steps: user research, MVP, PVD, user stories, point, sprint
  Much messier than that

Learn Django

Lessons about user research:
	let them talk/don't summarize
	go off script, it's not a survey
	look for feelings

Lessons from user research:
	Mundane vs daring roches
	Goldilocks zone for good roches
	Odds
	Peer pressure
	Producing something from nothing
	Warm fuzzies from memories of great roches

Would have pivoted to Odds for a real product

Link to PVD: https://docs.google.com/document/d/1KCPcIaPg9cG9SYVcfsVISdsw6-eUMbDgvX_tfMiRnqg/edit?usp=sharing

MVP board

A last-minute bug!

Should have done TDD

Close with hopes for emotional attachment

===

Ultimate frisbee was a big part of my experience at Brown. It gave me a cultural home on campus, a welcome counterbalance to the stress of engineering coursework, and a network of friends I maintain to this day.

One essential piece of culture in the Brown Ultimate community is roching. For the uninitiated, roching combines rocks-paper-scissors with dares. (The name "roche" is short for [roshambo, an alternate name for rocks-paper-scissors](http://mentalfloss.com/article/80201/why-do-people-call-rock-paper-scissors-roshambo).) Here's how a roche typically works:

1. Someone in a group proposes a roche, ex. "Roche wear sunglasses for 24 hours." (Note: wearing sunglasses for 24 hours is harder than it sounds!)
1. The person proposing the roche specifies a number of wins or losses required to decide the performer. The default is one loss, i.e. the ultimate loser in the group has to do the dare.
1. After there are enough participants - at least two, oftentimes more - the first round of rocks-paper-scissors begins
1. The group plays rounds of rocks-paper-scissors until someone hits the specified number of wins or losses
1. The ultimate loser/winner performs the dare, much to the enjoyment of everyone around

People familiar with [Odds](https://what-are-the-odds.info) will recognize some similarities.

Roching is a mainstay of nearly every gathering of Brown Ultimate players, and anyone who has played at least one seasons can conjure up memories of favorite roches. In my research, I talked to alumni who graduated up to fifteen years ago, and all of them regaled me with at least one such tale. More about that in a minute.

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

I'm a big believer in buying before building. Back in my Castle days, we often deployed "Ops solutions" before "Dev solutions," i.e. wrote a process or found a third-party tool to do a job before coding a tool ourselves. I often think back on a PM colleague from Atrium deciding to ship a custom Airtable setup as a product instead of deploying engineers to build one. It's fun and exciting to start building your own tool, but often you run into edge cases that the producers of similar third-party tools encountered and solved ages ago. Also, [comparative advantage[(https://en.wikipedia.org/wiki/Comparative_advantage).

I took a crack at a MVP using Airtable, but quickly ran into features I absolutely needed that Airtable wouldn't support. The hardest part would have been the logic of the game - taking all the players' throws and deciding who was the winner/loser. However, the exercise of attempting the MVP with Airtable was still valuable; it uncovered edge cases I may not have considered until I was knee-deep in code, well beyond the design stage where it's easy to make revisions.

Looking back, I could have done the whole thing in Google Sheets, which is easy to extend with Google App Script, but part of my goal was to learn some Django and PM myself like I would an engineer. If I were PMing for real, I would have given Google Sheets + Google App Script a serious go.

## PVD
