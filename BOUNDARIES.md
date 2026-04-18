# opensin-ai-code Boundaries

## Role
`opensin-ai-code` is the Python agent development surface in the OpenSIN-AI ecosystem.

Short version:

- **This repo = Python development surface for agent building and experimentation**
- **Not this repo = sole owner of the global runtime stack, product shell, or control-plane truth**

---

## Canonical Ownership

| Concern | Canonical Repo |
|---|---|
| Python agent development surface | `opensin-ai-code` |
| Free/open runtime core | `OpenSIN` |
| Rust CLI runtime surface | `opensin-ai-cli` |
| Product web app | `OpenSIN-WebApp` |
| Internal ops control plane | `ai-agent-system` |
| Official documentation | `OpenSIN-documentation` |

---

## This repo MUST own

- Python-first developer workflows
- Python agent scaffolding and development ergonomics
- Python-side abstractions specific to this repo’s package surface
- repo-local tests and docs for the Python development surface

---

## This repo MUST NOT own

- sole canonical ownership of all runtime primitives across the org
- product app behavior
- control-plane behavior
- official docs canon
- architecture SSOT

---

## Hard rules

### 1. Development surface, not global monopoly
This repo may provide a Python implementation surface, but it must not describe itself as the only authoritative owner of runtime concerns already owned elsewhere.

### 2. Scope claims must be repo-local
Feature descriptions should be explicit about whether they are repo-local, shared, mirrored, experimental, or aligned with another canonical runtime.

### 3. Product and ops boundaries stay out
Anything primarily about user-facing product UX or fleet operations belongs elsewhere.
