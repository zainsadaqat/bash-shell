# Shell / Bash Roadmap: Your Step-by-Step Learning Guide

This roadmap is designed to take you from a complete beginner to proficient in Shell / Bash scripting, which is crucial for development, system administration, and automation.

---

## 1. Introduction to Shell / Bash
*   **What is Bash?**
*   **CLI vs GUI:** Understanding the command-line interface versus graphical user interfaces.
*   **What is scripting?**

## 2. Popular Shells
*   **dash**
*   **bash**
*   **zsh**
*   **fish**
*   **tcsh**
*   **ksh**
*   **cmd**
*   **PowerShell**

## 3. Setting Up Bash
*   Get your environment ready to start scripting.

## 4. Shell Fundamentals
*   **Files & Directories:** Core commands for navigating and managing files.
    *   `pwd`: Print Working Directory
### `ls`: List directory contents
- The `ls` command is used to list the contents of a directory.
- The `ls` command can display files, directories, and information about them.
    *   `cd`: Change Directory
    *   `echo`: Display text or variables
    *   `mkdir`: Make Directory
    *   `touch`: Create empty files or update timestamps
    *   `rm`: Remove files or directories
    *   `rmdir`: Remove empty directories
    *   `mv`: Move or rename files
    *   `cp`: Copy files and directories
    *   `cat`: Concatenate and display file content
    *   `find`: Search for files in a directory hierarchy
    *   Navigate between dirs: Tips for efficient directory traversal
*   **Tab Completion:** Speed up your typing and reduce errors.
*   **Repeat Commands:** Efficiently re-run previous commands.
*   **Help Commands:** Learn how to get help for any command (`man`, `help`).
*   **Bash Alias:** Create shortcuts for frequently used commands.
*   **Stop Execution:** How to stop a running command (`Ctrl+C`).
*   **Redirects & Pipelines:** Control the flow of input and output.
    *   `stdin`, `stdout`, `stderr`: Standard input, output, and error streams.
    *   Output redirection (`>`, `>>`)
    *   Input redirection (`<`)
    *   Error redirection (`2>`, `&>`)
    *   Pipes (`|`): Connect command outputs to inputs.
    *   Command substitution (`` `command` `` or `$(command)`)
    *   Process substitution (`<(command)`)

## 5. Working with Text
*   **View & Search:**
    *   `grep`: Search for patterns in files.
    *   `less`, `more`: View file content page by page.
    *   `head`, `tail`: View the beginning or end of files.
    *   `find`: (Also used for text searching within files)
*   **Text Transform:**
    *   `cut`, `paste`: Manipulate columns of text.
    *   `join`, `split`: Combine or divide files based on common fields or size.
    *   `tr`: Translate or delete characters.
    *   `sed`: Stream Editor for filtering and transforming text.
    *   `awk`: Pattern scanning and processing language.
*   **Analysis:**
    *   `wc`: Word Count (lines, words, characters).
    *   `sort`: Sort lines of text files.
    *   `uniq`: Report or omit repeated lines.
    *   `nl`: Number lines of files.
*   **Wildcards:** Pattern matching for file names.
    *   `*`: Match any sequence of characters.
    *   `?`: Match any single character.
    *   `[...]`: Match any character within the brackets.
    *   `{...}`: Brace expansion for generating arbitrary strings.

## 6. Text Editors
*   **Nano**
*   **Vim**
*   **Emacs**
*   **Vi**
*   **Basic Editor Ops.** (common functions across editors)

## 7. Bash Script Anatomy
*   Understand the basic structure of a Bash script.

## 8. Running Shell Scripts
*   **Direct Execution:** Running scripts as executable files.
*   **Running with Bash:** Explicitly running scripts with `bash script.sh`.
*   **Running with Source:** Executing scripts in the current shell environment.

## 9. Variables
*   **Environment vs Shell vars.**
*   **Create, Print, Modify:** How to declare, display, and change variables.
*   **Variable Scopes:** Understanding local and global variables.
*   **Special variables:** `$?, $$, $!, $0, $1`, etc.
*   **Variables best practices:** Naming, quoting, and usage.

## 10. Bash Data Types
*   **Strings**
*   **Numeric**
*   **Arrays**
*   **Associative Arrays**

## 11. Comments
*   How to add comments (`#`) to your scripts for readability.

## 12. Bash Operators
*   **Arithmetic:** Perform calculations.
*   **Comparison:** Compare values.
*   **String operators:** Work with strings.
*   **Logical:** Combine conditions (`&&`, `||`, `!`).
*   **File test:** Check file attributes (existence, permissions, type).

