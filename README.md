# 47loader

An open-source tape loader for the ZX Spectrum implemented from scratch.

## Why should I use 47loader for my next Spectrum project?

* Custom loaders are always more fun than using the ROM loader :-)
* By default, loads at ~160% of the ROM loader speed (543 T-states for a zero pulse, 1086T for a one pulse, versus the ROM loader's 855T/1710T). [Speed can be configured](Timings.md) up to 185% of the ROM loader speed (475T/950T).
* In addition to fast blocks, the loader can also cope with blocks using ROM timings, so the same build of your software can be distributed as both TZX and TAP files.
* Robust error detection using [Fletcher's algorithm](https://en.wikipedia.org/wiki/Fletcher's_checksum).
* [Choice of border effects](BorderThemes.md); additional themes can be added with a few lines of assembly language.
* [Choice of FancyScreen screen loading effects](FancyScreen.md), or an "instant" loading screen a la Speedlock.
* Optional colour-changing progress indicator.
* [Free, open-source software, liberally licensed](./LICENSE). 

## Why shouldn't I use 47loader?

* It's written by a rank amateur with next to no Z80 coding experience. 

## How do I use it?

  * Start by looking at a [simple example](./docs/SimpleExample.md).
  * Here's [how to specify the speed of the loader](./docs/Timings.md).
  * You can [load blocks glued together with no gaps](./docs/Resume.md).
  * A [loading screen that pops up instantly](./docs/Instascreen.md) always looks slick.
  * Or perhaps you'd like a [bidirectional screen load](./docs/FancyScreen.md)?
  * The [error handling can be configured](./docs/ErrorHandling.md).
  * It's fairly simple to [embed the loader in a REM statement in a BASIC loader](./docs/EmbeddingInBasic.md).