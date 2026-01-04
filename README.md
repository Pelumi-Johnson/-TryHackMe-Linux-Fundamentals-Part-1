# 🐧 TryHackMe – Linux Fundamentals Part 1  
### Hands-On Linux Command Line Practice

📄 **Full Lab Report (Google Doc):**  
👉 [Click here to open the complete lab report](https://github.com/Pelumi-Johnson/-My-Local-Network-Home-Topology-Lab/blob/main/1.5.4%20Lab%20-%20My%20Local%20Network-1.docx%20(1).pdf)

## 📘 Overview
This repository documents my completion of the **TryHackMe – Linux Fundamentals Part 1** room.  
The purpose of this lab was to build foundational Linux skills through direct, hands-on interaction with a Linux system using the command line.

All actions were performed on a **live Ubuntu Linux machine** deployed directly in the browser through TryHackMe. This was not a simulation or theory only exercise, every command shown was executed in a real Linux environment.

This lab introduced how Linux systems are structured, how users interact with them, and how files, directories, logs, and commands are managed through the terminal.

## 🧰 Environment
- **Platform:** TryHackMe (In-Browser Machine)  
- **Operating System:** Ubuntu 20.04 LTS  
- **Shell:** Bash  
- **User Account:** `tryhackme`

## 🧭 Step 1: Introduction to Linux
I began by learning what Linux is and where it is commonly used. Linux is an open-source operating system widely deployed across servers, cloud environments, embedded systems, point of sale systems, mobile devices, and critical infrastructure.

I learned that Linux is not a single operating system, but an umbrella term for many distributions (distros) such as Ubuntu and Debian. For this lab, Ubuntu was used.

I also researched the history of Linux and confirmed that the first Linux operating system was released in **1991**.

## ▶️ Step 2: Starting the Linux Machine
I deployed the Ubuntu Linux machine provided by TryHackMe directly in the browser.

Once the machine started, I was presented with a terminal interface — the primary way administrators, engineers, and security professionals interact with Linux systems.

## ⌨️ Step 3: Basic Command Interaction
I practiced issuing basic commands to understand how the terminal works and how Linux responds to user input.

Commands used:
- `echo`
- `whoami`

Using `echo`, I printed text to the terminal to confirm command execution.  
Using `whoami`, I identified the active user account I was logged in as.

This confirmed that I was operating as the user **tryhackme**, reinforcing the importance of understanding user context in Linux environments.

## 📂 Step 4: Navigating the Filesystem
I learned how Linux organizes files and directories and how to move through them using the terminal.

Commands used:
- `pwd`
- `ls`
- `cd`
- `cd ..`

Using `pwd`, I displayed the full path of my current working directory.  
Using `ls`, I listed the files and folders within directories.  
Using `cd`, I moved into specific directories, and `cd ..` allowed me to return to the parent directory.

Through this, I learned how Linux paths work and how directories such as `/home/tryhackme` are structured.

## 📝 Step 5: Creating and Viewing Files
I practiced creating files and viewing their contents directly from the command line.

Commands used:
- `echo "text" > filename`
- `cat filename`

Using output redirection (`>`), I created files and wrote text into them.  
Using `cat`, I displayed the contents of files directly in the terminal.

This demonstrated how Linux treats nearly everything as a file and how simple commands can manipulate file contents efficiently.

## 🔍 Step 6: Searching Files with `grep`
I learned how to search through files efficiently using the `grep` command, which is especially important when dealing with logs.

Command used:
- `grep "THM" access.log`

Using `grep`, I searched through a web server access log to find entries containing a specific pattern.

This allowed me to successfully locate the embedded flag:
`THM{ACCESS}`

This step highlighted how logs can be analyzed to extract meaningful information. A key skill in cybersecurity and incident response.

## 🔁 Step 7: Output Redirection & Command Operators
I learned how Linux handles command output and how that output can be redirected or controlled using operators.

Operators learned:
- `>`  – overwrite file contents  
- `>>` – append to file contents  
- `;`  – run commands sequentially  
- `&&` – run the next command only if the previous command succeeds  
- `&`  – run a command in the background  

Commands used:
- `echo password123 > passwords`
- `echo tryhackme >> passwords`

Using `>`, I replaced the contents of a file.  
Using `>>`, I appended additional content without overwriting existing data.

## 🔗 Step 8: Command Chaining with `;`
I learned how to connect multiple commands using the semicolon operator.

Example:
- `commandA ; commandB`

Command A runs first, and Command B runs immediately after, regardless of whether Command A succeeds or fails. This is useful when commands are independent and need to run sequentially.

## ✅ Step 9: Conditional Execution with `&&`
I learned how to chain commands conditionally using the `&&` operator.

Example:
- `commandA && commandB`

Command B only runs if Command A completes successfully. This ensures controlled execution and is commonly used in installations, updates, and automation scripts.

## 🕒 Step 10: Background Execution with `&`
I learned how to run commands in the background while continuing to use the terminal.

Example:
- `command &`

This allows long-running processes to execute while still allowing other commands to be run in the same terminal session.

## 🧪 Step 11: Practical Reinforcement
I applied all learned commands directly on the live Linux machine, reinforcing:
- User awareness  
- Directory navigation  
- File creation and modification  
- Log searching  
- Output redirection  
- Command chaining and background execution  

Each task was validated through TryHackMe’s built-in checks.

## 🏁 Completion
I successfully completed all tasks in the **TryHackMe Linux Fundamentals Part 1** room.

Completion confirms:
- Understanding of basic Linux concepts  
- Ability to navigate and interact with a Linux system  
- Comfort using foundational command-line tools  
- Readiness to move on to more advanced Linux topics  

## 🧠 Key Takeaways
- Linux is precise and unforgiving, but extremely powerful when used intentionally  
- The terminal becomes approachable once its structure is understood  
- Logs tell stories, and tools like `grep` help uncover them  
- Small commands build the foundation for advanced security operations  

  


