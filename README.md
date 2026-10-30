
# Linux Fundamentals | Kali Linux

![Kali Linux](https://img.shields.io/badge/OS-Kali%20Linux-557C94?logo=kalilinux&logoColor=white)
![Linux](https://img.shields.io/badge/Platform-Linux-FCC624?logo=linux&logoColor=black)
![Focus](https://img.shields.io/badge/Focus-Linux%20%7C%20Networking%20%7C%20Cybersecurity-blue)
![Status](https://img.shields.io/badge/Status-Completed-success)

**A hands-on Linux fundamentals project demonstrating directory management, system information gathering, and basic network connectivity testing using Kali Linux.**

## 📌 Project Overview

This project is part of the 10alytics Linux Fundamentals assignment, completed in 2026.

It demonstrates practical experience using the Linux command-line interface (CLI) to perform essential system administration and networking tasks in a Kali Linux environment.

The project focuses on developing foundational technical skills relevant to Linux administration, networking, cybersecurity, and Governance, Risk and Compliance (GRC).

Through practical exercises, I explored how to organise files and directories, identify system configurations, retrieve hardware and operating system information, and troubleshoot basic network connectivity.

## 🎯 Problem Statement

Understanding how to interact with Linux systems through the command line is an essential skill for anyone pursuing a career in networking, cybersecurity, or IT infrastructure.

This project addresses the need to develop practical Linux knowledge by working through common system administration and networking activities.

The exercises demonstrate how to:

- Organise files and directories efficiently.
- Navigate the Linux file system.
- Identify the current user and hostname.
- Retrieve operating system and hardware information.
- Examine memory and disk usage.
- Test network connectivity using IP addresses.
- Understand how domain name resolution works during network connectivity testing.

## 🚀 Project Objectives

The main objectives were to:

1. Develop confidence using the Kali Linux terminal.
2. Practise creating and managing directory structures.
3. Understand basic Linux system identification commands.
4. Explore operating system, memory, and disk information.
5. Perform basic network connectivity tests.
6. Understand the relationship between DNS resolution and network communication.

## 🛠️ Technologies and Tools

| Technology / Tool | Purpose |
|---|---|
| Kali Linux | Linux operating system used for the exercises |
| Linux Terminal | Executing commands and interacting with the operating system |
| Bash / Shell | Command-line environment |
| `mkdir` | Creating directories |
| `ls` | Listing directory contents |
| `nano` | Creating and editing text files |
| `mousepad` | Graphical text editing |
| `whoami` | Identifying the currently logged-in user |
| `hostname` | Identifying the system hostname |
| `pwd` | Displaying the current working directory |
| `uname -a` | Retrieving kernel and operating system information |
| `free -h` | Displaying memory usage |
| `df -h` | Displaying disk space information |
| `ping` | Testing network connectivity |

## 📂 Project Structure

The assignment involved creating two main directory structures.

### 1. General 10alytics Documents

```text
My-10Alytics-Documents/
├── Network-Security/
├── SOC-Analysis/
├── Penetration-Testing/
└── Threat-Intelligence/
```

### 2. 10alytics GRC Documents

```text
My-10Analytics-GRC-documents/
├── Governance-and-Policy/
├── Risk-Assessment/
├── Compliance-Management/
└── Information-Security-Audit/
```

Text-file creation was also included in the assignment using the Nano and Mousepad editors.

## 💻 Practical Exercises and Implementation

### Part 1: Creating Directories

**Objective:** Practise creating and organising directories within the Kali Linux file system.

The exercise involved:

- Creating the main 10alytics documents directory.
- Creating subdirectories for Network Security, SOC Analysis, Penetration Testing, and Threat Intelligence.
- Creating a separate GRC documents directory.
- Organising GRC-related folders covering Governance and Policy, Risk Assessment, Compliance Management, and Information Security Audit.
- Using `ls` to verify directory creation.
- Using text editors to create a `.txt` file within a directory.

**Example commands:**

```bash
mkdir My-10Alytics-Documents

cd My-10Alytics-Documents

mkdir Network-Security
mkdir SOC-Analysis
mkdir Penetration-Testing
mkdir Threat-Intelligence

ls
```

For the GRC directory structure:

```bash
mkdir My-10Analytics-GRC-documents

cd My-10Analytics-GRC-documents

mkdir Governance-and-Policy
mkdir Risk-Assessment
mkdir Compliance-Management
mkdir Information-Security-Audit

ls
```

### Part 2: System Information

**Objective:** Identify the logged-in user, hostname, current working directory, operating system, memory usage, and disk space.

#### Step 1: User and system identification

The following commands were executed individually:

```bash
whoami
hostname
pwd
```

**Observed results:**

| Command | Result |
|---|---|
| `whoami` | kali |
| `hostname` | kali |
| `pwd` | /home/kali |

These commands helped establish the current user account, machine hostname, and working directory.

#### Step 2: Operating system and hardware information

The following commands were used:

```bash
uname -a
free -h
df -h
```

**Observed environment information:**

| Information | Result |
|---|---|
| Linux Distribution | Kali Linux |
| Kernel Version | 6.19.14-1+kali1 |
| Architecture | x86_64 |
| Total RAM | 1.9 Gi |
| Disk Space (assignment summary) | 889 MB |

Additional commands identified in the assignment for exploring system resources included:

```bash
lscpu
uptime
```

These can be used to inspect CPU information and system uptime.

### Part 3: Basic Network Connectivity Test – IP Address

**Objective:** Test connectivity to a known public IP address.

The assignment used Google's public DNS IP address:

`8.8.8.8`

Command executed:

```bash
ping -c 2 8.8.8.8
```

**Observed results:**

| Metric | Result |
|---|---|
| Packets transmitted | 2 |
| Packets received | 2 |
| Packet loss | 0% |
| Average round-trip time | 11.222 ms |

**What this demonstrates:**

- Successful communication with the target IP address.
- Understanding of ICMP echo requests and replies.
- Ability to interpret packet transmission statistics.
- Basic understanding of latency and packet loss.

The `-c 2` option specifies that the ping command should send two packets before stopping.

### Part 4: Basic Network Connectivity Test – Domain Name

**Objective:** Test network connectivity using a domain name and observe DNS resolution.

Command executed:

```bash
ping -c 4 google.com
```

**Observed results:**

| Metric | Result |
|---|---|
| Domain | google.com |
| Resolved IP address | 172.217.76.102 |
| Packets transmitted | 4 |
| Packets received | 4 |
| Packet loss | 0% |
| Average round-trip time | 16.280 ms |

**What this demonstrates:**

- Successful network connectivity using a domain name.
- Automatic resolution of a domain name to an IP address.
- Understanding of the relationship between DNS and network connectivity.
- Ability to interpret ping statistics.

The terminal resolved `google.com` to `172.217.76.102`.

The `-c 4` option specifies that four packets should be transmitted.

The observed average round-trip time differed from the direct IP connectivity test. This illustrates that network response times can vary between tests.

## 📊 Project Results and Key Learnings

The practical exercises successfully demonstrated several foundational Linux and networking concepts.

### Key Results

- Created and verified two organised directory structures.
- Identified the current Linux user as `kali`.
- Identified the hostname as `kali`.
- Retrieved the current working directory: `/home/kali`.
- Retrieved Linux kernel and system information.
- Examined memory and disk usage.
- Successfully tested connectivity to `8.8.8.8`.
- Successfully tested connectivity to `google.com`.
- Observed 0% packet loss in both documented connectivity tests.
- Identified the IP address returned when resolving `google.com`.

### Skills Demonstrated

- Linux command-line navigation.
- Directory and file management.
- Basic Linux system administration.
- System information gathering.
- Memory and disk usage inspection.
- Network connectivity testing.
- DNS resolution fundamentals.
- Command-line troubleshooting.
- Technical documentation and evidence capture.

## 📸 Screenshots and Evidence

The original assignment document contains screenshots demonstrating the practical exercises and their results.

For a more accessible GitHub portfolio, screenshots can be added to a dedicated folder:

```text
linux-fundamentals/
├── README.md
└── screenshots/
    ├── directory-creation.png
    ├── directory-structure.png
    ├── system-information.png
    ├── ping-ip-address.png
    └── ping-domain-name.png
```

Once uploaded, reference them in this README using:

```markdown
![Directory Creation](screenshots/directory-creation.png)

![System Information](screenshots/system-information.png)

![IP Connectivity Test](screenshots/ping-ip-address.png)

![Domain Connectivity Test](screenshots/ping-domain-name.png)
```

*Note: The screenshot filenames above are suggested names. They must match the actual uploaded image filenames.*

## ⚙️ Installation and Setup

This project is a practical Linux exercise rather than a software application requiring installation.

To reproduce the exercises, you will need:

- A computer capable of running Kali Linux.
- Access to a Kali Linux terminal.
- A working network connection for the connectivity tests.

### Step 1: Set up Kali Linux

Install or launch Kali Linux using an appropriate environment, such as:

- A virtual machine.
- An existing Kali Linux installation.
- Another supported Kali Linux environment.

Official documentation:

https://www.kali.org/docs/

### Step 2: Open the terminal

Launch the Kali Linux terminal.

### Step 3: Verify your environment

Run:

```bash
whoami
hostname
pwd
uname -a
```

### Step 4: Reproduce the exercises

Follow the directory creation, system information, and network connectivity commands documented above.

## ▶️ Usage Instructions

This project can be used as a practical learning reference for anyone beginning their Linux and networking journey.

Recommended learning sequence:

1. Start with directory creation and navigation.
2. Practise using `ls`, `mkdir`, and `pwd`.
3. Explore system identification using `whoami` and `hostname`.
4. Retrieve system information using `uname -a`, `free -h`, and `df -h`.
5. Investigate additional system details using `lscpu` and `uptime`.
6. Test network connectivity using `ping`.
7. Compare connectivity tests using an IP address and a domain name.

Experiment with the commands in a safe Linux environment and observe how the output changes.

## 🔐 Cybersecurity Relevance

Linux proficiency is an important foundation for several cybersecurity disciplines.

The skills demonstrated in this project provide introductory knowledge relevant to:

- **Network Security:** Understanding basic network communication and connectivity.
- **Security Operations Centre (SOC):** Developing familiarity with Linux environments and command-line operations.
- **Penetration Testing:** Building foundational Linux command-line knowledge.
- **Governance, Risk and Compliance (GRC):** Understanding system environments and basic technical infrastructure.
- **System Administration:** Learning how to inspect and manage Linux systems.

These exercises represent foundational learning rather than a complete implementation of the security disciplines listed above.

## 🤝 Contributions

Contributions, suggestions, and improvements are welcome.

If you would like to contribute:

1. Fork this repository.
2. Create a feature branch:

   ```bash
   git checkout -b feature/your-improvement
   ```

3. Make your changes.
4. Commit your changes:

   ```bash
   git commit -m "Add your improvement"
   ```

5. Push your branch:

   ```bash
   git push origin feature/your-improvement
   ```

6. Open a Pull Request describing your changes.

Please ensure that contributions are relevant to the project's Linux fundamentals learning objectives.

## 📚 Learning Resources

The following resources can help extend the knowledge covered in this project:

- [Kali Linux Documentation](https://www.kali.org/docs/)
- [Linux Manual Pages](https://man7.org/linux/man-pages/)
- [GNU Coreutils Documentation](https://www.gnu.org/software/coreutils/manual/)
- [Linux Foundation](https://www.linuxfoundation.org/)
- [Cisco Networking Academy](https://www.netacad.com/)

## 👩‍💻 Author

**Dorcas Gbenro**

Aspiring Network Engineer | Cybersecurity Enthusiast | GRC Learner

Location: Wellingborough, United Kingdom

Areas of interest:
- Linux Administration
- Computer Networking
- Network Security
- Cybersecurity
- Governance, Risk and Compliance

GitHub: https://github.com/GBDoc

LinkedIn: www.linkedin.com/in/dorcasgbenro

**Operating System:** Kali Linux  
**Year:** 2026  
**Author:** Dorcas Gbenro

*Building practical Linux, networking, and cybersecurity skills through hands-on learning.*
