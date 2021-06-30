# MemberOfTheOrder's Satisfactory Guiding Principles

_Satisfactory? More like Refactory_

## Preamble

_AKA the boring part of the recipe that no one reads_

As a software engineer, I find myself constantly looking to apply good design patterns in my work.
As will soon be obvious, similar principles apply to Satisfactory.

One of the biggest benefits of good, modular software design is improvements to the refactoring process.
When refactoring is easier and more obvious, there's less potential for introducing bugs with each change,
AND change is no longer something to fear, but rather something to be encouraged.

I call this "developing via refactoring". The idea is that each step of software development should be about
_refactoring_ new features into a working product.
Rather than starting from nothing and gradually building into something useable, start with a working product
with the most minimal possible set of features. From there, the smallest possible improvements are added one at a time.
This means that your project is always in working condition, and changes to the original plan (new features, discovered bugs, etc.)
can be implemented on the fly.

What does this mean for Satisfactory?

Turns out, FICSIT Pioneers and software engineers want the same things - ease of growth without ever sacrificing functionality.
To accomplish this in Satisfactory, we must **identify the problems that make refactoring hard.**

## What makes refactoring hard?

* **Not being able to reach your machines** for either viewing or construction purposes certainly would discourage modifying the factory.
* **Nowhere to grow** - if there's no space to expand, expansion becomes very difficult.
* **Tight coupling** - if factory line A produces _exactly_ the amount of material for line B, then when line C needs some of line A, everything needs to be redone.
* **Scattered resources** - what happens when you need more iron ingot, but there are 12 different places to check for excess? That's right! "I don't wanna deal with it"

## How do we make refactoring easy?

### Room to Breathe

#### Walkways

As an engineer, you need to be able to see ALL moving parts of your factory, and you need to be able to access all parts in order to change anything.

If you can't see what's happening, you can't know where changes need to happen / where there's opportunity for improvement.

If you can't reach some component, you can't change it without other changes.
"To do A we need to do B, and to do B we need to do C" makes for a great D&D adventure, but that's because it requires heros to accomplish.
Don't be a hero. Be a lazy engineer.

#### Room to Grow

Picture it, you have an awesome factory and you need more Resource^(TM), but the factory producing it is very close to other factories on 3 sides, and a cliff on the 4th.
You can (and should) build upwards, but then the extra Resource^(TM) needs to be piped/belted away. If there's no space to do that... you get hard to modify spagget.

Instead, make sure there's plenty of space (upwards and ground space) to expand. More space between sub-factories means more space to organize the output/input redirection.

### Loose Coupling

Instead of making one big factory to produce complex materials, make many sub-factories that have exactly 1 job - 1 output.

One of the most consistent, earliest, and most annoying problems I have early-game is suddenly needing copper wire or screws.
At first, those are just useless intermediary products used to construct useful things (cable or reinforced plates).
When I suddenly need those for other things, I have to completely redo those factories.

If I had kept those as separate sub-factories, all I'd have to do is slap on a splitter and redirect some output to the new factory. Done.

### High Cohesion

Avoid producing the same resource in multiple places.
That way, when you need more of that resource, you know exactly where to go and it's very easy to determine what you need to do to get more of it.

It also means that planning becomes easier. You have the option to pipe the final input to it's dependent factory's output before that dependent factory is able to provide for it.

## Further considerations

One final problem that I haven't yet resolved is how to arrange the sub-factories.
In the same way that these principles guide how to arrange machines within a sub-factory, I endeavour to find similar guiding principles to arrange sub-factories within a factory.
