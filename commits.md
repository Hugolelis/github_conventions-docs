# Commit convention

Based on [Conventional Commits](https://www.conventionalcommits.org/) — market standard, compatible with automatic changelog generation and tools like semantic-release/commitlint.

## Format

```
<type>(<optional scope>): <description>

[optional body]

[optional footer]
```

## Types

| Type | Use |
|---|---|
| `feat` | New feature |
| `fix` | Bug fix |
| `docs` | Documentation only (README, comments) |
| `refactor` | Changes code structure without changing behavior |
| `test` | Adds or fixes tests |
| `chore` | Maintenance that doesn't touch production code (deps, configs) |
| `perf` | Performance improvement |
| `build` | Build system or external dependencies |
| `ci` | CI pipelines/scripts |
| `revert` | Reverts a previous commit |

## Rules

- Description in the imperative, lowercase, no trailing period: `add cpf validation`, not `Added CPF validation.`
- Scope in parentheses indicates the affected module — optional, but helps filter history later (e.g. `feat(auth): ...`)
- Breaking change: `!` right after type/scope (`feat(api)!: remove legacy endpoint`) or footer `BREAKING CHANGE: description`
- Body explains the *why*, not the *how* — the diff already shows the how
- Footer to reference issues: `Closes #12`
- Messages always in English, even with scope/context in another language — same reason as the README: it's what any recruiter or collaborator expects to see in the history

## Examples

```
feat(cpf): add cpf validation endpoint
fix(short-url): handle duplicate short codes on collision
docs(readme): document rate limiting behavior
refactor(controllers): extract error handling into middleware
chore(deps): bump fastify to v5.1.0
test(uuid): add unit tests for uuid generator
feat(encoder)!: change matrix output format to support version 40
```

## Automation (optional)

To enforce the standard automatically: `commitlint` + a `husky` hook, blocking the commit if the message doesn't follow the format. A sign of engineering discipline, useful once the project grows or has more than one contributor.
