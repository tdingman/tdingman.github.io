---
layout: post
title: "SaaS vs. Tech-Enabled Services"
date: 2020-03-14
---

What changes and what stays the same when human service providers enter the mix

<!--more-->

I have spent the majority of my career in tech-enabled services. After founding [Castle](https://www.crunchbase.com/organization/castle) (tech-enabled property management), I spent time at [Atrium](https://www.crunchbase.com/organization/atrium-lts) (tech-enabled law) and [Great Jones](https://www.crunchbase.com/organization/great-jones#section-overview) (also tech-enabled property management). Now I work at [Reset Button](http://resetbutton.com) (also tech-enabled law).

Having seen enough different iterations, I know the key differences between SaaS and tech-enabled services. The following essay distills the differences and provides strategies for adapting traditional SaaS wisdom. It is the written version of a presentation I give to all new team members at Reset Button, hence the slides.

## Different Approaches, Similar Effects

<figure class="text-center">
  <img src="/img/saas-vs-tes-01.png" class="figure-img img-fluid rounded text-center" alt="Venn diagram for Saas vs tech-enabled service">
</figure>

Before we dive into any of the differences, let’s remember what SaaS and tech-enabled services share. For the user, there is ultimately no difference between the two approaches; the service does a job for the user. The differences I cover here matter to the people building the tech-enabled service, not so much the people using it.

## One Problem, Many Solutions

<figure class="text-center">
  <img src="/img/saas-vs-tes-02.png" class="figure-img img-fluid rounded text-center" alt="A single problem can have multiple solutions">
</figure>

The first major difference between SaaS and tech-enabled services is the range of solutions available. Tech-enabled services have three solution types:

<ol>
  <li><b>Process</b> - a codified series of steps</li>
  <li><b>Third-party tool</b> - software from an outside source</li>
  <li><b>First-party product</b> - software from the company</li>
</ol>

Note that any order or mixture of solution types is available: a process solution later codified into a first-party product solution, a hybrid third-party tool and first-party product solution, etc.

By contrast, the solution in SaaS is always first-party product. That’s not to say SaaS companies don’t purchase and use other software products of course, but the third-party tools are always in service to the first-party product. Not so with a tech-enabled business.

There are two consequences of having multiple solution types. First, since the right solution type is unknowable in advance, product managers must separate problem research from solution research in order to avoid being prescriptive. [Rigorous problem research](/on-problems) also clarifies the size and scope of the problem, allowing companies to prioritize problems and return to them down the road without having to rediscover everything.

Second, product managers should take advantage of the fact that not all of their solutions have to be first-party product. Specifically, process solutions are the cheapest and most flexible—often nothing more than a [checklist](https://en.wikipedia.org/wiki/The_Checklist_Manifesto)—and thus are frequently the first attempt at a solution. Third-party tools are more powerful, but more expensive and less flexible. First-party product is the most expensive, least flexible, and most powerful by far. Engineering time is precious, and tech-enabled service companies should avoid using it unless absolutely necessary to solve a problem.

## Visibility Is Limited

<figure class="text-center">
  <img src="/img/saas-vs-tes-03.png" class="figure-img img-fluid rounded text-center" alt="Emoji for see no evil">
</figure>

With software, everything is trackable: what users are doing, how the system is performing, etc.

There’s no such guarantee in a tech-enabled service business. For example, if a client came in to meet with their attorney at Atrium, there was no guarantee of a written record showing what the attorney and the client discussed. There may not even have been a written record showing that they met at all! Guarantees are impossible when dealing with humans instead of code.

In my experience, most of what happens at a tech-enabled service business is either difficult or impossible to track. Not having data makes informed decision-making and prioritization dicey. I certainly remember times at Castle where we built things off proxy data or anecdote, not because we were lazy, but because it was the best we could do.

Tech-enabled services should therefore focus primarily on the second half of Galileo's dictum: “Measure what is measurable, and <b>make measurable what is not so</b>.”

## Economic vs Temporal Efficiency

<figure class="text-center">
  <img src="/img/saas-vs-tes-04.png" class="figure-img img-fluid rounded text-center" alt="The pyramid of economic value">
</figure>

When we think about technology making things more efficient, we usually think of temporal efficiency—machines reducing the time it takes a human to do something.

What we tend to forget is economic efficiency, although a bit of reflection surfaces easy examples of such technology: division of labor, comparative advantage, firms.

Many services businesses already take advantage of economic efficiency. Oral hygienists, not dentists, clean teeth.

Tech-enabled service businesses should focus technology on unlocking further economic efficiency, rather than creating temporal efficiency, for two reasons.

First, economic efficiency is often easier to gain. What sounds easier: cutting the time it takes an attorney to complete a task in half, or enabling a paralegal who makes half the salary to do the task in the exact same time?

Second, economic efficiency moves a task one step closer to automation. The pyramid above illustrates the point. As tasks move down from the highest-skill worker to the lowest skill worker, they become simpler and more tech-enabled. By the time the task arrives at the lowest-skill worker, the jump to full automation is much smaller.

## Human Flexibility Is a Double-Edged Sword

<figure class="text-center">
  <img src="/img/saas-vs-tes-05.png" class="figure-img img-fluid rounded text-center" alt="Graph of human vs robot marginal economics">
</figure>

Software companies take a risk from day one creating something new. Many startups have died without ever finding product-market fit.

Tech-enabled service businesses by contrast start with little market risk; unless you are inventing a new type of service, you already know people want what you’re providing. Service-market fit is a given. (How product-market fit applies to a tech-enabled service business is an entire topic on its own.)

Not only that, but service providers can adapt to changing user needs faster than software. Pivots are a breeze.

Unfortunately, what tech-enabled businesses gain in starting, they lose in scaling. The fundamental difference between software and service providers is that software has zero marginal cost, whereas service providers do not. It costs Facebook ~$0 to add new users, but new clients force tech-enabled businesses to hire more service providers.

As the tech-enabled business scales, it also pays penalties of complexity. All the new service providers need onboarding, support, management, etc. The number of edges grows faster than the number of nodes in a network. Complexity is mathematically unavoidable.

The best thing a tech-enabled service business can do here is to master the arts of onboarding and change management. Every new team member needs to learn how the company operates, and every existing team member needs to understand changes to how the company operates. The company needs to guarantee everyone is rowing in the same direction.

Founders of tech-enabled service startups should also think carefully about taking significant outside capital. In order for the traditional startup tradeoff of massive upfront investment to unlock zero marginal cost to work, you have to automate away a significant amount of service provider labor. So far, that has proved difficult.

## Tension: Creative, or Destructive?
<figure class="text-center">
  <img src="/img/saas-vs-tes-06.png" class="figure-img img-fluid rounded text-center" alt="Emoji of scales">
</figure>
There will always be tension between the tech and service sides of the house.

Fundamentally, the tension comes from the different cultures.

Tech is radical. It looks at problems from first principles, comes up with novel approaches, and experiments. It moves fast and breaks things. When things break, consequences are usually small or reversible. There is a lot of room for error.

Service is (generally) conservative. It looks at problems from past history, uses known and trusted solutions, and tweaks. It moves slowly and does not break things. When things break, consequences are often substantial. There is not much room for error.

The question for tech-enabled services is, will the tension be creative or destructive?

The default is “destructive,” but each side can help make the tension creative.

Tech should focus on empathy. You don’t know what it’s like to have clients making demands day after day. It feels like there is no room to experiment when the slightest errors can catch you a lot of grief.

Service should focus on vision. Working the service day after day keeps your head down. You need to look up once in a while to see where your path is leading you.

## Summary of Solutions
<figure class="text-center">
  <img src="/img/saas-vs-tes-07.png" class="figure-img img-fluid rounded text-center" alt="Summary of solutions for tech-enabled services">
</figure>
<hr>

That’s it! If you have questions on the content, or have found something different/additional in your own tech-enabled service startup, [email me](mailto:me@timdingman.com) about it.
