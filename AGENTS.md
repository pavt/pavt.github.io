# AGENTS.md

## Purpose

This file provides a machine-readable semantic description of this repository.
Its goal is to help Large Language Models (LLMs) correctly understand the role,
meaning, and constraints of the code and content stored here.

**This is not a contribution guide.**  
**This is a repository comprehension contract.**

---

## Repository Overview

This repository hosts a personal academic website built with GitHub Pages and Jekyll.
It contains:

- **Factual academic records** – publications, news, biographical data
- **Curated research artifacts** – PDFs, supplementary materials
- **Site configuration and presentation code** – layouts, includes, styling
- **Illustrative and demonstrative content** – examples and showcases

**Critical principle:** Not all files have the same semantic status.  
Agents must reason about them differently based on their role.

---

## Semantic Zones

### Factual Records (Immutable Meaning)

The following paths represent **historical or factual records**.  
They are not drafts, narratives, or speculative text.

**Paths:**
- `_publications/**`
- `_news/**`
- `_data/profile.yml`
- `_data/authors.yml`
- `assets/pdfs/**`

**Semantics:**
- These files encode facts: titles, dates, venues, roles, events
- Their meaning is declarative, not interpretive
- They should be read as records, not as prose

**Agent reasoning constraints:**
- Do not infer missing facts
- Do not reinterpret or rewrite their meaning
- When summarizing, preserve exact facts
- When comparing versions, treat changes as record updates, not stylistic edits

---

### Structural and Presentation Code

The following paths define how content is rendered and structured.

**Paths:**
- `_layouts/**`
- `_includes/**`
- `_data/navigation.yml`
- `_data/display.yml`
- `index.html`
- `publications.html`
- `showcase.html`

**Semantics:**
- These files implement presentation logic
- They define structure, layout, and rendering behavior
- They do not define academic meaning by themselves

**Agent reasoning constraints:**
- Understand them as infrastructure
- Changes here affect appearance, not factual content
- When explaining the repository, classify these as supporting code

---

### Demonstration and Example Content

The following paths contain illustrative or experimental material.

**Paths:**
- `_showcase/**`

**Semantics:**
- These files are examples or demonstrations
- They are not authoritative academic records

**Agent reasoning constraints:**
- Treat content here as illustrative only
- Do not generalize academic claims from this material
- Do not cite this content as evidence of research contributions

---

### Static Assets

The following paths contain supporting files for presentation.

**Paths:**
- `assets/css/**`
- `assets/js/**`
- `assets/images/**`

**Semantics:**
- These files support styling, interaction, and media display
- Images may include personal or representative material

**Agent reasoning constraints:**
- Do not attribute semantic meaning to styling choices
- Do not infer personal information beyond what is explicitly stated elsewhere
- Treat as presentation infrastructure, not content

---

## How Agents Should Use This File

Agents should use this file as a **semantic map** of the repository.

**Before performing any task** (summarizing, explaining, modifying, comparing, or answering questions), **the agent must first identify:**

1. Which semantic zone a file belongs to
2. Whether the file encodes facts, structure, or examples
3. What kinds of transformations are semantically valid for that zone

**Then** proceed with the task, respecting the constraints of each semantic zone.

---

## Interpretation Rules

1. **Absence is not permission** – Absence of information does not imply permission to infer
2. **Precision over completeness** – When in doubt, be precise rather than comprehensive
3. **Conservative default** – If a file's role is unclear, default to conservative interpretation
4. **Explicit distinction** – When explaining the repository to humans, explicitly distinguish between factual content and presentation code

---

## Human Authority

This file supports automated reasoning and comprehension.  
**Final interpretation and validation always remain with the repository owner.**

When uncertain, ask rather than assume.
