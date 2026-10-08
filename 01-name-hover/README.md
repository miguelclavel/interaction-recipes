# A name where every letter reacts on its own

<img src="demo.gif" width="720" alt="A name where every letter reacts on its own: a screen recording">

Here's the actual trick behind the hover effect on my name. Steal it.

I wanted the first thing you touch on the page to feel alive, without turning my own name into a toy. So the rule was simple: react to the exact letter under your mouse, never the whole word.

Each of the 12 letters in "Miguel Clavel" gets its own animation, and neighbours never share one. One squashes like jello. One tips over and swings back. One drops, then springs up past where it started. One flips right over in 3D. The rest shiver, pop, hop, or slide. Eight in total.

Here's the bit I had to fix by hand. They kept firing while the name was shrinking up into the header on scroll, which looked broken. One check stops a letter animating once the name starts moving.

If you build this, send it to me. I'd genuinely like to see it.

## The prompt

Copy it as it is and paste it into Claude, or any AI coding tool.

```text
Split this heading into individual letters, each in its own element. Write eight short hover animations: a squash and stretch, a tip over that swings back, a drop and spring up, a 3D flip, a sideways slide, a shiver, a scale pop, and a hop. Cycle them across the letters so neighbours never match. Each runs between half a second and two seconds, and plays only when the mouse enters that one letter. Give each a sensible transform origin. Turn it all off for reduced motion.
```

**[Try the live demo](https://miguelclavel.github.io/interaction-recipes/01-name-hover/)** · [Source](index.html) · [See it on miguelclavel.com](https://miguelclavel.com/?utm_source=github&utm_medium=recipes&utm_campaign=name-hover)

<sub>[All recipes](../README.md) · By [Miguel Clavel](https://github.com/miguelclavel)</sub>
