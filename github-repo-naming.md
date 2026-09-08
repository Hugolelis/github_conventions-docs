# GitHub repository naming convention

Format: `project-name-suffix`, in kebab-case, all lowercase.

## Suffixes — projects/products

| Suffix | Use |
|---|---|
| `-api` | REST or GraphQL backend |
| `-cli` | Command-line tool |
| `-service` | Microservice (when there are several within the same domain) |
| `-worker` | Asynchronous processing / background jobs |
| `-lib` | Reusable library/package, no standalone use |
| `-sdk` | Client for consuming your own API |
| `-infra` | Infrastructure as code (Terraform, Docker, k8s) |
| `-web` | Frontend, when kept in a repo separate from the backend |
| `-docs` | Documentation separate from the code |

## Suffixes — study and learning

| Suffix | Use |
|---|---|
| `-roadmap` | The plan itself: topic list, checklist, timeline. Plain markdown, no functional code (e.g. `backend-roadmap`) |
| `-study` | Code and notes while learning a specific topic, without becoming a project with its own purpose (e.g. `sql-study`, `docker-study`) |
| `-exercises` (or `-katas`) | Solving practical challenges/exercises from a platform (e.g. `algorithms-exercises`, `leetcode-katas`) |
| `-course` | Repo that follows a specific course (e.g. `rocketseat-nodejs-course`) |

Rule to avoid confusing `-study` with `-exercises`: if you're writing code to internalize a concept (implementing something, trying out a lib), it's `-study`; if you're solving closed-ended problems from a platform, it's `-exercises`.

## Practical rules

- Suffix always in English, even when the project name is in another language.
- Only use a suffix when the project has more than one "face" (e.g. if only an API exists and there's never going to be a CLI/web, it can stay without a suffix).
- Don't mix a type suffix (`-api`) with a technology suffix (`-node`, `-go`) — pick one, not both.
- Services within the same domain: prefer a monorepo with folders (`/api`, `/worker`) over multiplying repositories.
- Always lowercase, even for suffixes that "deserve emphasis" (e.g. `-cli`, not `-CLI`) — uppercase breaks convention with the ecosystem (npm, Docker Hub, PyPI don't accept it or normalize it), can cause case-sensitivity issues across OSes, and doesn't help visibility. Visual emphasis belongs in the README, repo description, and topics, not in the name.

## How to decide the suffix when it's unclear

Ask what the project's real "face" is — how it will be consumed:

- Implements a core logic/algorithm that other parts will import → `-lib` (the engine of the project)
- Runs in the terminal → `-cli`
- Is consumed via HTTP requests → `-api`

When the project will eventually gain multiple faces (e.g. an algorithm that later becomes a CLI and an API), start with `-lib` — it's the core the others depend on. If you don't yet know which faces it will have, keep everything in a single repo without a suffix, with folders (`/lib`, `/cli`, `/api`), and only split into separate repositories once each part stabilizes.

## Examples

- `task-manager-api`
- `task-manager-cli`
- `task-manager-worker`
- `auth-service`
- `billing-service`
- `qrcode-lib` (encoding algorithm built from scratch) → later `qrcode-cli` and/or `qrcode-api` as layers on top
- `backend-roadmap`
- `sql-study`
- `algorithms-exercises`
