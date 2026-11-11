---
name: hyperframes-launch-teaser
description: Create a 12-second product feature reveal from a screenshot or recording using HyperFrames. Use when a user wants a short launch teaser, a before-and-after feature demo, or an editable HTML video with one call to action.
---

# HyperFrames Launch Teaser

Ask for the product name, one feature, one before-and-after pair (or a recording showing the change), and a destination URL. Use the product’s real UI for the result. For an illustrative example, label the product or interface as fictional.

## Build the clip

Use a single 12-second composition at 1280×720. Keep the same visual subject across the first two scenes so the change is easy to see.

| Time | Shot |
| --- | --- |
| 0–3.6 s | Show the task or problem in the original UI. |
| 3.6–9 s | Show one action and the result it produces. Let the result hold long enough to read. |
| 9–12 s | Give viewers one next action and its destination. |

Use the [starter composition](https://github.com/SnapSnap-LLC/awesome-gpt-6-2-sol-videos/blob/main/examples/feature-reveal/index.html) as a reference. Follow the [HyperFrames timing contract](references/hyperframes-contract.md) for clips, media and the paused animation timeline. Keep the headline, the UI result and the call to action readable when viewed on a phone.

With Node.js 22+ and FFmpeg installed, run these commands from the project directory.

```sh
npx --yes hyperframes@0.9.33 check .
npx --yes hyperframes@0.9.33 render . --fps 30 -o feature-reveal.mp4
```

Inspect the three scene midpoints and the two cuts in the exported MP4. Deliver both the editable HTML and the video. For another example, [open the free Launchry feature demo](https://launchry.dev/?resource=product-motion-demo-02&lang=en&utm_source=github&utm_medium=skill&utm_campaign=awesome-gpt-6-2-sol-videos).
