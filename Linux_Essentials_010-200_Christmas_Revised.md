# Linux Essentials 010-200 — Six-Week Learning Plan (Christmas Break Included)

> **Learning track:** Enterprise IT Learning → Linux System Administration → Certifications  
> **Start:** Monday, 16 November 2026  
> **Christmas break:** Wednesday, 23 December 2026 – Friday, 1 January 2027 (inclusive)  
> **Target readiness review:** Sunday, 10 January 2027  
> **Suggested exam window:** 11–17 January 2027 (subject to voucher and booking availability)  
> **Weekly commitment:** approximately 4–5 hours  
> **Resources:** Pluralsight (work access), LPI exam objectives, isolated Project Hearth lab  
> **Status:** Provisionally targeting **010-200 (Version 2.0)** — confirm at voucher redemption / exam registration

## 1. Certification target — Linux Essentials 010-200 (Version 2.0)

**Working assumption:** Prepare for **010-200** while the voucher is pending. Confirm the exact exam version in the booking / Pearson VUE registration before choosing final mock examinations. A voucher purchase or receipt may not itself show which version will be scheduled.

- **Current exam:** Linux Essentials **010-200**, launched **15 October 2026**.
- **Previous exam:** 010-160 remains available until April 2027, so it is important to verify the booking.
- **Format:** 40 questions in 60 minutes.
- **Primary source of truth:** [LPI 010-200 official exam objectives](https://www.lpi.org/our-certifications/exam-010-objectives/).
- **Official study guide and exercises:** [LPI Linux Essentials 010-200 Learning Materials](https://learning.lpi.org/en/learning-materials/010-200/).
- **Pluralsight course path:** [LPI Linux Essentials (010-160)](https://www.pluralsight.com/paths/lpi-linux-essentials-010-160) — use for common foundational knowledge; it is **not** the definitive 010-200 syllabus.

**Study rule:** For every topic, cross-check the Pluralsight lesson with the 010-200 objective and the corresponding official LPI learning chapter. Give extra attention to modern areas added/updated in Version 2.0: `systemctl`, `journalctl`, `ip`/`ss`, SSH/SSH keys, Bash `if` statements, current distributions and open-source applications, and cloud / remote administration concepts.

## 2. Learning strategy

Work in the cycle **Watch → Practise → Explain → Document → Test**.

1. **Watch:** Cover a focused Pluralsight module, not a marathon of videos.
2. **Practise:** Perform the command or task on a disposable Linux VM.
3. **Explain:** State what the command does, when to use it and what its output means.
4. **Document:** Add a short lab record and screenshots/output to the GitHub learning repository. Remove credentials, internal company information and sensitive IPs or tokens.
5. **Test:** Answer questions without notes and track weak areas.

**Time split:** approximately 40% Pluralsight, 45% lab work, 15% recall and practice questions.

### Suggested weekly timetable

| Day | Suggested work | Duration |
|---|---|---:|
| Thursday | Pluralsight lessons | 45 min |
| Friday | Hands-on lab | 45 min |
| Saturday | Additional lessons / flashcards | 45 min |
| Sunday | Hands-on lab / objective drill | 45 min |
| Monday | Review, notes and quiz | 90 min |
| Tuesday–Wednesday | Free / optional only | — |

The sessions are flexible: this pattern allows study **before the 16:00 work shift**, without allocating fixed study work to Tuesday and Wednesday. A missed session should roll into the following week rather than displacing rest or personal time.

**Christmas exception:** Do not schedule anything from **23 December 2026 through 1 January 2027 inclusive**. The regular timetable resumes **Monday, 4 January**. The days **21–22 December** and **2–3 January** are catch-up/rest buffers, not required study sessions.

## 3. Pluralsight course shortlist

### Core Pluralsight path — use alongside the official 010-200 guide

[**LPI Linux Essentials (010-160)**](https://www.pluralsight.com/paths/lpi-linux-essentials-010-160) — published catalogue describes **4 courses, 3 labs, about 8 hours and a practice exam**.

- [ ] **Introduction to the Linux Essentials 010-160 Exam** — David Clinton, 9 min
- [ ] **Getting Started with Linux** — David Clinton, 1h 44m
- [ ] **Get Started with Linux** — guided lab, 1h
- [ ] [**Getting Started with the Linux Command Line**](https://www.pluralsight.com/courses/linux-command-line-getting-started-cert) — David Clinton, 1h 3m
- [ ] **Use Basic Commands for the Linux Command Line** — guided lab, 1h 15m
- [ ] [**Getting Started with Linux System Administration**](https://www.pluralsight.com/courses/linux-system-administration-getting-started-cert) — David Clinton, 1h 7m
- [ ] **Perform Basic Linux System Administration** — guided lab, 1h 15m
- [ ] **Pluralsight practice exam** — confirm that the version matches the booked exam

### Modern supplements — targeted lessons, not all courses

- [**Linux Fundamentals**](https://www.pluralsight.com/paths/linux-fundamentals-1): *Mastering the Command Line Interface (CLI)*, *System Management and File Security*, and *Networking, Packages, and Automation Basics*. Use for additional current command-line, process, permissions and network practice.
- [**Shell Scripting with Bash**](https://www.pluralsight.com/paths/using-bash-and-z-shell): *Bash Script Flow and Basic Utilities* (53m), *Bash Input/Output and Streams* (51m), plus its *Basic Bash Scripting & Arguments* lab. Concentrate on variables, arguments, `if`, loops, shebang, exit status and redirection.
- [**User, Group, and Permission Management in Ubuntu Linux**](https://www.pluralsight.com/courses/ubuntu-linux-user-group-permission-management) (1h 29m): useful selected modules on users, groups, `sudo` and ownership.

**Access note:** Catalogue content is verified publicly, but which courses/labs are enabled in your employer's Pluralsight subscription must be checked when signed in.

## 4. Project Hearth study environment

Create **`hearth-learn01`**, an isolated, disposable Debian 13 Linux VM on Proxmox. If suitable, clone the powered-off Debian golden image `hearth-vm01` (VMID 100), assign the clone its own hostname and identity, and verify the VM's MAC/IP/SSH host keys are unique. Do not modify the golden image itself.

**Resource-conscious starting point:** 1–2 vCPU, 1–2 GB RAM, ballooning where appropriate, and modest storage. Check host memory availability before running it, especially until the planned RAM upgrade is fully confirmed and installed. Shut the lab VM down when not in use.

**Safety boundaries**

- Never do exam exercises on `hearth-pve01` (the hypervisor host).
- Avoid manipulating production Docker, Home Assistant, Music Assistant, AdGuard or database services.
- Use test files under `~/linux-essentials-labs` and test users/groups only on the disposable VM.
- Snapshot the disposable VM before user/service/security exercises.
- A Debian VM is sufficient for the vendor-neutral exam. RHEL command comparisons are a *career extension*, not a substitute for exam coverage.

Suggested initial checks:

```bash
cat /etc/os-release
uname -r
whoami
pwd
ip -brief address
free -h
```

## 5. Six active study weeks — with a Christmas break

| Phase | Dates | Focus | Status |
|---|---|---|---|
| Week 1 | 16–22 Nov 2026 | Linux landscape and open source | Scheduled |
| Week 2 | 23–29 Nov 2026 | Command line and files | Scheduled |
| Week 3 | 30 Nov–6 Dec 2026 | Text processing and archives | Scheduled |
| Week 4 | 7–13 Dec 2026 | Bash scripting | Scheduled |
| Week 5 | 14–20 Dec 2026 | Processes, logs and networking | Scheduled |
| Buffer | 21–22 Dec 2026 | Rest or optional catch-up only | Optional |
| **Christmas break** | **23 Dec 2026–1 Jan 2027** | **No lessons, labs, quizzes or revision** | **Protected break** |
| Buffer | 2–3 Jan 2027 | Rest or gentle restart only | Optional |
| Week 6 | 4–10 Jan 2027 | Security, permissions and structured review | Scheduled |
| Exam readiness | 11–17 Jan 2027 | Mock exam, corrections and exam when ready | Conditional |

The study plan contains six teaching weeks, not six consecutive calendar weeks. This avoids rushing security and permissions work before Christmas.

### Week 1 — 16–22 November: Linux landscape and open source

**LPI 2.0 objective group:** 011 — The Linux Operating System and Open Source Software.

**Pluralsight:** exam introduction + *Getting Started with Linux*; complete the introductory Linux lab if available. **Official LPI 010-200:** Topic 011.

**Learn:** kernel vs distribution; Debian/Ubuntu vs RHEL/Fedora/Rocky/AlmaLinux vs SUSE; stable/LTS/rolling releases; repositories and package managers (`apt`, `dnf`, `zypper`); open-source licenses (GPL, BSD, Creative Commons); desktop/server and cloud/virtualization roles.

**Lab:** create `hearth-learn01`; run `cat /etc/os-release`, `uname -a`, `hostnamectl`, `type`, `which` or `command -v`; compare a Debian package command with the RHEL equivalent in notes.

**Deliverable:** `week-01-linux-foundations.md` containing a distribution comparison table and lab evidence.

**Checkpoint:** Explain kernel, shell, distribution, package manager and open-source licensing without notes.

- [ ] Complete lessons
- [ ] Run lab commands
- [ ] Commit notes
- [ ] Self-test

### Week 2 — 23–29 November: Command line and files

**LPI 2.0 objective group:** 012 — Command Line Basics.

**Pluralsight:** *Getting Started with the Linux Command Line* + the corresponding command-line lab. Use *Mastering the Command Line Interface (CLI)* where extra practice is needed. **Official LPI 010-200:** Topic 012.

**Learn:** `pwd`, `ls`, `cd`, `mkdir`, `touch`, `cp`, `mv`, `rm`, `find`; absolute/relative paths; hidden files; command options; `man` and `--help`; environment variables and `$PATH`; quoting and basic globbing.

**Lab:** build a tree under `~/linux-essentials-labs/week02`, create and move files, find them by name, and explain why `"$HOME"` and `'$HOME'` expand differently. Use `man ls` to find an unfamiliar option.

**Deliverable:** `week-02-cli-and-files.md` with commands, outputs and a 10-command recall sheet.

**Checkpoint:** Navigate, find and reorganise files without a GUI or copied commands.

- [ ] Complete lessons
- [ ] Run lab commands
- [ ] Commit notes
- [ ] Self-test

### Week 3 — 30 November–6 December: Text processing and archives

**LPI 2.0 objective group:** 013.1–013.2 — Archives, Compression, Redirection and String Processing.

**Pluralsight:** relevant certification-path sections and selected *Bash Input/Output and Streams* / *Linux Fundamentals* material. **Official LPI 010-200:** Topics 013.1–013.2.

**Learn:** `cat`, `less`, `head`, `tail`, `grep`, `grep -E`, `sort`, `uniq`, `cut`, `wc`; `>`, `>>`, `<`, `|`; simple regular expressions; `tar`, `gzip`, `bzip2`, `xz`, `zip`, `unzip`.

**Lab:** create a sample service log (not a real sensitive log), filter `ERROR` entries using `grep`, count occurrences, sort them, archive the lab directory and restore it to a separate path.

**Deliverable:** `week-03-text-processing.md` plus a safe example pipeline and backup/restore instructions.

**Checkpoint:** Explain a command pipeline left-to-right and restore an archive reliably.

- [ ] Complete lessons
- [ ] Run lab commands
- [ ] Commit notes
- [ ] Self-test

### Week 4 — 7–13 December: Bash scripting

**LPI 2.0 objective group:** 013.3 — Shell Scripting Basics (high relative weighting within the exam objectives).

**Pluralsight:** *Bash Script Flow and Basic Utilities*; focused sections of *Bash Input/Output and Streams*. Do the *Basic Bash Scripting & Arguments* lab if available. **Official LPI 010-200:** Topic 013.3.

**Learn:** `#!/bin/bash`, variables, quoting, positional arguments (`$1`), conditions (`if`), `for` loops, exit codes (`$?`) and `chmod +x`.

**Lab:** write `hearth-health-check.sh` that prints a timestamp, checks whether an input directory exists, loops through named local test files and reports whether they are present. For an optional stretch goal, print `df -h` and `free -h`.

**Deliverable:** `scripts/hearth-health-check.sh` and `week-04-bash-scripting.md` with explanations and sample output.

**Checkpoint:** Rewrite a short `if` plus `for` script from memory and predict its output.

- [ ] Complete lessons
- [ ] Run lab commands
- [ ] Commit notes
- [ ] Self-test

### Week 5 — 14–20 December: Processes, logs and networking

**LPI 2.0 objective group:** 014 — Linux System Administration Basics.

**Pluralsight:** *Getting Started with Linux System Administration* + administration lab; selected *System Management and File Security* and *Networking, Packages, and Automation Basics* modules. **Official LPI 010-200:** Topic 014.

**Learn:** Linux boot/VM concepts and `/dev`; `ps`, `top`, `free`; `systemctl status/start/stop`; `journalctl`, `dmesg`, `/var/log`; `ip addr`, `ip route`, `ss`, `ping`, DNS configuration, IPv4 vs IPv6, DHCP and name resolution.

**Lab:** inspect `systemd-journald` rather than altering a production service; view recent journal entries; identify a process; document network address, default route and DNS settings on the lab VM.

Safe example commands:

```bash
ps aux | head
systemctl status systemd-journald
journalctl -n 20 --no-pager
ip addr show
ip route show
ss -tuln
```

**Deliverable:** `week-05-admin-and-networking.md` — a short Linux service / network triage runbook.

**Checkpoint:** Given a mock 'service is not responding' alert, identify which commands show service status, logs, listening sockets, IP address and route.

- [ ] Complete lessons
- [ ] Run lab commands
- [ ] Commit notes
- [ ] Self-test

### Christmas break — 23 December 2026 to 1 January 2027

**No scheduled learning.** No Pluralsight modules, lab work, GitHub commits, flashcards, or exam questions are expected during these dates. **21–22 December** are only optional catch-up days; **2–3 January** are optional re-entry days. If nothing gets done on those buffer days, nothing needs to be made up.

### Week 6 — 4–10 January 2027: Access control and exam review

**LPI 2.0 objective group:** 015 — Security and File System Permissions + all-objective review.

**Pluralsight:** selected *User, Group, and Permission Management in Ubuntu Linux* sections, followed by focused exam revision. **Official LPI 010-200:** Topic 015. Treat any **010-160** practice score as a fundamentals check, not proof of 010-200 readiness.

**Learn:** users/groups, `id`, `useradd`, `groupadd`, `passwd`; `/etc/passwd`, `/etc/shadow`; permissions (`rwx`, octal), `chmod`, `chown`; temporary directories, symlinks and sticky bit; `sudo`, `su`, `ssh`, `scp`, public-key basics.

**Lab:** on the disposable VM only, create a test group/user, manage ownership and permissions on test files, create a symlink and examine SSH key authentication concepts. Remove test identities after recording the exercise.

**Deliverable:** `week-06-security-and-review.md`, `exam-objective-checklist.md`, and a list of weak topics.

**Week 6 checkpoint:**

- [ ] Review the entire 010-200 objective checklist
- [ ] Take timed mock 1: **40 questions / 60 minutes** using version-matched material
- [ ] Review every wrong or guessed answer and identify its LPI objective
- [ ] Revisit weak topics with a short, isolated VM lab
- [ ] Explain high-weight objectives without reference notes

### Exam-readiness window — 11–17 January 2027

- [ ] Take timed mock 2: **40 questions / 60 minutes**, ideally a different version-appropriate question set
- [ ] Review errors and any remaining weak objective groups
- [ ] Confirm the exam code on the voucher/booking is **010-200**
- [ ] Check available booking times and choose the exam date only when prepared

**Readiness rule (self-imposed, not an LPI pass score):** aim for **85% or higher on two timed mocks**, with no persistent weak objective group, before sitting the exam. **11–17 January is a target window, not a fixed deadline**; move the exam if the voucher arrives late or you need more practice.

## 6. Version 2.0 additions that must not be missed

For the working target **010-200**, specifically verify these against the official objectives even if the 010-160 Pluralsight path doesn't emphasise them:

- [ ] `systemctl` for systemd services
- [ ] `journalctl` and journal-based log review
- [ ] `ip addr`, `ip route` and `ss` (modern networking tools)
- [ ] SSH login, `scp`, SSH key basics and `authorized_keys`
- [ ] Bash `if` conditions and exit status
- [ ] Current distribution names, application families and package managers
- [ ] Linux/cloud and VM provisioning concepts
- [ ] DNS and IPv6 fundamentals

See the [official 010-200 objective list](https://www.lpi.org/our-certifications/exam-010-objectives/) for precise scope. If taking **010-160**, use the [version 1.6 official objectives](https://wiki.lpi.org/wiki/LinuxEssentials_Objectives_V1.6) instead of assuming that the new list is your exam blueprint.

## 7. Repository structure

Suggested location inside **Enterprise IT Learning**:

```text
Enterprise-IT-Learning/
└── linux-system-administration/
    └── certifications/
        └── linux-essentials/
            ├── README.md
            ├── Linux_Essentials_010-200_Learning_Plan.md
            ├── exam-objective-checklist.md
            ├── notes/
            │   ├── week-01-linux-foundations.md
            │   ├── week-02-cli-and-files.md
            │   ├── week-03-text-processing.md
            │   ├── week-04-bash-scripting.md
            │   ├── week-05-admin-and-networking.md
            │   └── week-06-security-and-review.md
            ├── labs/
            ├── scripts/
            │   └── hearth-health-check.sh
            └── exam-preparation/
                ├── mock-exam-results.md
                └── weak-areas.md
```

Adjust the parent folders to match the actual repository layout. Do not add empty folders unless they contain a placeholder (Git only tracks files).

## 8. Weekly notes template

```markdown
# Week XX — Topic

**Study dates:**
**LPI objective(s):**
**Pluralsight module(s):**
**Time spent:**

## What I learned
-

## Commands practised
| Command | Purpose | Example / result |
|---|---|---|
| | | |

## Lab evidence
-

## What went wrong / what I fixed
-

## Self-test
- Score:
- Weak topics:

## Next actions
- [ ]
```

## 9. Exam readiness checklist

**Timing:** Complete this section from 4 January onward, not during the Christmas break.


- [ ] Confirmed booked exam code: `010-200` (or revised plan if the booking is `010-160`)
- [ ] Every official objective reviewed at least once
- [ ] All core Pluralsight courses finished
- [ ] Core guided labs finished or replaced with documented Hearth equivalents
- [ ] Shell commands practised from memory
- [ ] Bash script written and explained
- [ ] Service / logs / networking troubleshooting drill completed
- [ ] User, group, SSH and permission exercises completed safely
- [ ] Two timed version-appropriate mocks completed at target score
- [ ] Pearson VUE account, LPI ID, test arrangements and name details checked
- [ ] Lab notes and learning record committed to GitHub

## 10. After certification

The most useful next track for an L2 RHEL administrator is **RHEL administration → RHCSA-oriented fundamentals → Ansible**. Continue using the dedicated Project Hearth lab to turn exam knowledge into documented enterprise-style operations: service checks, user administration, permissions, package management, logs, SSH, and eventually automation.

---

**Prepared:** 15 November 2026  
**Sources:** LPI (official 010-200 objectives, new 010-200 Learning Materials and 2026 exam update) and current public Pluralsight catalogue.  
**Personal goal:** Pass the certification while producing an interview-ready, safe, reproducible Linux learning record.
