---
layout: post
title: Thoughts on Philosophy of Software Design
categories: learning-reflections
tags: []
date: 2026-01-12 05:09 +1100
---
Here are my thoughts and reflections on software design philosophy resources I've explored.

*Note: The thoughts and ideas expressed below are my own. The language has been polished with assistance from Claude.*

---

## Philosophy of Software Design

### [Article: Book Review - Philosophy of Software Design](https://han4wluc.com/blog/2025/01-book-review-philosophy-of-software-design/)

### [Video: A Philosophy of Software Design by John Ousterhout](https://www.youtube.com/watch?v=lz451zUlF-k)

### Book: A Philosophy of Software Design

#### My Thoughts:
This is a really inspiring book. When I read it, real cases that happened to me popped up in my mind. Here are some current thoughts I have after relating to my personal experiences:

- **Do not be a tactical tornado.** I implemented a task website early on. At that time, I just wanted the website to work, completely disregarding coding styles and design problems. The result was messy code — for example, I scattered side effects throughout the codebase instead of isolating them in a dedicated file, breaking the principle that all other functions should be pure. This led to more refactoring afterwards — exactly "borrowing time from the future".

- **Do not over-engineer either.** I learned about different design patterns and software architectures in one of my courses. Some of them, such as microservices or event-driven architecture, offer benefits like scalability and flexibility, but they also introduce trade-offs: network latency, distributed system complexity, and higher operational overhead. For startups, adopting these prematurely can be disastrous — that is over-engineering. The same principle applies at the code level: simple implementation designs should also evolve gradually rather than being over-planned upfront. Now when coding, I am still finding a balance between planning ahead and being tactical. The author suggests this balance comes from experience, so finding my own requires practice.

- **The worst is the unknown unknown.** There was a bug where some animations didn't show as expected. I spent hours debugging, assuming it was an update problem. Eventually I found that we were trying to sort a readonly field, which led to undefined behavior. The readonly constraint was not enforced at runtime, nor did it produce any warning — I only discovered it buried in the API documentation. This is the unknown unknown: I couldn't have searched for the answer because I didn't even know this constraint existed. I'm not assigning blame here — just acknowledging that unknown unknowns exist, and I need to be aware myself and try not to introduce unknown unknowns while writing code.

I believe I will gradually get a deeper understanding as I continue developing code.

---

## Key Takeaways:

- Balance tactical speed with strategic design — neither extreme works
- Start simple and evolve; don't over-plan upfront
- Unknown unknowns are inevitable; try to minimize when possible

## How I Plan to Apply What I Learned:

- Before coding, research and balance multiple solutions instead of just the working one
- Keep an eye on the time I spend on designing and ask "Should I start implementing or keep designing?"
- For unknown unknowns and other mentioned flaws, check the book frequently to identify them and try to eliminate them accordingly.
