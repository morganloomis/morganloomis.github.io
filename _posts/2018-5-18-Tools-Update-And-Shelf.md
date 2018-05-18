---
layout: post
title: Tools Update and Shelf Added
---

![shelf](https://github.com/morganloomis/morganloomis.github.io/blob/master/images/animationShelf.png)

I've finally gotten around to supporting a shelf for the animation tools, it's included in the [gitHub repository](https://github.com/morganloomis/ml_tools) or you can download it individually [here](https://github.com/morganloomis/ml_tools/blob/master/prefs/shelves/shelf_MLAnim.mel).

I've also done a few tool updates over the last couple weeks:
* World Bake has the option to parent or unparent an animated node in one click, rather than the old two-step process
* Arc Tracer was calculating in a way that was faster, but wasn't accurate for how certain rigs were evaluating. Now it tests for accuracy first and runs either a fast or slow algorithm depending on the results.
* Anim Curve Editor has a delete frame option, which ripple deletes a single frame, moving all the following animation one frame forward. This mimics functionality in other animation packages.
* Copy Anim will now copy one to many if you select more than two objects.
