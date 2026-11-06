# GitHub Conventions Docs

> Personal collection of GitHub conventions and templates (commit message format, changelog structure, repository naming, and a README template) kept consistent across every project.

<div align="left">

[![Status](https://img.shields.io/badge/Status-Active-407a50?style=for-the-badge&labelColor=1a1a1a&logoColor=white)]()

</div>

<details>
<summary><strong>Table of Contents</strong></summary>

- [About](#about)
- [Contents](#contents)
- [How to Use](#how-to-use)
- [Author](#author)

</details>

---

## About

Every new project starts with the same small decisions (how to name the repo, how to format commits, how to structure a changelog, what a good README looks like) and re-deciding them each time wastes effort and drifts inconsistent over time. This repo is the single source of truth for those decisions: each file documents one convention in full, so it can be read on its own or copied straight into a new project.

---

## Contents

| File | Convention |
|---|---|
| [commits.md](commits.md) | Commit message format, based on Conventional Commits |
| [changelog_template.md](changelog_template.md) | `CHANGELOG.md` template, based on Keep a Changelog + Semantic Versioning |
| [github-repo-naming.md](github-repo-naming.md) | Repository naming and suffix convention (`-api`, `-cli`, `-lib`, etc.) |
| [readme_template.md](readme_template.md) | `README.md` template for new projects |

---

## How to Use

Each file is self-contained and includes its own guidance as HTML comments (visible in the raw markdown, hidden when rendered on GitHub). To start a new project:

```bash
# copy the README template into a new project
cp readme_template.md ../your-project/README.md

# copy the changelog template into a new project
cp changelog_template.md ../your-project/CHANGELOG.md
```

Then follow [github-repo-naming.md](github-repo-naming.md) to name the repository and [commits.md](commits.md) for every commit message going forward.

---

## Author

[Hugolelis](https://github.com/Hugolelis)
