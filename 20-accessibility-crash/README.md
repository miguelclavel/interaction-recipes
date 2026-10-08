# Fix: the keyboard support that crashed every time it ran

I wrote code to make my image viewer work with a keyboard.

It crashed every single time it ran, and nothing on the page ever looked wrong.

You click a picture on one of my case studies and it opens full size. The moment it opens, focus is supposed to jump to the close button, so if you're on a keyboard or a screen reader you land somewhere useful instead of somewhere random. Close it, and focus goes back to the picture you clicked.

To know the exact moment it opened, the code compared the new state to the state from a second ago.

The framework I'm using doesn't hand that function the previous state. It hands it the previous props. So the thing I was comparing against was nothing at all, and reading a value off nothing throws an error. Every line after it stopped running.

It threw on page load, before anyone had clicked anything.

And the page still looked perfect. The picture opened. The picture closed. The close button worked. The only broken part was the part you can only find by putting your mouse down.

Accessibility bugs fail quietly like this. A broken button is obvious because the page looks wrong. A broken focus move looks exactly like a working one.

I found it by loading all 14 pages in a headless browser and logging every console error. Took two minutes.

The fix, if you've ever written this kind of focus code:

Before: that error on every page load and every update. After: zero errors, and focus actually lands on the close button.

Go open your own site and look at the console. An error that fires on load is the cheapest bug you'll ever find.

## The prompt

Copy it as it is and paste it into Claude, or any AI coding tool.

```text
componentDidUpdate in my component assumes its second argument is the previous state, but this runtime only passes previous props, so that argument is undefined and every read from it throws. Rewrite the component to track the previous value itself: save the value you care about onto the instance at the end of componentDidUpdate, then compare against that saved copy at the start of the next call.
```

[See it on my second portfolio](https://miguelclavel-2.miguelclavel-1.workers.dev/?utm_source=github&utm_medium=recipes&utm_campaign=accessibility-crash)

<sub>[All recipes](../README.md) · By [Miguel Clavel](https://github.com/miguelclavel)</sub>
