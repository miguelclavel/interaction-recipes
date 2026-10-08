# A 404 game that never hands you an impossible jump

<img src="demo.gif" width="720" alt="A 404 game that never hands you an impossible jump: a screen recording">

My 404 page has a small game on it, and it can't hand you a jump you're unable to make.

The code that drops the obstacles solves the physics first, and shrinks anything you couldn't clear.

Someone landing on a 404 page is already a little annoyed. They clicked something and it didn't work. So the page has one job, getting them back out. The game sits at the lowest layer and the three ways out sit on top of it. The toy is never between you and the exit.

Before it drops a block in front of you, it works out how long you'd be in the air above that height at the current speed, gravity and jump strength. If that's not clearly longer than the time it takes to cross the block, it makes the block shorter and tries again. If even the shortest one can't be cleared, it skips it. The speed climbs the longer it runs, so the blocks quietly shrink to keep up.

It also plays itself until you touch it, so nobody needs to be told there's a game. Stop for four seconds and it takes over again.

And every block is a letter of my name, one per block, cycling through MIGUEL CLAVEL. Most people never notice they're jumping over it.

If you want the fairness rule in something you're building, copy this exactly:

Go break a URL on my site on purpose. Type anything after the slash. It's the only time I'll ever invite someone to a 404.

## The prompt

Copy it as it is and paste it into Claude, or any AI coding tool.

```text
In my side scrolling jump game, obstacles spawn at random heights, so at higher speeds some of them become impossible to clear. Before spawning one, solve the jump physics for the current speed, gravity and jump strength, and work out how long the character stays above that obstacle's height. If that airborne time isn't comfortably longer than the time it takes to cross the obstacle, reduce its height and check again. If even the shortest version can't be cleared, skip it.
```

[See it on miguelclavel.com](https://miguelclavel.com/?utm_source=github&utm_medium=recipes&utm_campaign=404-page-game)

<sub>[All recipes](../README.md) · By [Miguel Clavel](https://github.com/miguelclavel)</sub>
