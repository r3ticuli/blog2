---
layout: post
title: how i think about design
date: 2020-11-28 19:59 -0500
---

design aesthetics are rarely a trait attributed to software engineers.

for some reason, it is popular to consider developers as at odds with their designers. a common trope is for the designer to give a dev some spec, the dev builds it out, and the designer then asks a slew of questions such as "did you use the exact hex value for that yellow? it looks a bit muted...", or the painful "could you please nudge this a pixel to the right?". While design hand off is rarely a perfect science, this depiction has always seemed a bit hyperbolic. A user's experience with the visual component of our product bears significant weight on how much a product is enjoyed. **A developer who disregards this consideration is a bad developer.**

Whenever I build software, I always make a mockup. Always. Doing so provides the following benefits:

- development is focused on delivering the mockup
- edge cases are considered early in the dev process.
- reaffirmation of the goal of the product.

After having built products for the majority of the last 4 years of my life, I've devised a framework that helps me build mockups for my products.

# the mockup framework

1. build a mood board
   - assemble pictures of interfaces from competitors, existing apps, software in your solution space, etc.
2. pick apart the mood board
   - which pictures resonate with you? Which do not? consider why this is the case. write these points down as goals for your product
3. build rough sketches for FEATURES, not components.
   - I am a top down thinker. If we start from the top, we start with a product. this product serves some purpose through its features. This is the smallest component one can usefully design. this is why I prefer to let features drive the design process. Components are too low level, and can be more easily solved once the feature space is fixed.
   - consider the features of your product. What are they? How do users interact with them?
   - Pick a feature, and determine all of the data it is composed of (date, goal, is it accomplished?)
     - design is a multidimensional problem space.
     - you need to solve for multiple things
       - how do you visually represent goals, how will you label each of these goals, and how will you incorporate time into the picture?
       - those are 3 individual problems which can be solved individually in multipleways.
4. Iterate
   - don't create just one version of a facet of a feature. Try to be exhaustive, and iterate through at least 2 approaches. This gives you variability, which is essential to the design process.
   - keep making variants until you cant come up with any more sensible ones.
5. Compile
   - take your variants of a feature, and begin to mix and match them to compose the feature as a whole
   - you will quickly lean in favor of one over the other
   - create a top 3
6. Assess
   - have a user (or a professional designer if that is too difficult) assess your work, and provide constructive feedback/criticism
7. Improve
   - implement feedback and make your mockup better
8. Color
   - now that you have the structure in place, it is time to introduce color.
   - color is a tricky one. There are various blog posts on how to think about color, but the cliff notes are: Green = positive, Red = negative, yellow = caution, dark/black = layout, grey = neutral/demarcation
   - create variations of palettes, no more than 10.
   - each of these palettes will serve as a theme. your tool should support themeing in some capacity (figma : https://blog.prototypr.io/creating-themed-versions-of-a-master-design-in-figma-3d6679ffdeb7, sketch : xxx)

TODO

- talk more about solving open problems by fixing as many variables as possible.
- update this as the mockup is completed.
