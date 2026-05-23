# 📖 Content Coach — Usage Guide

## Overview

Content Coach helps TCGplayer employees write on-brand communications. It supports three modes and works with or without a specific component type selected.

---

## Modes

### Improve Text
Paste existing copy → get a revised, brand-aligned version with a rationale explaining the changes.

### Create Content
Describe what you need → get generated copy that follows brand guidelines.

### Design Link
Paste a Figma URL → the app reads the design, identifies components, and generates copy for all of them at once.

---

## Target Audience

Select **Buyers** or **Sellers** before submitting. The voice and tone guidelines differ significantly between the two.

---

## Component Type (optional)

Selecting a component type tells the model the format rules for that element:

| Component | Output fields |
|---|---|
| Inline error | Message |
| Blocking error (modal) | Title, Body, Primary CTA, Secondary CTA |
| Alert (banner / toast) | Message, CTA |
| Call to Action | Label |
| Heading / title | Text |
| Helper text | Message |
| Field label | Text |
| Inline hint | Message |
| Empty state | Title, Body, CTA |

When a component is selected in **Improve Text** mode, you fill in the existing field values and the model improves each one. In **Create Content** mode, the model generates all fields from your description.

---

## Processing Steps

Every request shows a real-time step panel:

1. **Analyzing Input** — Parsing your request
2. **Finding Guidelines** — Semantic search across brand guidelines (local vector index)
3. **Refining / Generating** — LLM call with style guides + retrieved guidelines
4. **Finalizing** — Parsing and formatting the response

---

## Results

### Primary Output
The main corrected or generated text (or per-field pieces for component mode).

### Variant Tabs
Every response includes 3 alternatives — **Primary** plus up to 3 labeled variants (e.g. "More direct", "Shorter", "More casual"). Switch tabs to compare.

### Refine Actions
Apply a follow-up instruction to the current result without re-entering your input:

- **Simplify this** — shorter words, simpler structure
- **Make it shorter** — remove redundant words
- **Make it clearer** — reduce ambiguity
- **Make it more direct** — active voice, lead with key info
- **Explain simply** — plain language, no jargon
- **Custom…** — type any instruction; the model validates it against brand guidelines

### Coach's Tips / Rationale
- **Improve Text**: conversational paragraph explaining what changed and why
- **Create Content**: bullet list explaining creative decisions and which guidelines were applied

### Guidelines Referenced
The specific guideline chunks that influenced the output, with relevance scores.

---

## Project Context (optional)

Enable **Use project context** and enter a project name to pull in relevant Jira/Confluence content via Atlassian MCP. This helps align terminology with the specific project.

---

## Tips

- **Be specific in your input** — the more context, the better the retrieval and generation
- **Read the rationale** — it teaches brand voice faster than any style guide
- **Use refinements** — iterating on a good initial result is faster than rewriting your prompt
- **Check cited guidelines** — these are the exact rules that apply to your use case

---

## 🆘 Support

Contact the development team or open an issue in the [source repository](https://github.com/TCGplayer/Electron_Content_Coach).
