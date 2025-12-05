---
layout: essay
type: essay
title: "Painting a Framework"
# All dates must be YYYY-MM-DD format!
date: 2025-12-04
published: true
labels:
  - Software Engineering
  - RateMyTools
---

<img width="300px" class="rounded float-start pe-4" src="../img/B_RATEMY.svg">

## Introduction

Design patterns are like paintings. You imagine your software in your head, perfectly planned, neatly segmented, and composed of parts that just make sense. In your mind, it is the modern software Mona Lisa. But once the brush swipes the canvas, everything slips: the proportions are wrong, the colors clash, and the canvas itself turns out unprepared. The painting collapses into something fragile and inconsistent. In this metaphor, the canvas represents the architectural logic behind software and how pages, components, and backend functions actually connect and interact with each other. Without structure, even the most creative ideas fall apart.

Enter attempt number two. Instead of freehanding the entire piece, you rely on established methods, techniques that help maintain proper proportions, guide your color choices, and ensure the canvas is properly primed. Although still not quite what was envisioned, it is functional, organized, and designed with intent.

This mirrors the role of design patterns and how they shaped my final project, RateMyTools, a student-driven platform for discovering and reviewing learning tools. What began as a simple framework evolved into a complex, interconnected system built through patterns I had not anticipated at first but came to understand as essential.

---

## Design Patterns

Design patterns in software engineering function much like the techniques painters rely on to bring structure to their artwork. While the viewer may only notice the final image, an artist understands the composition, layering, and brushwork that holds the painting together. In the same way, design patterns are not simply lines of code but guiding approaches that solve recurring problems. For example, using a Singleton to control access to a resource or a Factory to create objects without over-specifying their type. These patterns give shape to the software beneath the surface, and with them in place, a codebase becomes cohesive and stable, ensuring that its structure remains intact as the project grows more complex.

---

## Making RateMyTools

Designing RateMyTools felt similar to envisioning a painting and then actually trying to bring it to life. At first, my team and I prepared the canvas by planning our timeline, setting up the basic structure of the project, and organizing the React components. But as the painting became more detailed, we realized that the tasks we assumed were simple were far more complex. This is where design patterns emerged. The contrast between database models, UI components, and server logic mirrored the layered planning painters use to maintain structure in their work.

React’s state system acted like controlled brushstrokes that allowed small changes, such as typing in a search bar or submitting a review, to blend into the final composition. Our Neon database served as the foundation for every layer we added, and Prisma became the tool we used to paint the surface by defining models, relationships, and tables that kept our data organized.

---

## Patterns in RateMyTools

As RateMyTools took shape, our project began adopting many design patterns. Whenever new users, reviews, or tools were added, Prisma handled the creation process like a Factory that produces consistent objects. React’s ability to refresh components automatically when state or session data changed reflected the behavior of the Observer Pattern, keeping the interface responsive and in sync.

We also depended on a single shared Prisma client, an example of the Singleton Pattern that prevented unnecessary database connections. Prisma’s abstraction of queries resembled the Repository Pattern, and our authentication logic followed the Strategy Pattern by choosing different flows depending on the user. Together, these patterns kept the codebase organized, predictable, and easy to evolve.

---

## Conclusion

In the end, building RateMyTools taught me that software engineering is less about improvising on a blank canvas and more about understanding the techniques that allow a vision to take form. Just as a painter relies on composition, layering, and foundational structure to keep a piece from collapsing, developers rely on design patterns to keep their systems structured as they evolve.

The patterns that emerged throughout our project, such as Factories, Observers, Singletons, Repositories, and Strategies, were tools that shaped how our application behaved and grew. They helped transform isolated features into a unified system, allowing each part of the app to interact in sync. RateMyTools demonstrated how thoughtful architecture can turn a rough sketch into a functioning work of software.
