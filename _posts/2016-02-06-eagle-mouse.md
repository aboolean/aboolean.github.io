---
layout: post
title: Better EAGLE Zoom/Pan
tags: electronics
published: true
---

Most traditional EAGLE users insist on using a three-button mouse; others enjoy the fluidity of using a Mac trackpad to pinch/swipe to zoom/pan. I'm somewhere in between: I want a desktop setting without sacrificing efficiency.

# Zoom in EAGLE with A Normal Mouse

The mouse triggers virtual buttons 4 and 5.

![image](/media/2016-02-06-eagle-mouse/ss-1.png)

[BetterTouchTools](https://www.boastr.net/) translates buttons 4 and 5 (detected as 3 and 4) to keyboard shortcuts. This intermediate levels adds flexibility by allowing the buttons to be used for different functions in other applications.

![image](/media/2016-02-06-eagle-mouse/ss-2.png)

Finally, the shortcuts are assigned in EAGLE.

![image](/media/2016-02-06-eagle-mouse/ss-3.png)

Note that `WINDOW (@) 2` will zoom in by 2X relative to the position of the cursor.

# Panning in EAGLE

Run `SET Interface.UseCtrlForPanning 1`. Hold down the **CMD** key and drag the mouse to pan on Mac OS. This behavior is the same on Windows with the **CTRL** key.

# Conclusion

None of this is obvious or straightforward, but it's well worth the effort to efficiently use EAGLE on a desktop machine.

![image](/media/2016-02-06-eagle-mouse/demo.gif)