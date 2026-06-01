# Linux+ Practice Exam – Make-Up Test C Review

**Date:** May 31, 2026
**Set:** 1/3 (Make‑Up Test C) – 30 questions
**Score:** 17/30 (57%)
**Previous scores:** 11/30 → 16/30 → 15/30 → 17/30

## Domain Breakdown of Misses

| Domain | Missed Questions | Specific Gaps |
|--------|------------------|---------------|
| System Management | 2,5,6,8,10,14 | `modinfo`, `du`, GPT tools, `/etc/resolv.conf`, current directory (`.`), NAT vs host‑only |
| Services & User Management | 16,18,20 | `passwd` vs `chsh`, `kill -15`, `jobs` command |
| Security | 24,26,27,28 | firewalld zones, `setgid`, `/etc/sudoers`, LUKS2 |

## Missed Questions – Correct Answers & Why

| Q | Your Answer | Correct | Explanation |
|---|-------------|---------|-------------|
| 2 | insmod | **modinfo** | `modinfo` shows kernel module details; `insmod` only loads.
| 5 | df | **du** | `df` = filesystem usage, `du` = directory usage.
| 6 | fdisk | **All of the above** | `fdisk`, `parted`, and `growpart` all support GPT.
| 8 | /etc/hosts | **/etc/resolv.conf** | DNS server addresses go in `resolv.conf`.
| 10 | Root directory | **Current directory** | Single dot (`.`) = current directory.
| 14 | Host‑only | **NAT** | NAT gives VM external access via host IP.
| 16 | chsh | **passwd** | `passwd` changes password; `chsh` changes shell.
| 18 | renice | **kill -15** | `kill -15` (SIGTERM) terminates gracefully.
| 20 | ps | **jobs** | `jobs` lists background jobs in current shell.
| 24 | Chains | **Zones** | `firewalld` uses zones to group rules.
| 26 | Sticky bit | **setgid** | `setgid` on directory makes new files inherit group.
| 27 | /etc/shadow | **/etc/sudoers** | `sudo` privileges are defined in `/etc/sudoers`.
| 28 | TLS | **LUKS2** | LUKS2 is full‑disk encryption for Linux.

## Flashcards to Create

- `modinfo` – display kernel module information
- `du` vs `df` – disk usage vs filesystem usage
- GPT support: `fdisk`, `parted`, `growpart`
- `/etc/resolv.conf` – DNS server addresses
- Current directory (`.`) vs parent (`..`) vs root (`/`)
- NAT vs host‑only networking
- `passwd` changes password, `chsh` changes shell
- `kill -15` (SIGTERM) for graceful termination
- `jobs` command lists background jobs
- firewalld zones (public, home, etc.)
- `setgid` on directories – inherit group ownership
- `/etc/sudoers` – sudo rules
- LUKS2 – encrypted filesystems

## Next Study Plan

1. **Drill System Management flashcards** (10 min daily).
2. **Re‑take a 30‑question set** in 2‑3 days, aim for 20+ correct.
3. **Schedule the real exam** once you consistently hit 80% on practice tests.

## Progress Over Time

- Set 1 (original): 11/30 (37%)
- Make‑Up Test A: 16/30 (53%)
- Make‑Up Test B: 15/30 (50%)
- **Make‑Up Test C: 17/30 (57%)**

---
*Every missed question is a flashcard. Keep grinding.*
