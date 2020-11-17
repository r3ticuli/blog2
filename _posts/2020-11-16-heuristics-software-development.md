---
layout: post
title: heuristics & software development
date: 2020-11-16 22:49 -0500
---

There are various heuristics we use to drive towards the north star of clean code. Some classics include :

- Writing files with no more than `n` LOC (very controversial)
- One File per Class
- Don't Repeat Yourself
- Build components that are self contained & independent

I recently realized why these conventions even arise in the first place. **It all stems from laziness.**

1. **It is much more efficient to tell someone what to do, than to have them go figure it out**

   It's virtually useless to tell someone to "go and write clean code". Some would ask "What exactly do you mean by that?".

   To aim for clean code is to aim for an abstract concept. These heuristics ground that aim in actionable tasks.

   How can a file be cleaned? We can start by checking a couple of things:

   - is it a large file?
   - are these methods too alike?
   - is the language being used idiomatically?

   <br> Addressing these concerns will slowly chip away at complexity, and in their sum **can tend to result in clean enough code**.

2. **Reading complex code is mentally tolling**

   Complexity is reviled. Ask any developer, "_Would you rather work on a legacy spaghetti monolith, or a well oiled project?_". None will opt for the spaghetti monolith, because the well oiled project is easier to work with.

These heuristics are guide rails when looking to reduce the complexity of your software. Determining the right combination and timing of these tricks is part of the essential trade of the software engineer.
