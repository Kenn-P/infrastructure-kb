---
layout: default
---

# 📊 Linux Process Management

This section covers commands used to monitor, manage, and control processes in Linux systems.

---

## 🔍 View Processes

| Command | Usage & Options |
|--------|----------------|
| `ps aux` | Show all running processes; `a` → all users, `u` → detailed format, `x` → background processes |
| `top` | Real-time process monitoring |
| `htop` | Interactive process viewer (if installed) |

---

## 🧠 Process Details

| Command | Usage & Options |
|--------|----------------|
| `ps -ef` | Full process listing; `-e` → all processes, `-f` → full format |
| `pidof nginx` | Get PID of a process |
| `pgrep nginx` | Find process ID by name |

---

## ❌ Kill Processes

| Command | Usage & Options |
|--------|----------------|
| `kill PID` | Terminate process gracefully |
| `kill -9 PID` | Force kill process; `-9` → SIGKILL |
| `pkill nginx` | Kill process by name |

---

## ⚙️ Process Priority

| Command | Usage & Options |
|--------|----------------|
| `nice -n 10 command` | Start process with priority; `-n` → niceness value |
| `renice 10 PID` | Change priority of running process |

---

## 🔄 Background Jobs

| Command | Usage & Options |
|--------|----------------|
| `command &` | Run process in background |
| `jobs` | List background jobs |
| `fg` | Bring job to foreground |
| `bg` | Resume job in background |

---

## 🔥 Useful Example

| Command | Usage & Options |
|--------|----------------|
| `ps aux | grep apache` | Find Apache process |
| `kill -9 1234` | Force kill process with PID 1234 |
| `top` | Monitor CPU & memory usage |

---

## 🎯 Summary

- Use `ps`, `top`, `htop` to monitor processes  
- Use `kill`, `pkill` to stop processes  
- Manage priority using `nice` and `renice`  
- Background jobs help manage long-running tasks  
