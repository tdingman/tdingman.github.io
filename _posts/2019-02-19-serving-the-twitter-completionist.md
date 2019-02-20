---
layout: post
title: "Serving the Twitter Completionist"
date: 2019-02-19
---

Making the Sisyphean more pleasant

<!--more-->

I read Twitter daily. On a fairly busy day, I read once in the morning when I wake up and once at night as I ready myself for bed. On a slow day, I may check my timeline five or ten times.

For me, Twitter is the news; I mostly follow outlets like Ars Technica, Vice, and Nautilus, and the people I do follow tweet only occasionally. I stay away from low signal-to-noise accounts and almost never use Twitter for social purposes. It's like a RSS feed, but 10x better.

Because the people I follow tweet infrequently, I am a Twitter completionist - I read every tweet in my timeline. If I don't read them all, I may miss content from the people I follow, and then I get #fomo like a good Millenial.

"Completionist" is an established user persona in gaming. Have you ever played a video game that shows the percent of achievements unlocked and wondered who in their right mind would waste all that time getting to 100%? Completionists, that's who.

<figure class="text-center">
  <img src="/img/completionist.jpg" class="figure-img img-fluid rounded text-center" alt="@JKCompletesIt on Twitter">
  <figcaption class="figure-caption">There's even <a href="https://twitter.com/JKCompletesIt">someone on Twitter calling himself The Completionist</a></figcaption>
</figure>

Unfortunately, publishers have a nasty habit of tweeting the same story multiple times, albeit with different copy in the tweet. I assume they're designing for the average, non-completionist Twitter user, who may miss a story entirely if the publisher doesn't tweet it several times over the course of a few days. For completionists like me, though, tweeting the same story over and over again adds unwelcome noise and wastes my time.

Now, I'm sure Twitter would respond by directing me to the algorithmic timeline. They've been pushing it a lot recently, going so far as to make it the default view in their app. (I'm sure they're taking a page from Instagram's book here.) I turned it off immediately; I don't trust the algorithm, and a non-chronological timeline only makes life harder for a completionist like me. How would I know where I last left off?

The Economist has a neat solution here: follow normal publisher best practice and tweet a story multiple times with @TheEconomist, but offer users like me a different account to follow - @EconomistOnce - that only tweets stories once.

<figure class="text-center">
  <img src="/img/economistonce.png" class="figure-img img-fluid rounded text-center" style="max-width: 480px;" alt="@EconomistOnce on Twitter">
  <figcaption class="figure-caption"><a href="https://twitter.com/EconomistOnce">Sweet, sweet relief</a></figcaption>
</figure>

I remember how elated I was to see a publisher meeting my needs as a completionist. Since then, I have waited for other publishers to follow suit, but none have. Why should they? @EconomistOnce is a courtesy to readers like me that provides no benefit to The Economist; completionists are going to read the story whether they see the tweet once or a hundred times.

However, Twitter itself has an opportunity here to better serve some of its biggest users, possibly while increasing revenue at the same time.

## The Deduped Timeline

The problem is simple: multiple tweets from the same account to the same piece of content reducing the signal-to-noise ratio of the timeline. The solution is also straightforward: condense those tweets down to one, and suddenly your timeline becomes more manageable.

Facebook already does something similar. If your friend posts something, then five of your mutual friends share it, you don't see six copies of the same post - you see a parent post and child shares. The sharing is still there, but the effect is concentrated on the news feed.

Implementing shouldn't be tough either. Twitter already inserts its own link shortener, t.co, betwen links you see on Twitter and the actual page you're navigating to. That means they already know what content publishers are posting. The visual design could be tricky, but the basics are all there.

It's a fine solution for completionist users like me, but I think Twitter also benefits here. I'll use some made-up numbers about my timeline to illustrate my point.

Let's say the tweets I see in a normal day break down into the following categories:

* Stories from publishers: 90%
* Unique content from actual people: 7%
* Ads: 3%

My gut says a publisher tweets at least three times in one day about a story. In other words, that 90% is two-thirds duplicate content. If we dedupe my timeline, the breakdown becomes:

* Stories from publishers: 75%
* Unique content from actual people: 17.5%
* Ads: 7.5%

Just like that, we've more than doubled the amount of ads completionists will see! Not only that, they're more likely to spend more time viewing an ad, since they're not quickly scrolling through a sea of duplicate content.

## Validation and Implementation

If I were a PM at Twitter, here is how I would validate my hypothesis and implement the feature:

1. Verify the existence of the completionist user persona via surveys and interviews
1. Verify the pain of duplicate content, also via surveys and interviews
1. Model out numbers (as I did above) showing the current state of affairs for completionists vs what things would be like with the deduped timeline
1. Use the model to estimate the business impact, probably some increase in ad revenue
1. Estimate a cost to develop the feature using man-hours based on rough user story points
1. Determine a ROI from the preceding two steps
1. If the numbers work out, design/test/build
1. A/B test to determine impact and validate the financial model

If anyone from Twitter is reading this, get at me - I would love to see this feature happen!
