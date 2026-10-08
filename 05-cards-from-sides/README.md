# Screenshots that fly in from both sides

<img src="demo.gif" width="720" alt="Screenshots that fly in from both sides: a screen recording">

Four screenshots fly onto my homepage from both sides as you start scrolling.

The first version looked like a slideshow. Here's what fixed it.

They all left at the same moment, travelled the same distance, and landed together. One block sliding across. Technically correct and completely lifeless.

Real things don't arrive in formation. So each one got its own three numbers.

1. A start delay. Card one leaves straight away, card two waits a quarter of the way in, card four waits a third. They set off at different moments.

2. A distance. Each card starts a different distance off screen, between about a fifth and just under half the width of the stage. Different distance over the same time means different speed.

3. A vertical drift. Each one rises or falls a little on the way in, two up and two down, so they don't share a flight path.

The direction isn't a number. Each card flies in from whichever side it's headed for, so the screen empties and refills instead of everything sweeping one way.

Small numbers, big difference. Change one delay and watch it come apart.

## The prompt

Copy it as it is and paste it into Claude, or any AI coding tool.

```text
I have four images that animate into place as the user scrolls. Give each one its own start delay, its own travel distance, and its own small vertical drift, so they arrive as a loose sequence instead of one block. Measure the distances as a fraction of the container width, plus the image's own width, so every screen size pushes them fully off screen first. Have each image enter from the side it ends up on. Ease each one in and fade it up as it travels.
```

[See it on miguelclavel.com](https://miguelclavel.com/?utm_source=github&utm_medium=recipes&utm_campaign=cards-from-sides)

<sub>[All recipes](../README.md) · By [Miguel Clavel](https://github.com/miguelclavel)</sub>
