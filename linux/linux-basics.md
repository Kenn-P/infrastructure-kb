# 🐧 Linux Basics & Commands

This section covers essential Linux commands used in daily system administration and troubleshooting.

---

## 📂 File & Directory Management

```pwd```  
Print working directory (shows current location)

```ls -l```  
List files in long format (permissions, owner, size, date)  
-l → long format

```ls -a```  
List all files including hidden files (. files)  
-a → all

```cd /path```  
Change directory to specified path

```mkdir test```  
Create a new directory named "test"

```rm -rf test```  
Remove directory forcefully  
-r → recursive  
-f → force (no prompt)

```cp file1 file2```  
Copy file1 to file2

```mv file1 file2```  
Move or rename file

---

## 📄 File Viewing

```cat file.txt```  
Display full file content

```less file.txt```  
View file page by page (scrollable)

```head -n 10 file.txt```  
Show first 10 lines  
-n → number of lines

```tail -f file.txt```  
Show last lines and follow live updates  
-f → follow (real-time)

---

## 🔐 Permissions

```chmod 755 file.sh```  
Change file permissions  
7 → owner (read, write, execute)  
5 → group (read, execute)  
5 → others (read, execute)

```chown user:user file.txt```  
Change file ownership  
user:user → owner:group

---

## 👤 User Management

```useradd testuser```  
Create a new user

```passwd testuser```  
Set password for user

```id testuser```  
Show user ID, group ID, and groups

---

## 📊 Process Management

```ps aux```  
Show all running processes  
a → all users  
u → detailed format  
x → background processes

```top```  
Real-time process monitoring

```kill -9 PID```  
Terminate process forcefully  
-9 → SIGKILL (force stop)

---

## 🌐 Networking

```ip a```  
Show IP address and network interfaces

```ping google.com```  
Check network connectivity

```ss -tulnp```  
Show listening ports and services  
-t → TCP  
-u → UDP  
-l → listening  
-n → numeric output  
-p → process info

---

## 💾 Disk Usage

```df -h```  
Show disk space usage  
-h → human readable (MB/GB)

```du -sh *```  
Show size of files/directories  
-s → summary  
-h → human readable

```lsblk```  
List block devices (disks, partitions)

---

## 🔍 Logs

```journalctl -xe```  
View system logs  
-x → detailed explanation  
-e → jump to end

```dmesg```  
Show kernel logs (boot/system messages)

---

## 🔥 Useful Command

```watch -n 1 "df -h"```  
Run command every 1 second  
-n → interval in seconds

Monitor disk usage in real time
