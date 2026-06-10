---
name: ian-xiaohei-illustrations
description: Generate Ian-style inline illustrations for English content. Use when a user asks for strange Xiaohei hand-drawn illustrations, article illustrations, illustration suggestions, shot lists, title removal, or image edits for English articles, posts, blogs, Notion documents, workflow documents, methodologies, processes, structures, states, metaphors, or ideas. Defaults to the Xiaohei character IP, pure-white hand-drawn visuals, sparse red/orange/blue annotations, and a clean but imaginative style.
---

# Ian Xiaohei Strange Inline Illustrations

## Core Purpose

Design and generate 16:9 landscape inline illustrations for English articles. The goal is not commercial illustration, PPT infographics, or cute cartoons. Instead, turn a key judgment, process, structure, state, or metaphor from an article into a clean, strange, creative, and readable hand-drawn explanatory image that does not feel like an instruction manual.

The default visual character is Xiaohei: a solid-black figure with white dot eyes, thin legs, and a blank expression, seriously doing something absurd but coherent. Xiaohei must participate in the image's core action rather than stand nearby as decoration.

## Read These References First

Read only what the task requires rather than loading everything into context:

- `references/style-dna.md`: Style DNA, colors, text, and prohibitions.
- `references/xiaohei-ip.md`: Xiaohei's appearance, personality, action library, and prohibitions.
- `references/composition-patterns.md`: Structure types, original-metaphor methods, and anti-copying rules.
- `references/prompt-template.md`: Prompt template for generating one image.
- `references/qa-checklist.md`: Post-generation checks and iteration rules.
- `assets/examples/`: Use only for occasional visual calibration, not in the default generation path. Do not copy compositions, objects, or labels from these examples.

## Workflow

### 1. Understand the Content

First read the user's article, link, Notion page, Markdown file, or screenshot. Extract:

- The core idea
- The passages that carry cognitive shifts
- The content best explained visually
- The parts better left as text without an image

Do not distribute illustrations evenly. Prioritize cognitive anchors such as a core judgment, two breakpoints, an input-output loop, branching, a before-and-after comparison, one source with many uses, a handoff path, common pitfalls, or a change in character state.

### 2. Produce an Illustration Strategy First

If the user only asks to analyze illustration opportunities or decide where images are needed, produce a shot list first. For each image, specify:

- Where it should appear
- The image theme
- The core idea
- The structure type
- What Xiaohei is doing
- Suggested elements
- Suggested English labels

Default to 4-8 images. Use 1-3 for a short article, and rarely exceed 9 even for a long article. Use only what is needed and avoid turning the article into a picture book.

### 3. Generate Individual Images

If the user explicitly asks to generate, output, create, or make images, do not stop and wait for confirmation. Use the built-in `image_gen` tool to generate each image separately. Do not combine multiple images into one.

Each image should explain only one core structure. Every prompt must include:

- A 16:9 landscape inline illustration for English content
- Pure white background
- Black hand-drawn line art
- Sparse handwritten English annotations in red, orange, and blue
- Plenty of white space
- Xiaohei as the subject performing the core action
- No PPT styling, commercial illustration, childish cuteness, complex architecture, or type title in the top-left corner

Do not copy previous examples. Examples only establish style density and how Xiaohei participates. Do not directly reuse existing compositions such as conveyor-belt breakpoints, Xiaohei pulling lines, a source-material fish, a stamped-copy toolbox, or a common-pitfalls path unless the user explicitly asks to reproduce one. Invent a strange but coherent metaphor from the current article every time.

### 4. Check and Iterate

After generation, check `references/qa-checklist.md`. Regenerate or locally edit first if:

- Xiaohei is merely decorative
- The image is too crowded
- It looks too much like a flowchart or PPT slide
- There is too much English text or serious spelling errors
- A title such as "Common Pitfalls," "Flowchart," or "System Architecture" appears in the top-left corner
- The style is too cute, childish, or rigid
- The background is not clean white

### 5. Save and Deliver

If the user is working in a workspace, copy final images to:

```text
assets/<article-slug>-illustrations/
```

Name them in order:

```text
01-topic-name.png
02-topic-name.png
```

Preserve the original generated files. Do not overwrite existing assets unless the user explicitly requests replacement.

## Output Style

Keep the pre-generation strategy short and precise. After generation, include:

- How many images were generated
- The purpose of each image
- Their saved paths
- Which images are strongest and which are optional

Do not explain style theory at length; let the images speak for themselves.
