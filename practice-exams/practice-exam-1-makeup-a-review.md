# Linux+ Practice Exam – Make-Up Test A Review

**Date:** May 2026  
**Set:** 1/3 (Make-Up Test A) – 30 random questions, same difficulty as original Set 1  
**Score:** 16/30 (53%)  
**Previous score on original Set 1:** 11/30 (37%)  
**Improvement:** +5 correct answers  

**Goal:** Reach 24/30 (80%) before moving to Set 2/3.

---

## 📊 Domain Performance

| Domain | Questions Missed | Status |
|--------|------------------|--------|
| System Management | 4, 7, 8, 9, 11, 12, 14, 23 | Still weak (8 misses) |
| Services & User Management | 16, 17, 19, 20 | Moderate (4 misses) |
| Security | 25, 26, 27 | Weak (3 misses + blanks) |
| Automation & Troubleshooting | None (29,30 correct) | Strong |

**Biggest gains:** Automation & Troubleshooting (both correct).  
**Biggest opportunity:** System Management (23% of exam weight).

---

## 🔧 Missed Questions – Correct Answers & One‑Line Fixes

| Q | Topic | Correct Answer | Why / Command |
|---|-------|----------------|----------------|
| 4 | Create LVM physical volume | `pvcreate` | `sudo pvcreate /dev/sdb` |
| 7 | Apply Netplan changes | `netplan apply` | `sudo netplan apply` |
| 8 | Test HTTP connectivity | `curl` | `curl -I http://example.com` |
| 9 | What is `..` | Parent directory | `cd ..` moves up one level |
| 11 | Append output to file | `>>` | `echo "new line" >> file.txt` |
| 12 | Show kernel/arch info | `uname` | `uname -a` |
| 14 | VM direct host networking | Bridged mode | VM network = bridged to host NIC |
| 16 | Create a new group | `groupadd` | `sudo groupadd devops` |
| 17 | User account file (no hashes) | `/etc/passwd` | `cat /etc/passwd` |
| 19 | Keep process after logout | `nohup` | `nohup ./script &` |
| 20 | Change process priority (running) | `renice` | `renice +5 -p PID` |
| 23 | Container uses host network stack | `host` network | `docker run --network host` |
| 25 | Delete only own files in shared dir | Sticky bit (`+t`) | `chmod 1777 /shared` |
| 26 | Show SELinux status | `getenforce` | `getenforce` |
| 27 | Ticket‑based authentication | Kerberos | `kinit` (concept) |

*(I also left #2 blank – correct answer was `lspci` for PCI devices; #26, #27 were blank – now filled above.)*

---

## ✅ What I Got Right (and why it matters)

| Q | Topic | Why I knew it |
|---|-------|----------------|
| 1 | Log files in `/var` | I check `/var/log` frequently |
| 2 | `lspci` | Ran it when debugging GPU passthrough |
| 3 | `rmmod` | Removed a troublesome module once |
| 5 | `df` for disk space | Daily habit |
| 6 | `/proc/mounts` | Looked up mounted filesystems |
| 10 | `tail` | Use it for logs |
| 13 | `gzip` | Compressed backups |
| 15 | KVM native hypervisor | Use it for VMs |
| 18 | `who` | Check logged‑in users |
| 21 | `rpm` for RHEL | Familiar from Rocky Linux |
| 22 | `systemctl enable` | Set up auto‑start services |
| 24 | `ufw` on Ubuntu | Configured firewall earlier |
| 28 | TLS for network encryption | HTTPS = TLS |
| 29 | `while` loop | Wrote one in my git‑sync script |
| 30 | DNS issue | Experienced it – first thing to check |

These correct answers come from **real experience**, not just memorization. That's solid.

---

## 📝 Flashcards to Create (from this test)

Make a flashcard for each missed question. Example format:

> **Front:** How to create a physical volume for LVM?  
> **Back:** `pvcreate /dev/sdX`

Other flashcards:

- `netplan apply` vs `netplan verify`  
- `curl` for HTTP testing (not `ping`)  
- `..` = parent directory  
- `>>` appends, `>` overwrites  
- `uname -a` shows kernel/arch  
- Bridged vs NAT network mode  
- `groupadd` creates a group  
- `/etc/passwd` stores user info (not passwords)  
- `nohup` keeps process after logout  
- `renice` changes priority of running process  
- Docker `--network host`  
- Sticky bit (`chmod +t`)  
- `getenforce` for SELinux  
- Kerberos = ticket auth  

Review these for 5 minutes every morning.

---

## 🚀 Next Steps

1. **Lab every missed command** on your server or in a VM.
2. **Take another fresh 30‑question set** (same difficulty) in 2 days.
3. **Goal:** Score 20/30 (67%) or higher before moving to Set 2/3.

---

## 📌 Notes to Self

- I improved from 11 → 16 (+5). That's progress, not failure.
- System Management is still my weakest domain – focus there.
- I know more than my score shows – the gap is exam vocabulary, not skill.
- Keep using flashcards + terminal practice. It's working.

*Slow improvement is still improvement.*
