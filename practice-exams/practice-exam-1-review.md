# Linux+ Practice Exam 1 Review – Set 1 of 3

**Date:** May 2026  
**Questions:** 30 (from official XK0-006 objectives)  
**Score:** 11/30 (37%)  
**Goal:** Identify weak domains, focus study, and improve to 80%+

---

## 🎯 Domain Breakdown (based on missed questions)

| Domain | Questions Missed | Status |
|--------|------------------|--------|
| System Management | 2, 4, 5, 7, 8, 9, 14 | ❌ Weak |
| Services & User Management | 16, 17, 18, 20, 21, 22 | ✅ Mixed (some right) |
| Security | 24, 25, 26, 27, 28 | ❌ Weak (except 27) |
| Automation & Scripting | 29 | ❌ Weak |
| Troubleshooting | 30 | ✅ Correct |

**Priority focus:** System Management (23% of exam) + Security (18%)

---

## 🔧 Missed Questions – Correct Answers & Commands

| # | Question Topic | Correct Answer | One‑line Command / File to Remember |
|---|----------------|----------------|--------------------------------------|
| 2 | View loaded kernel modules | `lsmod` | `lsmod` (run it!) |
| 4 | Create LVM logical volume | `lvcreate` | `sudo lvcreate -n test -L 1G myvg` |
| 5 | Default Red Hat filesystem | XFS | `df -T` – check filesystem types |
| 7 | Auto‑mount at boot | `/etc/fstab` | `cat /etc/fstab` |
| 8 | Prevent binary execution | `noexec` mount option | `mount -o noexec /mountpoint` |
| 9 | Show routing info | `ip route` | `ip route show` |
| 14 | Archive without compression | `tar` | `tar -cf archive.tar files/` |
| 25 | Sudo no password | `NOPASSWD` in sudoers | `sudo visudo` → add `NOPASSWD` |
| 26 | Make file immutable | `chattr +i` | `sudo chattr +i file` (immutable) |
| 29 | Exit status of previous command | `$?` | `echo $?` after any command |

---

## 📝 Flashcards to Create (front/back)

- **Front:** Which command shows loaded kernel modules? → `lsmod`
- **Front:** How to create a logical volume? → `lvcreate -n NAME -L SIZE VG`
- **Front:** Default filesystem for RHEL? → XFS
- **Front:** Which file controls auto‑mount at boot? → `/etc/fstab`
- **Front:** How to prevent binary execution on a mount? → `noexec` option
- **Front:** Command to view routing table? → `ip route`
- **Front:** Which tool archives without compression? → `tar`
- **Front:** Sudoers option to skip password? → `NOPASSWD`
- **Front:** Make a file immutable? → `chattr +i`
- **Front:** Variable holding last command exit status? → `$?`

---

## ✅ What I Got Right (and why)

| # | Topic | Why I knew it |
|---|-------|----------------|
| 11 | `PATH` environment variable | I use `echo $PATH` often |
| 13 | `grep` for searching text | Daily use in troubleshooting |
| 15 | `rsync` for efficient sync | Used for backups |
| 17 | `id` command | Check UID/GID regularly |
| 18 | `chsh` change shell | Used when setting up user accounts |
| 19 | `SIGKILL` (9) | Killed unresponsive processes |
| 20 | `crontab` | Already set up cron jobs |
| 21 | `dpkg` (Debian) | Installed packages on Ubuntu |
| 22 | `systemctl start` | Starts services daily |
| 27 | SSH (encrypted remote shell) | Use it all the time |
| 30 | High I/O wait = storage issue | Diagnosed slow disk before |

These are **real, hands‑on skills** – not just book knowledge.

---

## 🚀 Next Study Plan

1. **Lab each missed command** (run `lsmod`, `lvcreate` in a test VM, edit `/etc/fstab`, etc.)
2. **Review flashcards** for 5 minutes every morning
3. **Take another 30‑question set** in 2‑3 days (focus on System Management + Security)
4. **Goal:** Improve to at least 20/30 (67%) before moving to Set 2

---

## 📌 Notes for Myself

- I learn by **doing** – so I'll run each command, not just memorize.
- The exam requires **recognition**; flashcards + terminal practice will bridge the gap.
- I already have strong troubleshooting and automation instincts – I just need to map them to exam terms.

*Progress, not perfection.*
