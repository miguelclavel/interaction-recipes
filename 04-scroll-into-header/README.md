# A name that travels into the header

<img src="demo.gif" width="720" alt="A name that travels into the header: a screen recording">

My name starts in the middle of the screen and ends up in the header.

It doesn't fade out and reappear up there. It actually travels.

Most portfolios have a big name on the first screen and a small one in the bar at the top, and they're two separate things. Swap one for the other and the reader feels the cut. I wanted one object that moves, so you always know where the name went.

Here's the whole idea in four steps.

1. Make the hero section tall, a few screens worth, and pin what's inside it to the top of the viewport while you scroll through.

2. Turn scroll position into one number between 0 and 1. How far are we through this tall section. That's the only input.

3. Feed that number into everything at once. The size of the name, where it sits, how much the rest fades. Nothing gets its own timer.

4. Bend the number through an easing curve before you use it. Straight lines feel mechanical. It's the step people skip and it's the one you actually feel.

The nice part is you can tune it forever by changing one number.

## The prompt

Copy it as it is and paste it into Claude, or any AI coding tool.

```text
Make my hero section three screens tall and pin its contents to the top while the user scrolls through it. Turn the scroll position inside that section into a single value from 0 to 1. Use that one value to move my name from large and centered to small and top left, and to fade the supporting text out as it goes. Run the value through an ease-out curve before applying it. When the section ends, leave the name parked in the header for the rest of the page.
```

[See it on miguelclavel.com](https://miguelclavel.com/?utm_source=github&utm_medium=recipes&utm_campaign=scroll-into-header)

<sub>[All recipes](../README.md) · By [Miguel Clavel](https://github.com/miguelclavel)</sub>
