# A text selection colour that belongs to the brand

<img src="demo.gif" width="720" alt="A text selection colour that belongs to the brand: a screen recording">

Select some text on my site. It won't be the blue you're used to.

It's the same yellow the pixels use, and that's not a coincidence.

Every browser highlights selected text in the same default blue. It's the one piece of your design the browser picks for you, and most people never touch it.

Mine's a warm yellow with near black text on top. It isn't a new colour though. It's the first of the four accent colours the pixel effects already use on the page, so selecting a sentence quietly reuses something you've already seen.

Here's the part worth stealing.

I didn't write a light version and a dark version. The pair is fixed. Yellow behind, near black in front, in both themes. Because both halves are locked together, the page theme can't break it.

That combination lands at about 13 to 1 contrast, which is far past the accessibility minimum. A selection colour is the easiest place in a design to accidentally make text unreadable, and it's the one nobody tests.

It's two lines of CSS. No JavaScript, no library.

Small thing. It's also the kind of detail that says somebody looked at every corner of the page, not just the parts people expect.

## The prompt

Copy it as it is and paste it into Claude, or any AI coding tool.

```text
Override the browser's default text selection colour for my whole site. Use an accent colour that already appears elsewhere in my design as the highlight, with a near black text colour on top of it. Set the same fixed pair in both light and dark mode rather than writing a variant for each, so the theme cannot make it unreadable, and check the pair passes contrast for normal text. Include the standard rule and the Firefox prefixed one.
```

**[Try the live demo](https://miguelclavel.github.io/portfolio-details/)** · **[Get the code: portfolio-details](https://github.com/miguelclavel/portfolio-details)** · [See it on miguelclavel.com](https://miguelclavel.com/?utm_source=github&utm_medium=recipes&utm_campaign=selection-colour)

<sub>[All recipes](../README.md) · By [Miguel Clavel](https://github.com/miguelclavel)</sub>
