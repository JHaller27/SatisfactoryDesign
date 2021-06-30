# MemberOfTheOrder's Satisfactory Guiding Principles

_Satisfactory? More like Refactory_

## Preamble

_AKA the boring part of the recipe that no one reads_

As a software engineer, I find myself constantly looking to apply good design patterns in my work.
As will soon be obvious, I believe that similar principles apply to Satisfactory.

One of the biggest benefits of good, modular software design is improvements to the refactoring process.
When refactoring is less difficult and less surprising, there's less potential for introducing bugs with each change,
AND change is no longer something to fear, but rather something to be encouraged.

I call this "developing via refactoring". The idea is that each step of software development should be about
_refactoring_ new features into a working product.
Rather than starting from nothing and gradually building into something useable, start with a working product
with the most minimal possible set of features. From there, the smallest possible improvements are added one at a time.
This means that your project is always in working condition, and changes to the original plan (new features, discovered bugs, etc.)
can be implemented on the fly, in any order.

What does this mean for Satisfactory?

Turns out, FICSIT Pioneers and software engineers want the same things - ease of growth without ever sacrificing functionality.
To accomplish this in Satisfactory, we must identify the problems that make refactoring hard.

## What makes refactoring hard?

* **Not being able to reach your machines** - if you can't see it nor touch it, you can't change it.
* **Nowhere to grow** - if there's no space to expand, expansion becomes very difficult.
* **Tight coupling** - if _exactly_ the right amount of material is piped _directly_ from line A into line B, then when line C needs some line-A resource,
potentially all 3 lines need to be redesigned.
* **Scattered resources** - what happens when you need more iron ingot, but there are 12 different places to check for excess? Generally speaking, what happens is a very frustrated pioneer.

## How do we make refactoring easy?

### Room to Breathe

#### Walkways

As a pioneer, you need to be able to see and touch ALL moving parts of your factory in order to change anything.

If you can't see what's happening, you can't know where changes need to happen or where there's opportunity for improvement.

If you can't touch some component, you can't change it without dismantling other parts of your factory or building ad-hoc structures that serve no long-term purpose.

Leave room to build walkways so that all parts of your factory are accessible.
You can build walking space between factories.
You can build elevated catwalks.
You could maybe even build catwalks underneath your factory and use glass floors to see up (though you wouldn't be able to see if belts are backed-up or unexpectedly empty).

Make it as easy as possible to see what's happening, and to reach any and every part of your factory. Obstacle courses and jumping-puzzles are fun, but become really annoying when they're repetitive.

#### Room to Grow

Picture it, you're building an awesome factory and you need more Resource^(TM). The factory producing it has a picturesque location betweeen 3 other factories, and a cliff. You stare at this art-piece of a building... and try to figure out how to expand it to produce more.

You can (and should) build upwards, but then the extra Resource^(TM) needs to be piped/belted away. If there's no space to do that... you get hard to modify spagget.

Instead, make sure there's plenty of space (upwards and ground space) to expand. More space between sub-factories means more space to organize the output/input redirection.

### Law of Least Surprise

This means that things should behave in such a manner as to cause the least amount of surprise. Alternatively, a goal should be accomplished using the least surprising methods.

For Satisfactory, ideally, every sub-factory would be identical. That way, it's very easy to see where there are problems, because those will be the only places that something is different (and humans are by-and-large very good at spotting things that don't match a pattern).

This is not entirely possible, so - as much as _is_ possible - sub-factories should be symmetrical. This applies between sub-factories (e.g. the iron sub-factory ought to be similar to the copper sub-factory), and within each sub-factory (machines and supply lines ought to be arranged uniformly).

This way, while you are using your _Room to Breathe walkways_, you'll always know where to go, and it will be easy to spot unexpected inconsistencies.

Additionally, this encourages the development and use of standard designs.
Standard designs means that expansion can happen without too much thought (and with very little training if playing with additional pioneers), and that extensions won't introduce new patterns.

### Loose Coupling

Instead of making one big factory to produce complex materials, make many sub-factories that have exactly 1 job; 1 output.

One of the most consistent, earliest, and most annoying problems I have early-game is suddenly needing copper wire and screws.
At first, those are just useless intermediary products used to construct actually useful things (cable and reinforced plates respectively).
When I suddenly need those for other things, I have to completely redo those factories.

Keep these as separate sub-factories. That way, all you need to do is modify the output slightly (e.g. a splitter) and redirect some output to new destinations.
And since we build with _Room to Grow_ and _Law of Least Surprise_ in mind, if there is no surplus, it should be easy to expand the sub-factory to produce more.

### High Cohesion

Avoid producing the same resource in multiple places.

That way, when you need more of that resource, you know exactly where to go and it's very easy to determine what you need to do to get more of it.
Instead of investigating 12 different locations for possible surplus, you can go to the one and only place that resource is produced and see exactly how much is being produced.
