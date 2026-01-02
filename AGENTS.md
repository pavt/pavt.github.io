# AGENTS.md

## Purpose

This file provides a machine-readable semantic description of this repository.
Its goal is to help Large Language Models (LLMs) correctly understand the role,
meaning, and constraints of the code and content stored here.

This file is not a contribution guide.
It is a **repository comprehension contract**.

---

## Repository Overview

This repository hosts a personal academic website built with GitHub Pages and Jekyll.
It contains a mix of:

- factual academic records
- curated research artifacts
- site configuration and presentation code
- illustrative and demonstrative content

Not all files have the same semantic status.
Agents must reason about them differently.

---

## Semantic Zones

### Factual Records (Immutable Meaning)

The following paths represent **historical or factual records**.
They are not drafts, narratives, or speculative text.

- `_publications/**`
- `_news/**`
- `_data/profile.yml`
- `_data/authors.yml`
- `assets/pdfs/**`

Semantics:
- These files encode facts (titles, dates, venues, roles, events).
- Their meaning is declarative, not interpretive.
- They should be read as records, not as prose.

Agent reasoning constraints:
- Do not infer missing facts.
- Do not reinterpret or rewrite their meaning.
- When summarizing, preserve exact facts.
- When comparing versions, treat changes as record updates, not stylistic edits.

---

### Structural and Presentation Code

The following paths define how content is rendered and structured:

- `_layouts/**`
- `_includes/**`
- `_data/navigation.yml`
- `_data/display.yml`
- `index.html`
- `publications.html`
- `showcase.html`

Semantics:
- These files implement presentation logic.
- They define structure, layout, and rendering behavior.
- They do not define academic meaning by themselves.

Agent reasoning constraints:
- Understand them as infrastructure.
- Changes here affect appearance, not factual content.
- When explaining the repository, classify these as supporting code.

---

### Demonstration and Example Content

The following paths contain illustrative or experimental material:

- `_showcase/**`

Semantics:
- These files are examples or demonstrations.
- They are not authoritative academic records.

Agent reasoning constraints:
- Treat content here as illustrative.
- Do not generalize academic claims from this material.

---

### Static Assets

- `assets/css/**`
- `assets/js/**`
- `assets/images/**`

Semantics:
- These files support styling, interaction, and media display.
- Images may include personal or representative material.

Agent reasoning constraints:
- Do not attribute semantic meaning to styling.
- Do not infer personal information beyond what is explicitly stated elsewhere.

---

## How Agents Should Use This File

Agents should use this file as a **semantic map** of the repository.

Before performing tasks such as:
- summarizing the repository
- explaining its structure
- proposing modifications
- comparing versions
- answering questions about its content

the agent should first identify:
- which semantic zone a file belongs to
- whether the file encodes facts, structure, or examples
- what kinds of transformations are semantically valid

---

## Interpretation Rules

- Absence of information does not imply permission to infer.
- Precision is preferred over completeness.
- If a file’s role is unclear, default to conservative interpretation.
- When explaining the repository to humans, explicitly distinguish
  between factual content and presentation code.

---

## Human Authority

This file supports automated reasoning and comprehension.
Final interpretation and validation always remain with the repository owner.
