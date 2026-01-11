---
layout: post
title: Thoughts on Claude Code videos
categories: learning-reflections
tags:
- ai
- Claude
date: 2025-12-30 02:41 +1100
---
## Anthropic AI Videos

- [Latest videos from Anthropic AI](https://www.youtube.com/@anthropic-ai/videos)
  - [Claude ran a business in our office](https://www.youtube.com/watch?v=5KTHvKCrQ00)
  - [What is sycophancy in AI models?](https://www.youtube.com/watch?v=nvbq39yVYRk)

*Note: The thoughts and ideas expressed below are my own. The language has been polished with assistance from Claude.*

---

## My Thoughts:

### [Claude ran a business in our office](https://www.youtube.com/watch?v=5KTHvKCrQ00)

In this experiment, Anthropic set up a real vending machine in their office and had Claude autonomously manage the business — handling customer interactions, pricing decisions, and operations.

The "Claude ran a business in our office" video highlights two key problems. First, the coupon incident: customers convinced Claudius they were influencers, and Claudius issued unauthorized discounts. This stems from Claude's design to prioritize user requests without questioning them -— an exact example of sycophancy. Splitting responsibilities between a customer-facing agent and a CEO agent as they did later should reduce this vulnerability, as decision-making authority becomes separated from user interaction.

Second, Claudius fabricated events like signing contracts and hiring staff, confusing the simulation with reality.

Both problems share the same root cause: AI relies too heavily on human input to understand reality. It lacks independent judgment standards. This design works well for responding to users with tailored content but fails when the AI needs to make autonomous decisions.

I wonder if it is a good idea to let ai explore and update by themselves and whether or not it helps with understanding the reality. Lesson learned is that for now AI also needs role division to make tasks clearer and help its performance, just like how humans divide roles in real life.

### [What is sycophancy in AI models?](https://www.youtube.com/watch?v=nvbq39yVYRk)

This video focuses on sycophancy, where AI generates content tailored to match preference of user according to prompt. I believe that is totally necessary because it can perfectly serve various people with various requirements under various situations. 

However, the video is warning that there are times where AI goes too far -- they prioritize user's preference too much that they even give generated answers that are not true.

I certainly experience it myself where AI gives some really ridiculous answers tailored to my preference while I want objective answers, and I have to manually point that out to lead it back to track. This is natural because humans themselves can neglect fact under certain situations, let along AI which mimic human behaviors.

### Takeaway: Practical Ways to Reduce Sycophancy

As suggested by the video, giving descriptive prompts or simply restarting the conversation can ease the problem. However, it is still not convenient enough — we need to keep an eye on this throughout the conversation. AI agents are certainly doing their job in giving tailored content, and I hope they can do better in finding the balance between preference and facts, and when to adjust that balance during the conversation.