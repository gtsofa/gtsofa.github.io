---
layout: post
title: "My Reflections on Design Patterns in Swift/iOS."
date: 2025-10-07
comments: true
tags: DesignPatterns, Decorator, MVC, MVVM, MVP, Singleton, Adapter
excerpt_separator: <!--more-->
---

In this article, I would like to share what I have learned about Design Patterns, what they are, why they matter, and how we can apply them as iOS Engineers.
<!--more-->

Understanding design patterns is not about memorizing definitions or fancy terminologies but instead it’s about connecting the dots between proven solutions and the real problems we face in our day-to-day work. As an engineer, when you understand how to use them effectively, you save time, avoid reinventing the wheel, and deliver cleaner, more maintainable code.

## Why Design Patterns Matter
Design patterns provide a shared language for developers. They help us describe problems and solutions clearly and avoid miscommunication. For example, when I tell a teammate, “Let’s use the Decorator pattern here,” I am communicating more than an idea and expressing intent. My colleague instantly knows that I plan to extend a component’s behavior **without changing its core logic**.

And even if they don’t recall every detail, they can always refer back to the Gang of Four (GoF) book or other resources. That’s the beauty of having a common design vocabulary. It helps teams collaborate smoothly and consistently.

Beyond communication, design patterns also provide proven solutions to recurring problems. They represent years of collective experience from developers who have solved similar challenges before us. Instead of starting from scratch each time, we can stand on their shoulders and apply time-tested approaches.

Finally, design patterns help us **compose our systems with good abstractions**. For instance, in iOS architecture, we can use design patterns to organize our composition root, manage dependencies, and keep modules decoupled. This leads to flexible, maintainable, and testable codebases, a good trait that every developer strives for.

## How to Use Design Patterns
You do not need to memorize every design pattern by heart. What matters is familiarity, knowing they exist and being able to recognize when to apply one. When you face a problem that needs an elegant solution, scan through the Design Patterns book and pick one that fits the problem you're trying to solve.

To be honest, the Gang of Four book can be intimidating, especially if you’re just starting out as an engineer. I feel like it was written with an advanced audience in mind. For me, the real “aha” moment came when I joined the [iOS Lead Essentials](https://www.essentialdeveloper.com/) program, where I saw concrete, practical examples of how these patterns solve real-world iOS problems.

Here are some patterns I’ve personally found useful in Swift/iOS projects:

- **Strategy Pattern**: Encapsulates decision-making logic. For example, instead of cluttering a view controller with `if-else` or `switch` conditions to decide between fetching data from different sources, I can create a strategy type to encapsulate that algorithm. This keeps my code testable, extendable, and easier to reason about.

- **Adapter Pattern**: Bridges mismatched interfaces. For example, if a service returns a dictionary of resources but a view controller expects an array, an adapter helps translate between the two without modifying either side.

## Key Takeaways
- **You don’t need to memorize all patterns**. Just be familiar with them. When a challenge arises, look up the right pattern and apply it.

- **Patterns are about communication and maintainability**. They make your codebase clear, testable, and adaptable, and not unnecessarily complex.

- **Common Swift design patterns include**: a) **Structural design patterns** like Decorator, Adapter, and Composite or Architectural patterns like MVC, MVVM, and MVP. b) **Creational patterns** like Builder, Factory Method, and Singleton, which focus on how objects are created.

## Summary
Design patterns are not about forcing a structure into your project but instead about recognizing recurring problems and applying proven, shared solutions. Think of them as tools in your engineering toolbox. The real skill lies in knowing **when**, **and when not**, **to use them**.

That’s my ongoing journey with design patterns, and I’d love to hear from others: Do you actively use design patterns in your projects, or do you let them emerge naturally over time?

