<!--
  HOW TO USE THIS TEMPLATE
  These HTML comments are just for you — they don't show up when GitHub
  renders the markdown. Leave them in until you publish, or delete each one
  as you fill in that section.

  README content (headings, text) stays in English — it's the standard for a
  public GitHub repo, it reaches any recruiter/dev browsing your profile.
-->

# Project Name

<!--
  Direct title + one line right below saying WHAT the project does and FOR
  WHOM. Avoid generic phrases like "This is a project that...". Get straight
  to the point, in the same tone as: "<ProjectName> is a high-performance
  REST API for..."
-->
> One clear sentence: what it does, in what context, and the main technical differentiator (if any).

<div align="left">

<!--
  Badges always at the top, right below the tagline — they convey engineering
  maturity before anyone reads a single line. Use the SAME style across all
  your repos to build consistent visual identity between projects (that's
  what actually "catches the eye", not all-caps in the name):
  style=for-the-badge, same background color everywhere.
  Generate the real ones at https://shields.io — license, main language/
  framework(s), version, and "last commit" if the repo already has history.
  No CI set up yet? Swap the build badge for a static one instead of removing
  the line (e.g. "status: in development").
-->
[![License](https://img.shields.io/badge/License-MIT-1a1a2e?style=for-the-badge&logoColor=white)](LICENSE)
[![Language](https://img.shields.io/badge/Language-000000-1a1a2e?style=for-the-badge&logoColor=white)]()
[![Version](https://img.shields.io/badge/Version-1.0.0-1a1a2e?style=for-the-badge&logoColor=white)]()

</div>

<!--
  Collapsible ToC — use it in READMEs with 6+ sections; for a short README you
  can remove the whole block. Always use a relative anchor (#section), never
  an absolute URL: it works the same, stays cleaner in the source, and won't
  break if the repo is renamed/forked. Adjust the items to match the sections
  you actually use.
-->
<details>
<summary><strong>Table of Contents</strong></summary>

- [About](#about)
- [Demo](#demo)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Architecture & Design Decisions](#architecture--design-decisions)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [API Reference](#api-reference)
- [License](#license)
- [Author](#author)

</details>

---

## About

<!--
  This is the section that separates a junior README from a senior one.
  Don't just describe what the code does — explain the WHY:
  - What real problem does this solve?
  - Why did you decide to build this (from scratch, without lib X, with
    approach Y)?
  - What was the main technical challenge?
  2-4 sentences, no filler.
-->

---

## Demo

<!--
  If it's a CLI: a GIF or code block showing real input/output.
  If it's web/design: a screenshot or link to the deployment.
  If it's a lib: a code snippet showing usage.
  If it's an API: you can SKIP this section — the curl examples in "Usage"
  already fill that role (that's what the Generator API did). Don't force a
  redundant Demo.
-->

---

## Features

<!-- A table works better than bullets when each feature deserves a line of description -->
| Capability | Description |
|---|---|
| **Feature name** | What it does, one line |

---

## Tech Stack

<!-- List only what's relevant to understand technical decisions, not the whole package.json -->
- **Runtime/Language:**
- **Framework:**
- **Database/Storage:**
- **Key dependencies:**

---

## Architecture & Design Decisions

<!--
  This section is what separates senior level from junior the most. Cover, in
  this order:
  1. How the project is organized (folder tree + what each layer does)
  2. "Why this shape:" — why this organization, why this lib/framework
     instead of the obvious alternative, what each trade-off bought you
  3. "Known limitations:" — what you know is missing or fragile today.
     This isn't a weakness, it's a sign that you understand your own system.
-->

```
.
├── src/
│   ├── ...
├── tests/
└── README.md
```

**Why this shape:**

**Known limitations:**
-

---

## Getting Started

### Prerequisites

<!-- Exact versions, not "recent Node" -->
-

### Installation

```bash
git clone https://github.com/your-username/your-project.git
cd your-project
# install commands
```

### Environment Variables

<!-- If there's a .env, document each variable and its purpose. Never commit real values. -->
| Variable | Default | Description |
|---|---|---|
| `EXAMPLE_VAR` | — | What it controls |

### Running locally

```bash
# command to run
```

---

## Usage

<!--
  REAL, runnable examples, not pseudocode.
  - API: curl with request + response in JSON, one block per main endpoint
  - CLI: real commands with expected output
  - Lib: import + function call snippet
-->

```bash
# usage example
```

---

## API Reference

<!--
  Rename this section based on the project type:
  - API → "API Reference" (endpoint table + parameter table)
  - CLI → "Commands" (command table + flags)
  - Lib → "Public API" (exported functions/classes and signatures)
  If the project has relevant operational behavior (rate limiting, retry
  policy, exit codes), document it right after this section, with the
  behavior's own name as the title (e.g. "## Rate Limiting").
-->

| Method/Command | Description |
|---|---|

---

## License

Distributed under the **MIT License**.

---

## Author

<!-- Name + GitHub (and LinkedIn, if you want) — makes it easy for a recruiter to find you -->
**Your Name** — [GitHub](https://github.com/your-username)
