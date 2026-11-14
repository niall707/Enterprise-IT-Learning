# Pluralsight Learning Plan — Enterprise IT & Systems Administration

**Prepared:** 14 November 2026  
**Focus:** Progression from Systems Support L1 into RHEL L2 Systems Administration  
**Platform:** Pluralsight (work-provided access)

## Purpose

A practical learning programme covering seven areas:

1. RHEL system administration
2. Ansible and cloud automation
3. IBM UrbanCode
4. LogicMonitor
5. AI and enterprise IT
6. Confluence
7. ServiceNow

Courses are grouped by estimated viewing time:

- **Short:** Under 2 hours
- **Medium:** 2–5 hours
- **Long:** Over 5 hours (including multi-course learning paths)

> **Note:** Durations are approximate published video/path times and exclude labs, exercises and revision. Course availability may depend on the Pluralsight libraries included in your employer's subscription. UrbanCode and LogicMonitor recommendations include transferable Pluralsight material and official vendor resources where dedicated Pluralsight training could not be verified.

---

## 1. RHEL System Administration

**Priority: 1 — Primary career focus**

| Level | Course / path | Duration | Link |
|---|---|---:|---|
| Short | RHCSA: Managing Software | 1h 7m | [Open course](https://www.pluralsight.com/courses/rhcsa-ex200-managing-software) |
| Medium | RHCSA: Creating and Configuring File Systems | 2h 51m | [Open course](https://www.pluralsight.com/courses/rhcsa-ex200-creating-configuring-file-systems) |
| Long | RHCSA EX200 Learning Path | ~20h | [Open learning path](https://www.pluralsight.com/paths/rhcsa-red-hat-certified-system-administrator-ex200-new) |

**Additional recommended course:** [RHCSA: Operating Running Systems](https://www.pluralsight.com/courses/rhcsa-ex200-operating-running-systems) — 1h 50m.

**Focus areas**

- systemd services and service failures
- journald and log investigation
- Software packages and patching
- Filesystems, storage and permissions
- SELinux, networking and troubleshooting

**Practical evidence:** Document a Linux alert investigation and resolution in Project Hearth, including commands, findings and verification.

## 2. Ansible and Cloud Automation

**Priority: 2 — Enterprise automation**

| Level | Course / path | Duration | Link |
|---|---|---:|---|
| Short | Ansible Environment Configuration (module in the Ansible path) | ~52m | [Open path](https://www.pluralsight.com/paths/ansible) |
| Medium | Ansible for Enterprise Automation | 2h 16m | [Open course](https://www.pluralsight.com/courses/ansible-enterprise-automation) |
| Long | Ansible Learning Path | ~19h | [Open path](https://www.pluralsight.com/paths/ansible) |

**Cloud-specific option:** [Automating Multi-vendor and Cloud Networks Using Ansible](https://www.pluralsight.com/courses/ansible-automating-multi-vendor-cloud-networks) — ~1h 23m.

**Focus areas**

- Inventory, variables and roles
- Idempotent playbooks and error handling
- SSH access, secrets and permissions
- Linux patching and configuration drift
- Repeatable automation with audit-friendly reports

**Practical evidence:** Build a Project Hearth playbook that patches Debian VMs, checks key services, and outputs an execution report. Keep production and homelab credentials separate.

## 3. IBM UrbanCode

**Priority: 4 — Deployment and release management**

A dedicated UrbanCode Deploy course could not be verified in Pluralsight; the following cover transferable CI/CD and release concepts.

| Level | Course / path | Duration | Link |
|---|---|---:|---|
| Short | DevOps Foundations: CI/CD | ~1h | [Open course](https://www.pluralsight.com/courses/devops-foundations-continuous-integration-continuous-delivery) |
| Medium | Continuous Delivery: Release Pipelines | 2h 1m | [Open course](https://www.pluralsight.com/courses/azure-devops-continuous-delivery-release-pipelines) |
| Long | CI/CD Tools Learning Path | ~11h | [Open path](https://www.pluralsight.com/paths/continuous-integration-and-continuous-delivery-cicd-tools) |

**Vendor-specific supplement:** [IBM — DevOps for IBM zSystems CI/CD Enablement: Deployment Specialist](https://www.ibm.com/training/course/devops-for-ibm-zsystems-cicd-enablement-deployment-specialist-DL007127G) — ~5h; verify that its zSystems focus matches your environment.

**Focus areas**

- Deployment agents and environments
- Pipeline stages and approvals
- Release failure investigation
- Rollback strategy and change control

**Practical evidence:** Produce a generic deployment workflow/runbook mapping stages, approval gates, failure points and rollback.

## 4. LogicMonitor

**Priority: 3 — Monitoring and alert investigation**

A dedicated LogicMonitor course could not be verified in Pluralsight. These options cover observability concepts useful with LogicMonitor.

| Level | Course / path | Duration | Link |
|---|---|---:|---|
| Short | Continuous Monitoring: The Big Picture | 49m | [Open course](https://www.pluralsight.com/courses/continuous-monitoring-big-picture-2022) |
| Medium | SRE: Monitoring and Observability | 2h 17m | [Open course](https://www.pluralsight.com/courses/sre-monitoring-observability) |
| Long | Observability and Monitoring Tools and Techniques | ~66h (select modules) | [Open path](https://www.pluralsight.com/paths/observability-and-monitoring-tools-and-techniques) |

**Vendor-specific supplement:** [LogicMonitor Academy / Customer Education](https://www.logicmonitor.com/customer-education) — product-specific training for collectors, dashboards, logs and AIOps. Durations vary.

**Focus areas**

- Alert thresholds and tuning
- Distinguishing transient from persistent alerts
- Device and service metrics
- Collector health and data quality
- Incident correlation and escalation

**Practical evidence:** Create a monitoring investigation case study based on recurring transient log alerts, with frequency, impact, probable cause and proposed threshold changes.

## 5. AI and Enterprise IT

**Priority: 5 — AI-assisted IT operations**

| Level | Course / path | Duration | Link |
|---|---|---:|---|
| Short | Practical Applications of Generative AI in DevOps | 19m | [Open course](https://www.pluralsight.com/courses/practical-applications-generative-ai-devops) |
| Medium | Safety and Security Architecture for GenAI Systems | 2h 7m | [Open course](https://www.pluralsight.com/courses/safety-security-architecture-gen-ai-systems) |
| Long | Generative AI for IT Pros | ~5h | [Open path](https://www.pluralsight.com/paths/generative-ai-for-it-pros) |

**Additional course:** [Integrating AI Agents with ServiceNow](https://www.pluralsight.com/courses/integrating-ai-agents-servicenow) — ~1h 30m.

**Focus areas**

- AI-assisted log triage and troubleshooting
- Incident summarisation and ticket classification
- Human-in-the-loop approval and auditability
- Data confidentiality and enterprise security controls

**Practical evidence:** Design an AI-assisted incident triage workflow using *synthetic or authorised* sample logs. Never upload confidential company data to unapproved AI systems.

## 6. Confluence

**Priority: 7 — Documentation and knowledge management**

| Level | Course / path | Duration | Link |
|---|---|---:|---|
| Short | Confluence Foundations | 55m | [Open course](https://www.pluralsight.com/courses/confluence-foundations) |
| Medium | Confluence: Getting Started | 2h 14m | [Open course](https://www.pluralsight.com/courses/confluence-getting-started) |
| Long | Confluence Learning Path + Site Administration | ~5h 38m combined | [Learning path](https://www.pluralsight.com/paths/confluence) · [Administration course](https://www.pluralsight.com/courses/site-administration-confluence-cloud) |

**Focus areas**

- Spaces, pages and permissions
- Reusable operational documentation templates
- Runbook organisation and change history
- Incident postmortems and service knowledge bases

**Practical evidence:** Draft templates for an incident investigation, change record, deployment runbook and operating procedure.

## 7. ServiceNow

**Priority: 6 — ITSM and operational reporting**

| Level | Course / path | Duration | Link |
|---|---|---:|---|
| Short | Reporting and Dashboards Using Data-driven Insights | 1h 33m | [Open course](https://www.pluralsight.com/courses/reporting-dashboards-data-driven-insights) |
| Medium | Platform Administration Essentials and Automation Introduction | 2h 8m | [Open course](https://www.pluralsight.com/courses/platform-administration-essentials-automation-introduction) |
| Long | ServiceNow Fundamentals Learning Path | ~18h | [Open path](https://www.pluralsight.com/paths/servicenow-fundamentals) |

**Focus areas**

- Incident and request lifecycles
- Reports and trend dashboards
- SLAs, escalations and assignment groups
- Workflow and approval controls
- Data quality for actionable operational reporting

**Practical evidence:** Develop a report specification for recurring Linux alerts, including time range, filters, trend metrics and recommended operational action.

---

## Seven-week starter programme

Complete one course in each subject before committing to the longer paths.

| Week | Subject | Starter course | Viewing time | Complete |
|---|---|---|---:|:---:|
| 1 | RHEL | Operating Running Systems | 1h 50m | [ ] |
| 2 | Ansible | Ansible for Enterprise Automation | 2h 16m | [ ] |
| 3 | LogicMonitor | SRE: Monitoring and Observability | 2h 17m | [ ] |
| 4 | ServiceNow | Reporting and Dashboards | 1h 33m | [ ] |
| 5 | UrbanCode | DevOps Foundations: CI/CD | 1h | [ ] |
| 6 | Confluence | Confluence Foundations | 55m | [ ] |
| 7 | AI | Integrating AI Agents with ServiceNow | 1h 30m | [ ] |

**Total video time: 11h 21m**, plus exercises and practice.

## After the starter programme

1. **RHCSA EX200 (~20h):** Prioritise Linux operating systems, services, storage, security and troubleshooting.
2. **Ansible (~19h):** Move from executing established automation to authoring, debugging and maintaining playbooks.
3. **LogicMonitor + ServiceNow:** Build a stronger end-to-end view from alert generation to incident reporting.
4. **UrbanCode:** Develop confidence in deployment workflows, failures and rollbacks.
5. **AI + Confluence:** Improve documentation quality and adopt controlled AI-assisted operations.

## Learning evidence log

Copy this template after completing each course.

```markdown
### Course: [Course title]
- Date completed: YYYY-MM-DD
- Duration: 
- URL: 
- Main concepts learned:
  - 
  - 
  - 
- Work relevance:
- Homelab / practical exercise:
- Evidence link (GitHub, Markdown, screenshots):
- Follow-up questions:
```

## Suggested GitHub organisation

```text
enterprise-it-learning/
├── README.md
├── rhel/
├── ansible/
├── urbancode-cicd/
├── logicmonitor-observability/
├── ai-enterprise-it/
├── confluence-documentation/
└── servicenow-itsm/
```

Keep employer-specific architecture, customer information, credentials and internal operational data out of public repositories. Use sanitised or homelab examples for portfolio evidence.
