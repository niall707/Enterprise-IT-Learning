# Enterprise IT Learning

> **Building enterprise IT expertise through continuous learning, hands-on engineering, and real-world application across systems administration, automation, cloud infrastructure, and IT operations.**

A structured, evidence-led learning repository supporting progression into **Linux / RHEL L2 systems administration** and broader enterprise operations. It combines a **knowledge library** with a **professional portfolio**: not just courses completed, but concepts understood, labs performed and outcomes verified.

## Learning model: Knowledge → Practice → Evidence

| Layer | What belongs here | What it demonstrates |
|---|---|---|
| **Learn** | Course notes, reading, command references, key concepts | Technical understanding |
| **Practise** | Repeatable exercises on personally controlled systems | Hands-on application |
| **Demonstrate** | Lab reports, troubleshooting write-ups, sanitized case studies | Reasoning, verification and documentation |

**Evidence matters:** a note records *what I learned*; a lab documents *what I did*; a case study explains *why the work matters*.

## Learning streams

| # | Stream | Focus | Priority |
|---:|---|---|---|
| 01 | [Systems Administration](01-systems-administration/README.md) | RHEL, Linux, storage, networking, services, security | Primary |
| 02 | [Automation & Configuration](02-automation/README.md) | Ansible, Bash, Python | Primary |
| 03 | [Cloud & Infrastructure](03-cloud-infrastructure/README.md) | Cloud platforms and virtualisation | Supporting |
| 04 | [CI/CD & Deployment](04-cicd-deployment/README.md) | UrbanCode, pipelines, release management | Supporting |
| 05 | [Monitoring & Observability](05-monitoring-observability/README.md) | LogicMonitor, metrics, logging, alerts | High |
| 06 | [IT Service Management](06-itsm/README.md) | ServiceNow, incidents, problems, changes | High |
| 07 | [Knowledge Management](07-knowledge-management/README.md) | Confluence, SOPs, runbooks | Supporting |
| 08 | [AI & Enterprise Operations](08-ai-enterprise-operations/README.md) | AI-assisted operations, AIOps, governance | Exploratory |
| 09 | [Projects & Case Studies](09-projects-case-studies/README.md) | Verified labs and portfolio evidence | Portfolio |

## Start here

1. Read the [learning roadmap](LEARNING-ROADMAP.md) and the [Pluralsight course plan](learning-plans/pluralsight-enterprise-it-learning-plan.md).
2. Choose a course or practical question in one of the streams above.
3. Copy the relevant file from [templates](templates/README.md) into that stream.
4. Record the **source, learning objectives, commands, results and validation**.
5. Update the [progress tracker](PROGRESS-TRACKER.md), linking to the completed evidence.

### Learning priorities

- **Core L2:** RHEL service management, logs, storage, permissions, SELinux and networking.
- **Automation:** Ansible inventory, idempotency, playbook testing and configuration control.
- **Operational maturity:** Alert investigation, ServiceNow reporting and deployment failure analysis.
- **Supporting knowledge:** Cloud foundations, Confluence documentation, and governed enterprise AI.

## How progress is measured

Use clear states: **Planned → In progress → Completed → Validated**.

- **Completed** means the learning activity or course is finished.
- **Validated** means the exercise was reproduced and tested, with evidence recorded.
- Do not claim a certification, employment result, incident resolution or production implementation unless it actually occurred.

A practical lab may be more useful than a long note. Each completed lab should include a reproducible procedure, observed output, verification, and what did not work.

## Repository conventions

- Write in **Markdown**, with descriptive `kebab-case.md` filenames.
- Keep each topic in its relevant stream. Cross-link related topics rather than duplicate them.
- For terminal snippets, mark the language (`bash`, `yaml`, `powershell`, etc.).
- Include source links and the date reviewed for training materials that may change.
- Use ISO dates (`YYYY-MM-DD`) in evidence records.
- Put **personal lab deployments/configuration** in the relevant infrastructure project's repository; keep concepts, learning notes and portfolio summaries here.
- The course catalogue in this repository was prepared in November 2026; course durations and employer entitlements may change.

## Confidentiality and responsible publishing

This repository is suitable for a **public GitHub portfolio only when its content is sanitised**.

**Do not commit:** employer/customer data, internal ticket numbers, architecture diagrams, internal URLs/IPs, usernames, credentials, tokens, real operational logs, proprietary SOPs or screenshots containing workplace details. Use invented scenarios, synthetic datasets, or self-owned lab systems. Review [SECURITY.md](SECURITY.md) before publishing.

## Repository guides

- [Learning roadmap](LEARNING-ROADMAP.md)
- [Progress tracker](PROGRESS-TRACKER.md)
- [Pluralsight course plan](learning-plans/pluralsight-enterprise-it-learning-plan.md)
- [Templates and writing conventions](templates/README.md)
- [Content contribution workflow](CONTRIBUTING.md)
- [Local Git setup](QUICKSTART.md)
- [Publication safety](SECURITY.md)

---

*Status: initial framework. Subject areas and exercises are planned until actual learning and testing evidence is added.*
