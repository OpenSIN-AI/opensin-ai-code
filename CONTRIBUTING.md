# Contributing

## Boundary Rules

Before adding a feature description, package, or top-level claim, answer:

1. Is this repo implementing a Python development surface, or claiming global runtime ownership?
2. Does another OpenSIN repo already own the canonical form of this concern?
3. Should the README/docs describe alignment rather than sole ownership?

### Put it in `opensin-ai-code` if:
- it improves the Python development surface
- it adds Python-side tooling, tests, or package-local abstractions
- it documents repo-local capabilities clearly

### Do NOT put it in `opensin-ai-code` if:
- it claims product or control-plane ownership
- it implies this repo alone owns the full runtime stack
- it duplicates official docs canon
