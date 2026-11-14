# Publication Safety and Data Handling

This repository is intended to support learning and potentially a public professional portfolio.

## Never commit

- Employer or customer data, internal ticket details, unredacted screenshots or proprietary procedures.
- Real production architecture, internal network ranges, hostnames, URLs, asset identifiers or access details.
- Passwords, keys, tokens, `.env` files, certificates, secrets or session cookies.
- Real log data that could reveal customer data, usernames, infrastructure or incident patterns.
- Non-public training content reproduced without permission (write original summaries instead).

## Do instead

- Use personal lab systems, invented scenarios and synthetic incident records.
- Redact identifying details and verify screenshots **before** adding them to the repository.
- Use generic component labels such as `test-linux-vm`, `monitoring-platform` and `example.invalid`.
- Describe general skills learned at work without revealing protected workplace context.
- Cite and link to training sources rather than copying their course materials.

## Before every push

1. Run `git status` and review `git diff --staged`.
2. Search changed files for credentials, private hostnames, company/customer data and unintended attachments.
3. Confirm each result in a case study is actually observed, or label it **synthetic / example**.
4. If something sensitive was committed, stop publishing and follow the relevant incident / credential-rotation process; deleting a file from the latest commit may not remove it from Git history.
