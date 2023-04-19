---
layout: post
title: Tokenization
description: Jupiter Money's Design System
author: Sumit
tags: 
image: /img/thumb/tokenization.png
thumb: /img/thumb/tokenization.png
---

<div class="hero-block">
    <img src="{{ site.tokenization.bg }}" alt="Tokenization in the Design system Europa" />
</div>

### What are Tokens?
Design tokens are all the values needed to construct and maintain a design system — spacing, color, typography, object styles, animation, etc. — represented as data. These can represent anything defined by design: a color as a RGB value, an opacity as a number, an animation ease as Bezier coordinates. They’re used in place of hard-coded values in order to ensure flexibility and unity across all product experiences.

>Essentially, a design token is a design decision: a pairing of the same code and visual properties—design elements you use over and over again in your products—packaged in a format that’s deployable across all platforms.

For example, let’s say your team decided your brand’s primary color is #276EE5. You could create a design token of the following: color.primary = #276EE5 (The token’s name is color.primary, and its value is #276EE5.)

### Why they are important?

> The design system is your land, and your design tokens are the language people use to communicate design decisions with each other.

The difference between design tokens and any other design variable is that they are an abstraction layer that makes them platform-agnostic.

Design tokens help you reach:
- Unique source of truth for your branding
- Better translation from design to development
- Design consistency across any product UI
- Improved management of your design system
- Easier management of themes and white-labelling features
- Proper methodology to collaborate between teams

Tokens forms the base for your Atoms which gives you the power to add/edit/upgrade any atom, molecule, organism etc.

<div class="post-section-img">
    <img src="{{ site.tokenization.tokens }}" alt="Tokens description"/>
</div>

#### Example
<div class="post-section-img">
    <img src="{{ site.tokenization.component-tokens }}" alt="Token implementation in a Design system"/>
</div>

### Current practice
As a front-end developer, I assume designers are responsible for taking design decisions. Updating a color, a font-size or any “core style” and seeing the result in whatever platform should be effortless for them. Unfortunately, this is not currently the case.

Let’s say a color needs to be updated. The current workflow would look like this:

1. The designer updates the color in the design tool.

2. This design update is shared to the developer.

3. The developer updates the value in the code.

4. The designer can see the result in a development environment.

This workflow suffers from several pitfalls:

- The designer depends on the developer to see the result of a core style update. This slows down the design process and makes the designer sad 😢
- Updating a color value in the codebase is not very time consuming when you only have to update a single style variable. However the time taken to do this change is less time for a developer to work on something valuable for the company. The developer is also sad 😢
- Since we often track project tasks with a task manager, this change would imply another ticket to deal with 😕
- From a general point of view, this time lost by the company also delays the go to market of its products 😪

This workflow can be optimized! 💪

#### Figma Tokens to the rescue
Close your eyes and imagine a world where a design tokens generator would be integrated in design tools.

Using a combination of <a href="https://www.figma.com/community/plugin/843461159747178978" target=_blank>Figma Tokens</a> and <a href="https://amzn.github.io/style-dictionary/#/README" target=_blank>Style Dictionary</a> you can automate this process.



#### How?
<div class="post-section-img">
    <img src="{{ site.tokenization.tokens-structure }}" alt="Tokens structure"/>
</div>

#### Steps
- Install &nbsp;<a href="https://www.figma.com/community/plugin/843461159747178978" target=_blank>Figma Tokens Plugin</a>
- Populate the entries in the plugin
<div class="post-section-img">
    <img src="{{ site.tokenization.tokens-entry }}" alt="Figma tokens overview"/>
</div>
- Head to the settings section and go to GitHub tab
- Enter the Github details of the repository where you want to push the code to, this is a little technical. You can take take help from your developers. 
<div class="post-section-img">
    <img src="{{ site.tokenization.tokens-github }}" alt="Figma tokens with Github"/>
</div>
- Done, You just automated the Process!!

The tokens/Json file would be pushed to the corresponding repo and the developer just need to pull that changes and you are good to go.

Code would be Integrated with <a href="https://amzn.github.io/style-dictionary/#/README" target=_blank>Style Dictionary</a> which would spit out CSS, iOS, Android format tokens.














<!-- This Design system is named after one of the Jupiter's moon.

### The current system(What)
Currently, it is a collection of individual components or you can say, a sticker sheet.
Designers use them and modify them according to their designs. There is a lack of documentation or rules/guidlines as to when and how those components or atoms should be used.

With a growing team and an ever-evolving product comes the need for an ecosystem of reusable components and helpful guidelines to build the best product we can for our users in the most efficient way. That’s where Europa, our design system, comes in.

### What is a Design System?
>A design system is a complete set of standards intended to manage design at scale using reusable components and patterns
> <br> - Nielson Norman Group


### What does it mean?
- It's like creating a unified language within and between cross-functional teams
- Also maintaining visual consistency across products, channels, and (potentially siloed) departments language within and between cross-functional teams


### Why it is needed?
- Are we always happy with the speed of product development?
- Do our interfaces share the same design patterns, colors, typography and other styles?
- Do we always have enough time to deliver a quality product to meet KPIs?
- How much time and money do we spend on redundant design or code tasks?
- How much time and money do we spend cleaning up design or technical debt?



### How?
### Design system structure
![](https://res.cloudinary.com/dcx5qfzvy/image/upload/v1660639575/design-system-structure_czi4k3.png) -->