## 13. Input/Output
*   **Read user input:** Get input from the user (`read`).
*   **printf formatting:** Formatted output.
*   **Here documents (`<<`):** Multiline input for commands.
*   **Here strings (`<<<`):** Single-line input for commands.

## 14. Working with Numerics
*   **Arithmetic expansion (`$((...))`):** Basic integer arithmetic.
*   `expr`: Evaluate expressions.
*   `bc`: Arbitrary precision calculator language.
*   `let`: Perform arithmetic operations.
*   `awk`: Can also be used for numerical computations.

## 15. String Manipulation
*   **String length:** Get the length of a string.
*   **Substring extraction:** Extract parts of a string.
*   **Pattern replacement:** Replace parts of a string using patterns.
*   **Case conversion:** Change string case (upper/lower).

## 16. Exit Codes
*   `$?`: Check the exit status of the last command.
*   `exit`: Terminate a script with a specific exit status.
*   **Success vs failure:** Convention of exit codes (0 for success, non-zero for failure).

## 17. Script Arguments
*   `$1`, `$2`, `$3`: Access individual arguments.
*   `$0`: The name of the script itself.
*   `$@`: All positional arguments as separate strings.
*   `$*`: All positional arguments as a single string.
*   `$#`: The number of positional arguments.
*   `shift`: Shift positional parameters to the left.

## 18. File Permissions
*   `rwx`: Read, Write, Execute permissions.
*   `chmod`: Change file permissions.
*   `chown`: Change file owner.
*   `chgrp`: Change file group.

## 19. Conditionals
*   `if`: Execute code conditionally (`if...then...fi`, `if...else...fi`, `if...elif...else...fi`).
*   `case`: Multi-way branching based on pattern matching.

## 20. Loops
*   `for`: Iterate over a list of items.
*   `while`: Loop as long as a condition is true.
*   `until`: Loop until a condition is true.
*   `break`, `continue`: Control loop execution.

## 21. Functions
*   Define and use functions to modularize code.
*   **Function Scopes:** Understanding local variables within functions.
*   **Recursive Functions:** Functions that call themselves.

## 22. Error Handling
*   `set -e`: Exit immediately if a command exits with a non-zero status.
*   `set -o` (various options): Configure shell behavior.
*   `set -u`: Treat unset variables as an error.
*   `trap`: Execute commands upon receipt of signals.
*   **Error logging:** Techniques for logging errors from scripts.

## 23. Debugging
*   `set -x`: Print commands and their arguments as they are executed.
*   `bash -n`: Check syntax without executing.
*   `shellcheck`: A static analysis tool for shell scripts.

## 24. Regular Expressions
*   **Basic regex syntax**
*   **Extended regex**

## 25. Process Management
*   `jobs`: List active jobs.
*   `nohup`: Run a command immune to hang-ups, with output to a non-tty.
*   `fg`, `bg`: Bring jobs to foreground or send to background.
*   `disown`: Remove jobs from the shell's job control.
*   **Process substitution:** Pass the output of a command as a file to another command.

## 26. System Admin.
*   **System Monitoring:**
    *   `ps`: Report a snapshot of the current processes.
    *   `top`, `htop`: Display Linux processes (interactive).
    *   `free`: Display amount of free and used memory.
    *   `df`, `du`: Report file system disk space usage.
    *   `uptime`: Tell how long the system has been running.
    *   `iostat`, `vmstat`: Report CPU, I/O, and memory statistics.
*   **Task Scheduling:**
    *   `cron`, `crontab`: Schedule commands to run periodically.
    *   `at`: Schedule commands to run once at a specified time.
    *   `systemd timers`: Modern Linux service for scheduling tasks.

## 27. Package Management
*   `apt`: Debian/Ubuntu package manager.
*   `brew`: macOS (Homebrew) package manager.
*   `yum`: Red Hat/CentOS package manager.
*   `dnf`: Modern Fedora package manager.

## 28. Networking
*   `ping`: Send ICMP ECHO_REQUEST to network hosts.
*   `curl`: Transfer data from or to a server.
*   `wget`: Non-interactive network downloader.
*   `ssh`: Secure Shell client (remote login program).
*   `scp`: Secure Copy (file transfer over SSH).
*   `rsync`: Remote file and directory synchronization.
*   `netstat`, `ss`: Network statistics and sockets info.
*   `ifconfig`, `ip`: Configure network interfaces.

## 29. File Compression
*   `tar`: Archiver utility.
*   `zip`, `unzip`: Compress/decompress files.
*   `gzip`, `gunzip`: GNU zip compression/decompression.
*   `bzip2`, `xz`: Other compression utilities.
