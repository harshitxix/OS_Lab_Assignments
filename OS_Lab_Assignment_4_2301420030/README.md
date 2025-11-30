# 🧠 ENCS351 – Operating Systems Lab (Sheet 4)

## 📋 Overview
This repository contains all the tasks and outputs for **ENCS351 – Operating Systems Lab (Sheet 4)**.  
Each task demonstrates a key concept of operating system functionality, including process management, inter-process communication, scheduling, and virtual machine detection.

---

## 👤 Student Information
**Name:** Harshit Chauhan  
**Program:** B.Tech (CSE – Data Science)  
**University:** K.R. Mangalam University  
**Date Submitted:** *[Insert Date]*  

---

## 🧩 Task Details

### 🧱 Task 1 – Batch Processing
**Approach:** Sequential subprocess execution of Python scripts.  
**Evidence:** `screenshots/task1.png`  
**Output:** `outputs/task1_batch_output.txt`

> Demonstrates simple batch job execution — scripts are run one after another in sequence.

---

### ⚙️ Task 2 – System Startup & Logging
**Approach:** Used Python’s `multiprocessing` module to spawn processes and log their lifecycle to a file.  
**Evidence:** `screenshots/task2.png`  
**Output:** `outputs/system_log.txt`

> Simulates an operating system startup process with process creation and lifecycle logging.

---

### 🔗 Task 3 – System Calls & Inter-Process Communication (IPC)
**Approach:**  
- **C Program:** Demonstrates `fork()`, `exec()`, `wait()`, and `pipe()`.  
- **Python Alternative:** Uses `os.pipe()` and `os.fork()` for IPC demonstration.  
**Evidence:** `screenshots/task3_exec.png`, `screenshots/task3_pipe.png`  
**Outputs:** `outputs/task3_exec.txt`, `outputs/task3_pipe.txt`

> Highlights process creation, execution replacement, synchronization, and communication mechanisms.

---

### 💻 Task 4 – VM Detection & Shell Interaction
**Approach:**  
- **sysinfo.sh:** Prints kernel, user, and virtualization info.  
- **vm_detect.py:** Detects VM using `systemd-detect-virt`, CPU hypervisor flags, and DMI strings.  
**Evidence:** `screenshots/task4.png`  
**Outputs:** `outputs/task4_sysinfo.txt`, `outputs/task4_vmdetect.txt`

> Uses multiple heuristic checks to determine whether the system is virtualized or running on physical hardware.

---

### 🧮 Task 5 – CPU Scheduling Algorithms
**Approach:** Implemented classic CPU scheduling algorithms:
- FCFS (First Come First Serve)
- SJF (Shortest Job First)
- RR (Round Robin)
- Priority Scheduling  

Calculates **Waiting Time (WT)**, **Turnaround Time (TAT)**, and their averages.  
**Evidence:**  
`screenshots/task5_fcfs.png`, `screenshots/task5_sjf.png`, `screenshots/task5_rr.png`, `screenshots/task5_priority.png`  
**Outputs:** `outputs/task5_*.txt`

> Compares performance and fairness across different scheduling techniques.

---

## 📘 Observations & Learnings
- **Batch Processing:** Simulates simple job queues and sequential task execution.  
- **Logging:** Helps visualize process lifecycles similar to OS boot/shutdown events.  
- **System Calls & IPC:** `fork`, `exec`, and `wait` demonstrate address space isolation; pipes enable communication between processes.  
- **VM Detection:** Combines system tools and hardware inspection for reliable virtualization detection.  
- **Scheduling:** Each policy offers trade-offs between turnaround time and fairness — Round Robin improves responsiveness; SJF minimizes average waiting time when burst lengths are known.

---

## 🧾 References
- Linux Man Pages: [`fork(2)`](https://man7.org/linux/man-pages/man2/fork.2.html), [`exec(3)`](https://man7.org/linux/man-pages/man3/exec.3.html), [`wait(2)`](https://man7.org/linux/man-pages/man2/wait.2.html), [`pipe(2)`](https://man7.org/linux/man-pages/man2/pipe.2.html)  
- [Python Docs – multiprocessing](https://docs.python.org/3/library/multiprocessing.html)  
- [Python Docs – subprocess](https://docs.python.org/3/library/subprocess.html)  
- [Python Docs – os](https://docs.python.org/3/library/os.html)
