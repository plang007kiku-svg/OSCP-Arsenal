🛡️ Major Privilege Escalation Vulnerabilities (Privilege Escalation Cheatsheet)
💻 Windows PE Tactics

1. Service Misconfiguration: Check for unquoted service paths or services with insecure file/folder permissions to replace EXE files with payloads.

2. Unpatched Kernel/Software: Find outdated kernel exploits or software exploits (such as printer spoolers). Using tools like Watson or PowerUp.

3. Stored Credentials: Search for passwords or hashes stored in the Registry, files, or in memory (e.g., via Mimikatz) used for administrator access.

4. Scheduled Tasks Misconfiguration: Check for tasks running with high privileges that can modify the binaries they call.

🐧 Linux PE Tactics

1. Misconfigured SUID/GUID: Search for binaries containing a special SUID/GUID bit (e.g., `find / -perm -4000 2>/dev/null`) that allows a regular user to run code with root privileges.

2. Kernel Exploits: Search for unpatched kernel vulnerabilities (requires a custom script to compile).

3. Weak File Permissions: Check for sensitive system files (e.g., `/etc/passwd`, `/etc/shadow`) or configuration files with write permissions.

4. Writable PATH: Check for environment variables. 4. $PATH: Check which folders a regular user has write permissions to place fake binaries (e.g., `ls -l /usr/local/sbin`).

5. Crontab/Scheduled Tasks Misconfiguration: Check Cron Jobs running with root privileges and the ability to modify the executed scripts.

🔑 Important Commands/Tools

• Windows: `whoami /priv`, `systeminfo`, PowerUp.ps1, WinPEAS

• Linux: `uname -a`, `sudo -l`, `find / -perm -4000 2>/dev/null`, LinPEAS.sh
 
