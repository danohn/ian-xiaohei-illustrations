# QA Checklist

## Required

- The image is 16:9 landscape.
- The background is clean white.
- Xiaohei is present.
- Xiaohei performs the core action rather than serving as decoration.
- The image does not copy an old example composition and instead creates a new metaphor for the current article.
- The image is strange, creative, and interesting.
- The image is simple and clean, with the main subject occupying no more than about 60% of the canvas.
- The image explains only one core structure.
- English labels are sparse, short, and readable.
- Orange is used only for the main path or arrows.
- Red is used only for emphasis, problems, warnings, or results.
- Blue is used only for secondary notes, feedback, or system state.

## Failure Signals

Regenerate or locally edit if:

- A title such as "Common Pitfalls," "Workflow," "System Architecture," or "Roadmap" appears in the top-left corner.
- Xiaohei looks like a mascot, reaction image, or cute cartoon.
- The image looks like a PPT slide, course material, or formal flowchart.
- There are too many elements, arrows, or nodes.
- The text becomes a long explanation.
- The background has paper texture, shadows, gradients, beige, or noise.
- The image contains a real UI screenshot or futuristic interface.
- English text has serious spelling errors or unreadable labels.
- The image is too rigid and lacks an absurd metaphor.
- The composition is too similar to an old example in `assets/examples/`.

## Iteration Methods

- Too ordinary: Make Xiaohei the subject performing the action and add a strange but coherent metaphor.
- Too complex: Remove nodes, leaving one action and 3-5 short labels.
- Too cute: Emphasize `deadpan`, `blank serious expression`, `not cute`, and `not mascot`.
- Too PPT-like: Remove titles, borders, tidy grids, and excessive arrows; turn it into a hand-drawn scene.
- Too similar to an old example: Preserve the core idea but replace the main object and Xiaohei's action.
- Incorrect text: Prefer a local edit. If many labels are wrong, regenerate with fewer labels.

## Delivery Standard

A high-quality image should first make the reader think, "That is a little strange," then make the structure clear within one second.

If it looks like a tutorial page at first glance rather than an absurd product sketch on white paper, it does not pass.
