# Google IT Automation with Python — Practice Repository

Personal practice repository for labs and exercises completed while working through the **Google IT Automation with Python Professional Certificate**.

This repository is a learning record, not an unofficial redistribution of the course. It keeps the small lab artifacts close to their original structure so the progression from scripting to Git, services, and automation remains visible.

## Repository map

| Path | Focus | Included artifact |
| --- | --- | --- |
| `Course3/Lab4/` | Python validation and debugging | `validations.py` |
| `Course4/Lab4/` | Data/files practice | `employees-with-date.csv` |
| `Course5/Lab3/` | Cloud/service automation | `hello_cloud.py`, `hello_cloud.service` |
| `docs/` | Repository contribution notes | `contributing.md` |

## Automated checks

GitHub Actions performs a syntax compilation check for every tracked Python practice file on Python 3.11 and 3.13. The check deliberately **does not execute** labs that may expect a particular operating system, service manager, network environment, or course sandbox.

Run the same core check locally from the repository root:

```bash
python -m py_compile Course3/Lab4/validations.py Course5/Lab3/hello_cloud.py
```

## Why the original structure is preserved

Course exercises are useful evidence of learning precisely because they show the constraints and techniques practiced at that point in time. Files are therefore not mass-refactored into a single application or modern package layout merely for presentation.

Repository-wide improvements are limited to documentation, CI, contribution hygiene, and clearly justified corrections.

## Pull requests

A maintenance workflow marks pull requests stale only after 60 days of inactivity and closes them after an additional 14 days. Any new activity removes the stale state. The workflow runs daily rather than hourly because this is a small learning repository.

## License and course materials

See `LICENSE` for repository licensing. Course names and trademarks belong to their respective owners. Only practice artifacts tracked in this repository are covered by this project; access to original lessons, quizzes, instructions, and graded environments remains subject to the course provider's terms.
