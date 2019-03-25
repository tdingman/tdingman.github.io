---
layout: post
title: "Tech-Enabled Service Startup Lessons from The Goal"
date: 2019-03-24
---

Efficientia delenda est

<!--more-->

_The Goal_ is the most enthralling book you'll ever read about the life of a factory manager. It is probably also the only book you'll ever read about the life of a factory manager.

_The Goal_ describes the trials and transformation of a struggling factory (or "plant" as the narrator calls it) in a struggling manufacturing division of a generic conglomerate, UniCo. The plant manager, Alex, revolutionizes how his plant functions after a chance encounter with his old physics professor, Jonah. Sure, the plot is thin at points, and the B plot about Alex's marital issues is trite and bland, but the story is shockingly gripping given its subject matter.

You see, The Goal is not fiction for fiction's sake; it is a sugary coating of fiction over the bitter pill of process improvement frameworks.

And what a curative pill it is! The Goal was an absolute revelation to me. For anyone working on a startup that uses humans + technology to deliver a service, the lessons of The Goal could be your salvation. As a former founder of [one such company](https://techcrunch.com/2016/02/29/castle-is-a-property-management-platform-from-the-future/) and a former employee of [another](https://www.atrium.co/), here's what I learned:

## 1. Throughput, Inventory, Operational Expense

The author's first major claim is that any production system has three financial metrics: throughput, inventory, and operational expense. All other financial metrics roll up into one of the three. (OK, technically his first major claim is that the titular goal of a plant is to make money, but I didn't find that one especially insightful.)

Jonah, the author's mouthpiece in the book, defines each term precisely:

* Throughput: the rate at which the system generates money through sales
* Inventory: all the money the system has invested in purchasing things which it intends to sell
* Operational Expense: all the money the system spends in order to turn inventory into throughput

The job of the production system's manager - here, our plant manager Alex - is to increase throughput while decreasing inventory and operational expense. It's a simple framework, but Alex's story shows over and over how he can make difficult decisions by breaking complex issues down into their impact on the three core metrics.

Your production system of tech-enabled service providers is no different. Throughput and operational expense translate directly. Inventory requires a little imagination; where Alex deals with half-finished parts, a service business deals with half-finished client work.

Apply the framework of the three core metrics to your team properly, and the complex will become straightforward.

## 2. In Praise of Idleness

After establishing the three core metrics, the author spends the next quarter of the book discussing bottlenecks, which he develops with corollaries for basically the rest of the book.

It's worth reading the hike scene in _The Goal_ in full to gain an intuitive understanding of bottlenecks and their consequences. The scene is too involved for me to rehash here. For now, take the following points as given:

* A bottleneck is the stage in a system with the lowest capacity
* Every system has a bottleneck

We can immediately combine the two premises to create a corollary: the system capacity is the bottleneck capacity. Even if other stages in the system produced faster, the system overall would not produce faster. Therefore, the capacity of non-bottlenecks is irrelevant above the threshold of bottleneck capacity. 

Alex has a lot of trouble with Jonah's conclusion here. Intuitively, shouldn't each stage be producing at its capacity? Isn't that more efficient? He can't have workers on non-bottlenecks just sitting idle, it looks bad!

Jonah categorically rejects Alex's notions of efficiency. There is no point in production above bottleneck capacity, since it will not increase throughput. In fact, the system would then gain inventory - the opposite of what we want based on the three core metrics! (Using excess capacity has little or no impact on operational expense. You're paying your workers whether they're working or idle, assuming they're salaried.)

Again, your production system is no different. Somewhere in your team is a bottleneck. Your job is to identify it, focus on increasing its capacity (probably by building product for it!), and optimize every stage in the system for it. Let your non-bottlenecks be idle when there is no work to due on account of the bottleneck. Even if throughput stays flat, your inventory will go down, and you'll probably decrease burnout by allowing your team to be idle sometimes.

## 3. Lead Time Is Queue Time

In a scholarly appendix to the narrative of The Goal, the author mentions a fact I found shocking: in manufacturing, 90% of lead time is queue time. Only 10% is production time, i.e. time when a system is somehow altering the thing being produced. The reason? Most manufacturing operations shoot for "efficiency" like Alex, and thus have high inventory, which creates long lead times.

Upon reflection, I realized the same ratio applied to client work in my experience at tech-enabled service startups. In fact, the ratio I've seen is probably more like 95% to 5%. With all the service providers at capacity in order to be "efficient," new incoming work enters a long queue. Inventory is high, so lead times are high.

The solution is to minimize batch size, i.e. the amount of stuff your team is working on at a time. It's just the reverse of the problem; if working on lots of stuff creates long lead times, working on a little stuff creates short lead times. If you want your service providers to complete client work faster, reduce the number of client projects they have open at the same time.

## 4. The Context Problem

Alex initially pushes back on Jonah's recommendation to cut batch sizes because smaller batches means more setup time per part, which is "inefficient." Jonah shows how the overall tradeoff is worth it, but does acknowledge that minimizing setup time is a good use of resources. The author echoes the same idea when discussing Hitachi's production methods in the scholarly appendix.

The equivalent of setup time for humans is task switching, a term I first learned in [this essay](https://www.joelonsoftware.com/2001/02/12/human-task-switches-considered-harmful/). Humans need time to reorient when changing from one task to another. If we try to multitask or work on many projects in parallel (which we know from above is bad!), switching costs eat us alive.

In my experience at tech-enabled service startups, we faced a bigger, more specific issue: the context problem. When switching from one client project to another, there is the task switching cost of refocusing your attention, _plus_ the much thornier task of gaining context on the new client project. It's hard to learn all the relevant information about a client in a short amount of time, and it's even harder to capture all the relevant information in the first place!

For any relationship-based tech-enabled service startup - which I suspect is most of them - solving the context problem is absolutely essential once more than one person starts working on any one client project. If you can't reduce setup time, you'll have a high floor on your queue times, which will limit throughput and keep inventory high. (You'll probably also make mistakes due to internal miscommunications or dropped balls - issues machines in a plant don't have.)

Overall, I would recommend _The Goal_ to anyone in operations, and would call it essential for product and operations people working on tech-enabled service startups. If you want to discuss takeaways more, hit me up - [you know where to find me](timdingman.com).
