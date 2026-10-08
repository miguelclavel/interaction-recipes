# A playable game in the footer

There's a playable game hiding in the footer of my portfolio.

The thing you're jumping over is my own name.

Scroll to the bottom and my face is running. Blocks come at you from the right and you hit space to jump them. Miss one and it's over.

Look closely at the blocks. Each one's a letter, and together they spell MIGUEL CLAVEL. Hand drawn, one letter per block, as little 8 by 8 grids of hashes and dots in the code.

Why put a game in a footer at all.

A footer is where people land when they're done. Either they leave, or you give them a reason to stay ten more seconds. It makes the page feel like somebody actually lives there.

The physics are four numbers. Gravity pulls down hard, the jump pushes up a little less hard, and the world starts at a walking pace then ramps to more than twice that. Tuning those four against each other is the whole game design. Too floaty and it's boring, too heavy and it's unfair.

And when nobody's playing, it plays itself. It runs, it jumps, it keeps going in the background, so it's alive whether or not you touch it.

Fair warning, I've lost more time to this than I'll admit.

## The prompt

Copy it as it is and paste it into Claude, or any AI coding tool.

```text
Build a small side scrolling runner in the footer of my page. The character jumps on space or click, with gravity so the jump arcs. Blocks scroll in from the right and the run ends on a hit. Draw each block as a letter from my name, defined as an 8 by 8 grid of on and off pixels in the code, one letter per block. Start the world slow and ramp the speed up to roughly double over a run. Show the current score and the best score of the session. When nobody has played for a while, let the game play itself in the background.
```

**[Play it and get the code: pixel-run-game](https://github.com/miguelclavel/pixel-run-game)** · [See it on miguelclavel.com](https://miguelclavel.com/?utm_source=github&utm_medium=recipes&utm_campaign=footer-game)

<sub>[All recipes](../README.md) · By [Miguel Clavel](https://github.com/miguelclavel)</sub>
