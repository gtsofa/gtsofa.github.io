---
layout: post
title: "Inside-Out vs Outside-In Development Approaches"
date: 2025-09-13
comments: true
tags: InsideOut, OutsideIn
excerpt_separator: <!--more-->
---

In my previous article, I talked about the struggles developers often face at the start of a project. I also promised to share two techniques that can help us avoid getting stuck and keep delivering value. 
<!--more-->
Today, let’s explore the Inside-Out and Outside-In design approaches.

At the end of the day, software development is about delivering value to customers and businesses. That’s what pays our bills and keeps products alive. The challenge is that we often build under conditions of uncertainty, so we need approaches that help us stay productive even when all the pieces aren’t ready.

## Why This Matters in Real Projects
Again in my experience, I have seen in cross-functional teams such as mobile, web, backend, or design, it's common to see progress often depends on other resources such:

- The design team may still be polishing final mockups.

- The backend team may still be finalizing endpoints.

- The product team may still be debating business rules.

Rather than waiting and getting blocked, we can use the Inside-Out or Outside-In approaches to keep us moving. Let's see what they mean.

## Inside-Out Design
With this approach, you start from the **core logic** or **domain models**. Make sure you sit down with the backend and agree on a contract between the client and backend API. As long as you have this contract you can go ahead and start test driving things.

Example: If you know your app needs to load image data but you don’t yet have the UI, go ahead and build the logic. Write unit tests for your domain and verify how your model behaves.

When to use this:

- No UI designs or backend yet.

- Building with long-term maintainability and testability in mind.

## Outside-In Design
Here, you begin with the UI and user flows. You also need to sit down with the design team and come up with some contracts as well in the form of sketches or mockups. This will help you create the correct designs not something off from what the designers have.

Example: If you already have design sketches or Figma screen mockups, build the UI and plug in mocks until the backend is ready. Test drive how your view responds to user interactions like button taps and gestures.

When to use this:

- You have full UI designs.

- Need clickable prototypes quickly for fast feedback.

- Exploring user experience first.

## Why TDD Helps
Many developers pause when they don’t have an API or a dependency ready. That pause wastes valuable time.

This is where I find Test-Driven Development (TDD) powerful. It acts like a compass, giving me feedback on my design and helping me move forward. Whether I start inside-out or outside-in, I’m not blocked. I’m always making progress and delivering value to my customers several times a day.

So, if you’re stuck, at least remember this: Don’t stop. Stub it. Spy it. Mock it. Abstract it. Keep going.

You can switch approaches as needed or sometimes even mix them. The key here is progress.

What do you think about these approaches? Have you tried switching between them in your projects?

I’d love to hear your thoughts in the comments.





