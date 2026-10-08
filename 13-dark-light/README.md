# A dark mode that remembers you

<img src="demo.gif" width="720" alt="A dark mode that remembers you: a screen recording">

If your site forgets dark mode the moment someone refreshes the page, that's not a design choice. That's a bug.

Mine has a small toggle in the corner. Click it and the whole site switches between light and dark. Come back tomorrow, and it's still exactly how you left it.

The part people usually skip: on someone's very first visit, before they've touched the toggle at all, the site checks their operating system's own dark mode setting and matches it. Nobody has to make a choice they didn't already make once, in their system settings.

Here's the prompt:

Try switching it a couple times. I still think it's more fun than a toggle has any right to be.

## The prompt

Copy it as it is and paste it into Claude, or any AI coding tool.

```text
Add a button that switches the whole site between a light and dark color theme. When the visitor picks one, save their choice in localStorage so it's remembered the next time they visit. On their very first visit, before they've chosen anything, check their operating system's dark mode setting and match the site to it instead of defaulting to light.
```

**[Try the live demo](https://miguelclavel.github.io/dark-mode/)** · **[Get the code: dark-mode](https://github.com/miguelclavel/dark-mode)** · [See it on miguelclavel.com](https://miguelclavel.com/?utm_source=github&utm_medium=recipes&utm_campaign=dark-light)

<sub>[All recipes](../README.md) · By [Miguel Clavel](https://github.com/miguelclavel)</sub>
