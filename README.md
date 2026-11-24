# I have nothing to say, but I'm saying it anyway

**Live:** https://hughesjoseph.github.io/corporeal/

A conversation that builds a space out of type. Each spoken sentence is set on a plane and hung in the room, the next one opposite, the next one further in, until talking has made a corridor. Fly close to any letter and it gains depth, dissolving into soft gradients of its own colours.

The type is **Corporeal**: Helvetica, as a 2013 screen drew it.

## Origin

In September 2013 I took screenshots of Helvetica on an iMac and enlarged them in Photoshop. The letters came back fringed: yellow and orange on the left of each stroke, blue and cyan on the right. This is subpixel rendering. Each pixel is a red, a green and a blue stripe, and the system lit them separately to smooth an edge.

I always imagined that accident as a kind of variable type in RGB, using the Z axis where the screen only had two dimensions. Separating and re-blending the channels in Photoshop never came close, because it isn't a blend. This is the reconstruction.

## How it works

1. **Glyphs from the source.** Every character was cut from the 2013 specimen screenshot with its fringes intact, together with its baseline and original spacing. Sentences are set by laying those glyphs down like ink on white.
2. **The screenshot, enlarged.** The text is enlarged with a soft bicubic filter, like the screenshot in Photoshop: no pixels, only fringes. Close up, red and blue slide apart in the screen's own order (red right, blue left).
3. **Depth.** Behind each sentence the letters continue as a soft volume, ray-marched in the browser. Every layer further back is the same screenshot, blurrier and with wider fringes, accumulated like smoke or a prism's shadow.
4. **Conversation.** Speech comes through the browser's speech recognition. Turns alternate walls. The demo is set with quotations from John Cage, Muriel Cooper and Alan Fletcher.

One HTML file: WebGL (three.js), Web Speech API. No build step.

## Specifications

| | |
|---|---|
| Source | Screenshots, 8 and 13 September 2013 |
| Machine | iMac (2013) |
| System | OS X 10.8 Mountain Lion, or a pre-release of 10.9 Mavericks; LCD font smoothing on |
| Enlarged in | Adobe Photoshop CC (14.0) |
| Typeface | Corporeal (2013): Helvetica, screenshotted with LCD smoothing and enlarged |
| Rendering | Subpixel, RGB stripe order |
| Rebuilt | 2026, on macOS Tahoe 26. macOS stopped subpixel smoothing in 2018, so here it is reconstructed in code |

## Context

- John Cage, *Lecture on Nothing* (c. 1949–50), published in *Silence* (1961): "I have nothing to say / and I am saying it."
- Alan Fletcher, poster *I Have Nothing to Say And I'm Saying It*; *The Art of Looking Sideways* (2001).
- Muriel Cooper and the MIT Visible Language Workshop, *Information Landscapes* (TED5, 1994).
- 90s editorial type: David Carson, *Ray Gun*.

## Run it

Open `index.html` from a local server (the microphone needs https or localhost):

```
python3 -m http.server 8000
```

then visit `http://localhost:8000`. Best in Chrome on a laptop.

---

Joseph Hughes, 2026. Code written with AI assistance.
