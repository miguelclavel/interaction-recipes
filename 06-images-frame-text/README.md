# Images that turn into the frame for the text

<img src="demo.gif" width="720" alt="Images that turn into the frame for the text: a screen recording">

Keep scrolling my homepage and the screenshots move out to the edges.

They stop being the subject and become the frame.

I had a sentence I actually wanted people to read. The problem is screenshots always win. Put a line of text next to product shots and your eye goes to the pictures every time.

So instead of shrinking the images or fading them out, I moved them out of the way and let them hold the border while the sentence takes the middle.

Here's how it works.

1. Put the images on a ring, not in a row. Each one sits at its own angle around an invisible circle, so they spread to the corners instead of stacking on one side.

2. Let each image tilt to follow the curve. That's what makes it read as a ring rather than four pictures that happen to be far apart.

3. Fold every tilt back into a range of minus 90 to plus 90 degrees. Without this, the image at the bottom of the ring ends up rotated a full 180 and your screenshot is upside down. I shipped that bug before I caught it.

4. On narrow screens, turn the whole ring by half a step. With four images the ring puts one directly left and one directly right, which is exactly where the text sits on a phone.

The upside down one is the bug everyone hits. Now you won't.

## The prompt

Copy it as it is and paste it into Claude, or any AI coding tool.

```text
Lay my images out around an invisible circle, each at its own angle, so the centre of the screen stays clear for a line of text. Rotate each image to sit tangent to the circle, then fold every rotation into the range minus 90 to plus 90 so no image is ever upside down. On narrow screens, rotate the whole ring by half a step so no image lands on the horizontal centre line where the text is.
```

[See it on miguelclavel.com](https://miguelclavel.com/?utm_source=github&utm_medium=recipes&utm_campaign=images-frame-text)

<sub>[All recipes](../README.md) · By [Miguel Clavel](https://github.com/miguelclavel)</sub>
