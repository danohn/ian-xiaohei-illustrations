# Ian Xiaohei Illustrations

> Turn the judgments, processes, states, and metaphors in English articles into clean, strange, hand-drawn inline illustrations on white backgrounds.
>
> 16:9 landscape | Xiaohei character IP | Hand-drawn on pure white | Sparse red, orange, and blue English annotations | Codex Skill

> **Note:** This repository is an English-translated fork of the original [Ian Xiaohei Illustrations](https://github.com/helloianneo/ian-xiaohei-illustrations) repository.

---

## What This Repository Is

Ian Xiaohei Illustrations is a Codex Skill that guides AI agents in generating inline illustrations for English articles, posts, blogs, Notion documents, and methodology content.

It is not a general-purpose illustration prompt or a PPT infographic template. Its core goal is to first understand the cognitive anchors in an article, then turn one judgment, process, structure, state, or metaphor into a memorable 16:9 hand-drawn explanatory illustration.

The default visual character is Xiaohei: a small, solid-black figure with white dot eyes, thin legs, and a blank expression. Xiaohei is not a mascot, sticker, or corner decoration, but an absurd worker seriously participating in the operation of a system.

In one sentence: **AI should not merely "add a picture"; it should draw a key cognitive action from the article.**

---

## Who It Is For

Especially suitable for:

- People writing English articles who need inline illustrations
- People creating knowledge content, methodology content, or AI workflow content
- People who want to turn abstract judgments into concrete metaphors
- People who want an illustration style lighter, stranger, and more distinctive than PPT infographics
- People using Codex for content production who want to reuse a consistent visual language

Not suitable for:

- People looking for commercial illustration, brand key visuals, or polished flat illustration
- People looking for traditional PPT infographics, complex architecture diagrams, or formal flowcharts
- People looking for children's cartoons, cute characters, or reaction-image styling
- People trying to fit large amounts of body text, long explanations, or a complete course page into one image
- People who need strictly editable vector source files

---

## What It Produces

Default outputs:

- 16:9 landscape inline illustrations
- A 4-8 image shot list for an article
- The theme, core idea, structure type, Xiaohei action, and suggested English labels for each image
- Final PNG images saved to `assets/<article-slug>-illustrations/` in the workspace

Not produced by default:

- PPTX / PDF / Keynote
- Editable SVG / HTML / Canvas graphics
- Commercial posters or cover key visuals
- Text-heavy infographics

---

## Visual Style

This skill uses Ian's default "strange Xiaohei inline illustration" style:

- Pure white background with no paper texture, beige, shadows, or gradients
- Thin, slightly wobbly black hand-drawn line art
- Plenty of white space, with the subject occupying only about 40%-60% of the canvas
- Sparse handwritten English annotations in red, orange, and blue
- One core action, structure, state, or metaphor per image
- Xiaohei must participate in the core action rather than serve as decoration
- Strange, creative, and clean, but neither childish nor cute

---

## Examples

### Two Breakpoints

![Two breakpoints](examples/images/01-two-breakpoints.png)

### Sort by Purpose

![Sort by purpose](examples/images/02-sort-by-purpose.png)

### One Source, Many Uses

![One source, many uses](examples/images/03-one-fish-many-uses.png)

### Handoff Path

![Handoff path](examples/images/04-handoff-path.png)

### Information Well

![Information well](examples/images/05-information-well.png)

### Idea Press

![Idea press](examples/images/06-idea-press.png)

### Content Fermentation

![Content fermentation](examples/images/07-content-fermentation.png)

### Trust Bridge

![Trust bridge](examples/images/08-trust-bridge.png)

These images are style-calibration examples, not composition templates. Invent a new metaphor for the current article instead of copying objects and compositions from previous examples.

---

## Installation

Clone the repository:

```bash
git clone https://github.com/helloianneo/ian-xiaohei-illustrations.git
cd ian-xiaohei-illustrations
```

Copy the skill into the Codex skills directory:

```bash
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
cp -R ./ian-xiaohei-illustrations "${CODEX_HOME:-$HOME/.codex}/skills/"
```

After installation, use it in Codex:

```text
Use $ian-xiaohei-illustrations to design and generate five strange Xiaohei inline illustrations for this English article.
```

---

## Usage

### Plan Illustrations Only

```text
Use $ian-xiaohei-illustrations, but do not generate images yet.
Analyze where the following article would benefit from illustrations and produce a shot list of about five images.
For each image, specify where it should appear, its theme, core idea, structure type, Xiaohei's action, and suggested English labels.

<paste article>
```

### Generate Inline Illustrations Directly

```text
Use $ian-xiaohei-illustrations to generate four strange Xiaohei inline illustrations for the following article.
Requirements: 16:9 landscape, pure white background, black hand-drawn line art, and sparse handwritten English annotations in red, orange, and blue.

<paste article>
```

### Generate One Illustration for a Concept

```text
Use $ian-xiaohei-illustrations to create an inline illustration for: "Trust is not declared; it is built one piece of evidence at a time."
The image should be strange but clean, and Xiaohei must perform the core action.
```

### Remove a Title or Incorrect Text

```text
Use $ian-xiaohei-illustrations to edit this image. Remove the "Flowchart" title from the top-left corner while preserving everything else.
```

See [examples/prompts.md](examples/prompts.md) for more examples.

---

## Workflow

The skill follows this process:

1. Read the article, Markdown, Notion content, screenshot, or user-provided topic
2. Extract core ideas, cognitive shifts, process structures, and passages worth visualizing
3. Produce a shot list first, choosing one cognitive anchor per image
4. Select a structure type for each image: workflow, system detail, before-and-after comparison, character state, conceptual metaphor, method layers, map route, or mini-comic sequence
5. Invent a low-tech physical metaphor that is strange but coherent
6. Make Xiaohei perform the core action
7. Generate each image separately with the image model
8. Check the QA checklist: white background, white space, Xiaohei's action, English labels, no PPT feel, and no copied example composition
9. Save the final PNGs and report their purpose and paths

---

## Directory Structure

```text
.
├── README.md
├── LICENSE
├── NOTICE.md
├── assets/
│   └── ian-wechat-qr.jpg
├── examples/
│   ├── images/
│   │   ├── 01-two-breakpoints.png
│   │   ├── 02-sort-by-purpose.png
│   │   └── ...
│   └── prompts.md
└── ian-xiaohei-illustrations/
    ├── SKILL.md
    ├── agents/
    │   └── openai.yaml
    ├── assets/
    │   └── examples/
    └── references/
        ├── style-dna.md
        ├── xiaohei-ip.md
        ├── composition-patterns.md
        ├── prompt-template.md
        └── qa-checklist.md
```

The subdirectory that should be installed into Codex is:

```text
ian-xiaohei-illustrations/
```

The root README, LICENSE, NOTICE, and examples are GitHub sharing documents.

---

## Notes

- Short English text in images is more reliable.
- Each image should explain only one core structure; do not turn the article into an instruction manual.
- Xiaohei must perform the core action. If the image still works perfectly after removing Xiaohei, the character is too decorative.
- Example images are only for calibrating line density, white space, restrained color, and Xiaohei's participation. Do not copy their compositions.
- AI image models may produce typos, hallucinated labels, style drift, or unnecessary titles, so inspect generated images.
- If labels contain serious errors, reduce their number and regenerate the image.

---

## Related Projects

- [Ian Handdrawn PPT](https://github.com/helloianneo/ian-handdrawn-ppt) - a Skill for generating hand-drawn technical PPT-style page graphics
- [Awesome Claude Code Skills](https://github.com/helloianneo/awesome-claude-code-skills) - a curated collection of Claude Code Skills, Agents, and Plugins
- [Obsidian + Claude AI Second Brain](https://github.com/helloianneo/obsidian-ai-second-brain) - a guide to building a personal knowledge base with Obsidian and Claude AI

---

## About the Author

**Ian** - Product designer / solopreneur / AI builder

Building a one-person company with an AI team.

- GitHub: [helloianneo](https://github.com/helloianneo)
- X/Twitter: [@ianneo_ai](https://x.com/ianneo_ai)
- Website: [www.ianneo.xyz](https://www.ianneo.xyz)
- WeChat: `ianneoxyz`
- Email: hello.neoc@gmail.com

---

## Keep Exploring

This Xiaohei illustration Skill is one small tool in the personal production system I am building with AI.

If you also use AI for content, knowledge bases, workflows, or product development, explore more on my website: [www.ianneo.xyz](https://www.ianneo.xyz).

You can also follow me on [X/Twitter](https://x.com/ianneo_ai).

To learn about Indie Builders Club, add `ianneoxyz` on WeChat and include the note `OPC`.

<p>
  <img src="assets/ian-wechat-qr.jpg" alt="Ian's WeChat QR code" width="120">
</p>

You can also find me on WeChat by searching for `ianneoxyz`.

---

## License

MIT License. See [LICENSE](LICENSE).
