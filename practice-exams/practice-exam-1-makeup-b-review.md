# Linux+ Practice Exam – Make‑Up Test B Review

**Date:** May 27, 2026  
**Set:** 1/3 (Make‑Up Test B) – 30 questions, same difficulty as previous sets  
**Score:** 15/30 (50%)  
**Previous scores:** 11/30 → 16/30 → 15/30 (improvement consistent)

**Goal:** 24/30 (80%) before moving to Set 2/3.

---

## 📊 Domain Performance (estimated from misses)

| Domain | Misses (approx) | Key gaps |
|--------|----------------|----------|
| System Management | 10+ | `lsusb`, `modprobe`, `nosuid`, `/etc/hosts`, `find`, `xz`, host‑only networking, `lvextend` (not listed but missed), inodes |
| Services & User Management | 3 | `at`, `&`, `daemon-reload` |
| Security | 3 | `firewall-cmd --permanent`, `setuid` |
| Automation & Scripting | 2 | Dockerfile `FROM`, `-eq` vs `=` |
| Troubleshooting | 1 | Inode exhaustion |

**System Management remains the weakest domain – but each miss becomes a flashcard.**

---

## 🔧 Missed Questions – Correct Answers & One‑Line Fixes

| Q | Topic | Correct Answer | Why / Command |
|---|-------|----------------|----------------|
| 1 | List USB devices | `lsusb` | `lsblk` = block devices, `lspci` = PCI, `lsusb` = USB |
| 2 | Load kernel module with deps | `modprobe` | `modprobe` handles dependencies; `insmod` does not |
| 7 | Disable SUID on mount | `nosuid` | `noexec` blocks execution, `nosuid` ignores setuid/setgid |
| 8 | Local hostname resolution | `/etc/hosts` | `/etc/hostname` is just the machine name |
| 11 | Real‑time file search | `find` | `grep` searches content, `find` searches files |
| 13 | Create `.xz` archive | `xz` | `gzip` → `.gz`, `bzip2` → `.bz2`, `xz` → `.xz` |
| 14 | VM network mode (isolated, host‑only) | Host‑only | Bridge = LAN, NAT = outbound, Host‑only = no external |
| 19 | One‑time scheduled task | `at` | `cron` = recurring, `at` = one shot |
| 20 | Background execution symbol | `&` | `command &` runs in background |
| 22 | Reload systemd unit files | `daemon-reload` | After editing a `.service` file, run `systemctl daemon-reload` |
| 23 | Dockerfile base image | `FROM` | `FROM ubuntu:22.04` is first line in Dockerfile |
| 24 | Permanent firewalld rule | `firewall-cmd --permanent --add-service=ssh` | Must use `--permanent` then `--reload` |
| 26 | Run program with owner privileges | `setuid` | Sticky bit = restrict deletion, setuid = run as owner |
| 29 | Numeric equality in bash `[ ]` | `-eq` | `[ "$a" -eq "$b" ]` for numbers; `=` for strings inside `[[ ]]` |
| 30 | "No space" but low disk usage | Inode exhaustion | `df -i` to check inodes; many small files fill inode table |

---

## ✅ What I Got Right (but should double‑check)

- `lvextend` (Q4) – correct.
- `fsck` (Q5) – correct.
- `blkid` (Q6) – correct.
- `ss` (Q9) – correct.
- `~` (Q10) – correct.
- `|` pipe (Q12) – correct.
- `virsh` (Q15) – correct.
- `id` / `groups` (Q16‑17) – correct.
- `SIGTERM` (Q18) – correct.
- `dnf` (Q21) – correct.
- `chown` (Q25) – correct.
- `SFTP` (Q27) – correct.
- `SHA-256` (Q28) – correct.

These are solid; I just need to keep them fresh.

---

## 📝 Flashcards Created from This Test

Make physical or Anki cards for each missed question. Example format:

**Front:** How to list USB devices?  
**Back:** `lsusb`

Additional cards:
- `modprobe` vs `insmod`
- `nosuid` mount option
- `/etc/hosts` vs `/etc/hostname`
- `find` vs `grep`
- `xz` compression
- Host‑only network mode (libvirt)
- `at` command
- `&` background operator
- `systemctl daemon-reload`
- Dockerfile `FROM`
- `firewall-cmd --permanent`
- `setuid` vs sticky bit
- Bash numeric `-eq`
- Inode exhaustion (`df -i`)

---

## 🚀 Next Steps

1. **Drill System Management flashcards** every morning (10 min).
2. **Take another fresh 30‑question set** (same difficulty) in 2 days.
3. **Goal:** 20/30 (67%) or higher.
4. **After consistent 70%+**, move to Set 2/3 (harder PBQ‑style).

---

## 📌 Notes to Self

- System Management is 23% of the exam – it's okay that it's my focus.
- I improved from 11 → 15 → 16 → 15; the drop is within noise. Next target: 20.
- Each missed question is a direct pointer to what to study next. No shame – just data.

*Review these flashcards daily. The scores will follow.*
