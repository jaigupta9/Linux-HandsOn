# Experiment 5

---

## Experiment Description
This lab focuses on managing processes using commands like `ps`, `top`, and `kill`, as well as managing software using `apt-get` for installation, updating, and removal.

---

## Approach

### 1. Process Management

#### a. Viewing Processes with `ps`
The `ps` command displays details about active processes.

##### Commands:
1. View processes for the current user:
   ```bash
   ps
   ```
2. View all processes:
   ```bash
   ps -e
   ```
3. View processes in detailed format:
   ```bash
   ps -ef
   ```

#### Screenshots:
- ![Display processes for the current user](./ps0.png)
- ![Display all processes](./ps.png)
- ![Display processes in full format](./psef.png)

---

#### b. Monitoring Processes with `top`
The `top` command provides a real-time view of system processes.

##### Command:
```bash
top
```

#### Screenshot:
![Running top command](./top.png)

---

#### c. Terminating Processes with `kill`
The `kill` command is used to terminate processes by their PID.

##### Commands:
1. End a process by PID:
   ```bash
   kill <PID>
   ```
2. Forcefully terminate a process:
   ```bash
   kill -9 <PID>
   ```

#### Screenshots:
- ![Terminating a process by PID](./kill0.png)
- ![Forcefully terminating a process](./kill.png)

---

### 2. Software Management with `apt-get`

#### a. Installing Software
The `apt-get install` command is used to install software packages.

##### Command:
```bash
sudo apt-get install htop
```

#### Screenshot:
![Installing htop](./installhtop.jpg)

---

#### b. Updating Software
To refresh the package list and upgrade installed packages:

##### Commands:
1. Update the package list:
   ```bash
   sudo apt-get update
   ```
2. Upgrade installed packages:
   ```bash
   sudo apt-get upgrade
   ```

#### Screenshots:
- ![Updating package list](./update.png)
- ![Upgrading packages](./upgrade.png)

---

#### c. Removing Software
The `apt-get remove` command is used to uninstall software, and `apt-get purge` removes it along with configuration files.

##### Commands:
1. Remove a package:
   ```bash
   sudo apt-get remove htop
   ```
2. Purge a package:
   ```bash
   sudo apt-get purge htop
   ```

#### Screenshots:
- ![Removing htop](./removehtop.jpg)
- ![Purging htop](./purgehtop.png)

---

### 3. Verifying Software Installation and Removal
The `dpkg` command is used to check if a package is installed.

##### Command:
```bash
dpkg -l | grep htop
```

#### Screenshot:
![Verifying htop installation](./dpkghtop.png)

---

## Conclusion
In this lab, you practiced:
1. Managing processes using `ps`, `top`, and `kill`.
2. Installing, updating, and removing software using `apt-get`.

These skills are essential for effective system administration, process monitoring, and software management in Linux environments.
