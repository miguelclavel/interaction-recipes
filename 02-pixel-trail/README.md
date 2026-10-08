# A pixel trail behind the hero

<img src="demo.gif" width="720" alt="A pixel trail behind the hero: a screen recording">

Move your mouse across the top of my site and you leave a trail of coloured pixels behind you.

It took three tries to stop it looking cheap.

The space around my name was dead space. I wanted it to answer you without competing with the words sitting on top of it.

So it's a grid, not a cursor. The page is split into 102 columns of small squares. Your pointer charges up whichever squares it passes near, and each one remembers the brightest it's ever been. That single rule is what makes the trail hold its shape instead of flickering out behind you.

The brightest squares paint in the page's own colour, white on dark and near black on light. The dimmer ones scatter into colour around the edges.

Here's what I got wrong twice. Squares kept lighting up underneath my name. I blocked the charge where the text sits and they still lit up, because the radius reaches in from outside it. The fix was to stop drawing there at all, not to stop charging.

Fair warning, you'll lose ten minutes drawing circles with your own mouse.

## The prompt

Copy it as it is and paste it into Claude, or any AI coding tool.

```text
Add a full width canvas behind my hero, split into a grid about 100 columns wide. As the pointer moves, raise an energy value on every cell within 60 pixels of it, and let each cell keep the highest energy it has reached rather than following the pointer back down. Fade energy slowly, twice as fast once the pointer has been still for half a second. Draw the highest energy cells as solid squares in the page text colour and lower ones in random accent colours, skipping the faintest. Never draw over the rectangle where my hero text sits.
```

**[Try the live demo](https://miguelclavel.github.io/interaction-recipes/02-pixel-trail/)** · [Source](index.html) · [See it on miguelclavel.com](https://miguelclavel.com/?utm_source=github&utm_medium=recipes&utm_campaign=pixel-trail)

<sub>[All recipes](../README.md) · By [Miguel Clavel](https://github.com/miguelclavel)</sub>
