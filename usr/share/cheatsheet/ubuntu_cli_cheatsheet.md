# Ubuntu Command Line Cheat Sheet

---

## 🧭 Basics & Navigation

| Command               | Description                       |
|-----------------------|----------------------------------|
| `pwd`                 | Print current directory           |
| `ls -l`               | List files in long format         |
| `cd /path/to/dir`     | Change directory                  |
| `cd ..`               | Go up one directory               |
| `mkdir mydir`         | Create a new directory            |
| `touch file.txt`      | Create a new file                 |
| `clear`               | Clear the terminal                |
| `history`             | Show command history              |
| `man <command>`       | Show manual/help for a command    |
| `alias ll='ls -alF'`  | Create a shortcut alias           |

---

## 📁 File Management & Permissions

| Command                          | Description                            |
|---------------------------------|--------------------------------------|
| `cp file1.txt file2.txt`        | Copy file                            |
| `mv file.txt /other/dir/`       | Move or rename file                  |
| `rm file.txt`                   | Delete file                         |
| `rm -r dir/`                   | Delete directory recursively         |
| `chmod +x script.sh`            | Make file executable                |
| `chmod 755 file`               | Change permissions (rwxr-xr-x)       |
| `chown user:group file`        | Change file owner and group          |
| `ls -l`                       | Show file permissions and ownership  |

---

## ⚙️ Processes & System Monitoring

| Command                        | Description                                |
|--------------------------------|--------------------------------------------|
| `ps aux`                      | Show all running processes                  |
| `top`                        | Interactive process monitor                  |
| `htop`                       | Enhanced interactive process viewer (if installed) |
| `kill PID`                   | Kill process by PID                         |
| `kill -9 PID`                | Force kill process                          |
| `systemctl status service`   | Check status of a systemd service           |
| `systemctl start service`    | Start a systemd service                      |
| `systemctl stop service`     | Stop a systemd service                       |
| `free -h`                   | Show memory usage in human-readable format |
| `df -h`                     | Show disk usage                             |

---

## 📝 Working with Text & Logs

| Command                            | Description                              |
|-----------------------------------|----------------------------------------|
| `cat file.txt`                    | Display file contents                   |
| `less file.log`                   | View file with scrolling                |
| `tail -f /var/log/syslog`         | Follow (live update) log file           |
| `grep "error" file.log`            | Search for "error" in file               |
| `head -n 20 file.txt`             | Show first 20 lines                      |
| `cut -d "," -f 2 file.csv`        | Extract 2nd column from CSV file         |
| `awk '{print $1}' file.txt`       | Print first field of each line           |
| `sort file.txt`                   | Sort lines alphabetically                 |
| `uniq file.txt`                   | Remove duplicate adjacent lines          |

---

## 📦 Package & Service Management

| Command                          | Description                               |
|---------------------------------|-------------------------------------------|
| `sudo apt update`               | Update package lists                       |
| `sudo apt upgrade`              | Upgrade installed packages                 |
| `sudo apt install package`     | Install a package                          |
| `sudo apt remove package`      | Remove a package                           |
| `dpkg -i package.deb`           | Install a .deb package                     |
| `systemctl status service`     | Check service status                       |
| `systemctl start service`      | Start a service                            |
| `systemctl stop service`       | Stop a service                             |
| `systemctl restart service`    | Restart a service                          |
| `systemctl enable service`     | Enable service at boot                     |
| `systemctl disable service`    | Disable service at boot                    |

---

## 🌐 Networking, SSH & Ports

| Command                          | Description                               |
|---------------------------------|-------------------------------------------|
| `ip a` or `ifconfig`            | Show network interfaces                    |
| `ping google.com`               | Ping a host                               |
| `ss -tuln`                     | List listening ports                       |
| `netstat -tulnp`               | Show active connections and ports         |
| `ssh user@hostname`             | Connect via SSH                           |
| `scp file user@host:/path`      | Copy file over SSH                        |
| `curl http://example.com`       | Fetch content from URL                    |
| `wget http://example.com/file`  | Download file from URL                    |
| `ufw status`                   | Check firewall status                      |
| `ufw allow 22/tcp`             | Allow SSH port through firewall            |

---

# Tips & Tricks

- Use `tab` for auto-completion.
- Press `Ctrl + R` to reverse search command history.
- Use `!!` to repeat last command.
- Combine commands with `&&` to run sequentially only if previous succeeds.
