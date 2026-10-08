# Interaction recipes

A page can be completely correct and still feel flat. The gap between flat and expensive is usually a few small moments where the page notices you're there.

These are the small moments from my portfolio, [miguelclavel.com](https://miguelclavel.com/?utm_source=github&utm_medium=recipes), each one written up the way I built it: what it does, what went wrong, and **the exact prompt**, so you can paste it into Claude or any AI coding tool and get it on your own site. Three of them also have a live demo with plain, copyable code. No libraries, no build step.

**[Try the live demos](https://miguelclavel.github.io/interaction-recipes/)** · By [Miguel Clavel](https://github.com/miguelclavel), Senior Product Designer

<table>
  <tr>
    <td width="50%" valign="top"><a href="01-name-hover/"><img src="01-name-hover/demo.gif" alt="Letters of a name reacting one at a time"></a><br><b><a href="01-name-hover/">01 · A name where every letter reacts on its own</a></b><br><sub>Eight hover animations, cycled so neighbours never match. Live demo.</sub></td>
    <td width="50%" valign="top"><a href="02-pixel-trail/"><img src="02-pixel-trail/demo.gif" alt="A trail of coloured squares following the pointer"></a><br><b><a href="02-pixel-trail/">02 · A pixel trail behind the hero</a></b><br><sub>A grid that remembers the brightest it's been, so the trail holds its shape. Live demo.</sub></td>
  </tr>
  <tr>
    <td width="50%" valign="top"><a href="03-wave-line/"><img src="03-wave-line/demo.gif" alt="A divider line bending toward the pointer"></a><br><b><a href="03-wave-line/">03 · A line that bends toward your cursor</a></b><br><sub>One control point, a spring that keeps 86% each bounce, no overlay. Live demo.</sub></td>
    <td width="50%" valign="top"><a href="04-scroll-into-header/"><img src="04-scroll-into-header/demo.gif" alt="A large name shrinking into the header on scroll"></a><br><b><a href="04-scroll-into-header/">04 · A name that travels into the header</a></b><br><sub>One scroll number from 0 to 1 drives everything, through an easing curve.</sub></td>
  </tr>
  <tr>
    <td width="50%" valign="top"><a href="05-cards-from-sides/"><img src="05-cards-from-sides/demo.gif" alt="Screenshots flying in from both sides"></a><br><b><a href="05-cards-from-sides/">05 · Screenshots that fly in from both sides</a></b><br><sub>Why the first version looked like a slideshow, and what fixed it.</sub></td>
    <td width="50%" valign="top"><a href="06-images-frame-text/"><img src="06-images-frame-text/demo.gif" alt="Images moving out to frame a line of text"></a><br><b><a href="06-images-frame-text/">06 · Images that turn into the frame for the text</a></b><br><sub>Images placed around an invisible circle, leaving the centre clear.</sub></td>
  </tr>
  <tr>
    <td width="50%" valign="top"><b><a href="07-pixel-dissolve/">07 · A pixel dissolve from light into dark</a></b><br><sub>Two thirds order, one third noise. Took four tries.</sub></td>
    <td width="50%" valign="top"><a href="08-footer-game/"><img src="https://github.com/miguelclavel/pixel-run-game/raw/main/assets/pixel-run-light.png" alt="A small runner game where the blocks spell a name"></a><br><b><a href="08-footer-game/">08 · A playable game in the footer</a></b><br><sub>The thing you jump over is my own name. Full code in <a href="https://github.com/miguelclavel/pixel-run-game">pixel-run-game</a>.</sub></td>
  </tr>
  <tr>
    <td width="50%" valign="top"><a href="09-case-study-carousel/"><img src="09-case-study-carousel/demo.gif" alt="Case study cards riding along a curve"></a><br><b><a href="09-case-study-carousel/">09 · Case studies that ride a curve</a></b><br><sub>Cards on a circle whose centre sits below the screen.</sub></td>
    <td width="50%" valign="top"><a href="10-selection-colour/"><img src="10-selection-colour/demo.gif" alt="Selected text highlighted in a brand yellow"></a><br><b><a href="10-selection-colour/">10 · A text selection colour that belongs to the brand</a></b><br><sub>The smallest detail on the site, and the one people notice.</sub></td>
  </tr>
</table>

## How to use a recipe

1. Open the recipe and watch the recording, so you know what you're aiming for.
2. Copy the prompt as it is and paste it into Claude, Claude Code, or any AI coding tool, along with your page.
3. Tune it. Every recipe says which number to play with.

For the three with live demos, you can also take the code straight from `index.html` in the folder. Each one is a single file.

## Why prompts and not just code

Because the decisions are the useful part. Each write up says what I got wrong before it worked: the letters that kept firing while the name was moving, the squares that lit up under the text, the dissolve that finished before anyone could see it. A prompt that carries those decisions gets you further than a snippet that doesn't.

If you build one of these, send it to me. I'd genuinely like to see it.

---

MIT licensed. Made by [Miguel Clavel](https://miguelclavel.com/?utm_source=github&utm_medium=recipes) with Claude Code. Also on [LinkedIn](https://www.linkedin.com/in/miguelclavel/).
