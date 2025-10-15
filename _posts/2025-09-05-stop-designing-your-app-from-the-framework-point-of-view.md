---
layout: post
title: "Stop Designing Your App From the Framework Point of View"
date: 2025-09-05
comments: true
tags: Design, 3rdPartyFramework
excerpt_separator: <!--more-->
---

One of the most common struggles developers (new comers or even experienced) face is choosing the “right” tools and frameworks at the start of a project.
<!--more-->

Should I use Alamofire, Moya, URLSession, Realm, Core Data… or something else?

![3rd-party framework](/assets/img/images-frameworks/third-party-frameworks.png "Third Party Frameworks")

What if I make the wrong decision and get stuck later?

Which Cocoapods should I bring in from day one?

As you can see it’s easy to feel paralyzed by these questions. And it’s tempting to start with frameworks because they seem like shortcuts that will help you deliver faster.

But here’s the truth I’ve learned the hard and painful way: 

- Starting from frameworks often slows you down.

## Why is that?
- You get stuck in decision paralysis.

- Frameworks rarely fit exactly what you need.

- Codebases end up bloated with unused dependencies.

- You risk locking yourself in: building your whole app around Core Data, UIKit, or another framework makes it painful to adopt better alternatives later.

From my experience, I have seen teams forced to rewrite entire apps just to move from UIKit → SwiftUI or from Core Data → SwiftData, because the original design was tightly coupled to the framework. That’s expensive, frustrating, and risky for the business.

## So what should you do instead?
Here let's invert the dependency. Design your app from the **user and business point of view and plug in the frameworks to obey your user or business requirements**.

Think of frameworks as details, not the foundation of your application.

- Start from features, use cases, and models.

- Keep your core logic decoupled from frameworks using abstractions.

- Plug frameworks (Moya, Alamofire, Core Data, URLSession, SwiftData, etc.) in later when you truly need them.

This will help you a lot. For example:

- You can build and test a UI without a backend by simulating data in memory.

- You can develop features without a database and plug in persistence later when it's ready.

- You can deliver something to stakeholders quickly, gather feedback, and keep on iterating, instead of waiting on infra teams or locked-in dependencies.

This approach keeps you in control and flexible:

- Swap or plug and play frameworks with minimal cost and pain when new, better tools arrive.

- Stay aligned with software's changing nature all the time example the Apple’s yearly iOS updates..

- Keep delivering value continuously, even when infra isn’t ready yet.

So, I recommend, you keep it simple and bring infrastructure complexity only when it's really need. You can do this by learning to design your apps in a way that is decoupled from frameworks. 

💡 **Takeaway**: Start with **business requirements**, **not frameworks**. Frameworks should serve your design, not dictate it.

There are techniques like the inside-out and outside-in approaches that can help you as well. This is something I learned from the [Essential Developer Academy](https://www.essentialdeveloper.com/) which changed my life :-) I will share more about those in my next post. Stay tuned!


