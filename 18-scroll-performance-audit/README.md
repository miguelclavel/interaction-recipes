# Fix: an animation that worked hard to change nothing

150 frames of animation work every 2.5 seconds, to change nothing at all on screen. That was my own site.

The hero animation on my portfolio never stopped running. It kept going long after you'd scrolled past it, nowhere near the screen.

Every frame it measured where things sat on the page, made the browser recalculate styles twice, and rewrote the position of every card. Sixty times a second, for as long as the tab stayed open.

The annoying part: once you scroll past the hero, all of those numbers are already sitting at their final value. It was doing the whole calculation to arrive at the answer it already had.

I measured it at the bottom of the page, before and after the fix. 150 frames in 2.5 seconds, down to 7.

Copy this prompt if your site might be doing the same thing:

One honest note: this didn't move my Lighthouse score at all. Lighthouse never scrolls, so it sits at the top where the animation is supposed to be running. The win is for people actually using the site, not for the score.

Still my favorite kind of bug. Nothing looked broken. It was just quietly doing nothing, very fast.

## The prompt

Copy it as it is and paste it into Claude, or any AI coding tool.

```text
I have a scroll-driven animation that runs on every animation frame. Add an IntersectionObserver watching the element that drives the scroll, and skip the animation work whenever that element is off screen. Give the observer a rootMargin of a few hundred pixels so it starts again just before the element scrolls back into view, and run one final frame as it leaves so nothing freezes halfway through a transition.
```

[See it on miguelclavel.com](https://miguelclavel.com/?utm_source=github&utm_medium=recipes&utm_campaign=scroll-performance-audit)

<sub>[All recipes](../README.md) · By [Miguel Clavel](https://github.com/miguelclavel)</sub>
