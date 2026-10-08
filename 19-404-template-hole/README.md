# Fix: the page that kept requesting a file called {{g.src}}

My site was requesting a page called {{g.src}}. Every single load, on one page, for who knows how long.

It's not a typo. That's a template placeholder, the thing that's supposed to get swapped for a real image path before anyone sees it.

Here's what happens. Browsers don't wait politely for your code to run. While they're still reading the HTML, they race ahead looking for images to start downloading early. That scanner found src="{{g.src}}", decided it looked like a file path, and went and asked the server for it. The server, reasonably, said no.

The image itself was fine. It loaded a moment later once my code filled in the real path. So nothing looked broken, which is exactly why it sat there unnoticed.

The fix is small. Keep the placeholder in a data attribute the browser ignores, and only move it into src once it's a real path:

I found it by loading all 14 pages in a headless browser and logging every request that came back 400 or worse. Took about two minutes and turned up one thing I'd never have spotted by looking.

Worth doing on your own site. You might be requesting something strange too.

## The prompt

Copy it as it is and paste it into Claude, or any AI coding tool.

```text
My image tags have a template placeholder in the src attribute, which the browser's preload scanner requests literally and 404s on. Move the placeholder into a data-src attribute instead, and add code that copies data-src into src once the value is a real path, checking that it no longer contains template syntax. Run that check both when the component mounts and whenever it updates.
```

[See it on miguelclavel.com](https://miguelclavel.com/?utm_source=github&utm_medium=recipes&utm_campaign=404-template-hole)

<sub>[All recipes](../README.md) · By [Miguel Clavel](https://github.com/miguelclavel)</sub>
