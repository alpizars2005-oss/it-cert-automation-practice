# Agent development guide

This repository is certification and lab practice. Preserve the educational objective and keep solutions easy to inspect and explain.

## Workflow

1. Read `PLAN.md`, `README.md`, `docs/contributing.md`, and the specific course/lab files before editing.
2. Verify Python, Linux, systemd, cloud, and library behavior against current official documentation when needed; Context7 may assist with current docs.
3. Keep dependencies and abstractions minimal unless the lab explicitly requires them.
4. Preserve assignment semantics and expected inputs/outputs.
5. Run the existing Python checks and add focused tests only where they improve understanding or regression safety.
6. Treat sample external input defensively, but do not turn small certification labs into production frameworks.
7. Never commit credentials, cloud tokens, SSH keys, or machine-specific secrets.

## Review roles

For substantial labs, perform separate implementation and test/readability reviews. Add a security review when files, networking, services, or credentials are involved.

## Completion gate

A change is complete when the lab remains faithful to its exercise, existing checks pass, and the resulting code is simple enough to explain line by line.
