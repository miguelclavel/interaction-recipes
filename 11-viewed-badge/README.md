# A case study list that remembers what you opened

Good case study pages just sit there. Great ones remember if you already looked.

On my site, once you open a case study and come back to the list, a small dot and the word "Viewed" show up next to it. Nothing loud, just enough to help you keep track of what you've already seen if you're browsing through several.

It resets if you close the tab or come back another day. It's not trying to track you forever, just to help while you're actually looking around.

Here's the prompt that builds this:

Small detail, but it's one of my favorite ones on the whole site.

## The prompt

Copy it as it is and paste it into Claude, or any AI coding tool.

```text
When a link to a project is clicked, save that project's id into a list in sessionStorage. On the page that lists all the projects, check that saved list against every project shown, and reveal a small hidden badge next to any project whose id is in the list. Keep the badge hidden by default so it only ever appears for something the visitor actually opened.
```

**[Try the live demo](https://miguelclavel.github.io/portfolio-details/)** · **[Get the code: portfolio-details](https://github.com/miguelclavel/portfolio-details)** · [See it on miguelclavel.com](https://miguelclavel.com/?utm_source=github&utm_medium=recipes&utm_campaign=viewed-badge)

<sub>[All recipes](../README.md) · By [Miguel Clavel](https://github.com/miguelclavel)</sub>
