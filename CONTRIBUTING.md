# Content Workflow

This is a personal learning repository, but it follows a lightweight enterprise documentation workflow.

## Create

1. Pick the appropriate stream and subtopic.
2. Start from a template in [`templates/`](templates/README.md).
3. State the learning question or lab objective before the procedure.
4. Record source references, dates and what was genuinely observed.

## Review

- **Accuracy:** commands and assumptions are correct for the tested operating system/version.
- **Reproducibility:** another person could follow the procedure in an equivalent test lab.
- **Verification:** there is evidence of success or failure, not just a claimed outcome.
- **Safety:** all example data is synthetic or suitable for publication.
- **Clarity:** headings, command blocks and rollback steps are easy to scan.

## Publish

- Use focused commits, for example `docs(rhel): add systemd troubleshooting lab`.
- Keep incomplete work labelled **Draft**; do not present placeholders as completed experience.
- Cross-link new lab or case-study files from [`PROGRESS-TRACKER.md`](PROGRESS-TRACKER.md).
