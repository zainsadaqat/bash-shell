# Shell / Bash Roadmap: Your Step-by-Step Learning Guide

This roadmap is designed to take you from a complete beginner to proficient in Shell / Bash scripting, which is crucial for development, system administration, and automation.

---

## 1. Introduction to Shell / Bash
### **What is Bash?**

Bash is a scripting language with its own syntax, variables, conditionals (if-else), loops (for, while), and functions.

It allows users to write scripts to automate tasks and perform complex operations, similar to other programming languages.

While it may lack some advanced features of higher-level languages like object-oriented programming, its capabilities are sufficient for system administration, automation, and general scripting within Unix-like environments.

### **CLI vs GUI:** Understanding the command-line interface versus graphical user interfaces.

- CLI: Text-based, requiring users to type commands and arguments into a terminal or console.
- GLI: Visual-based, allowing users to interact with elements like icons, menus, and windows using a pointing device.

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

### **Files & Directories:** Core commands for navigating and managing files.

Navigate between dirs: Tips for efficient directory traversal


#### `pwd`: Print Working Directory
Knowing which folder you're in is important when moving around the filesystem. It helps you make sure you're in the right place when running commands that use relative paths.



#### `cd`: Change Directory

The cd command supports several useful options for navigating directories:

- cd ..: Move up one directory level
- cd ~: Change to the home directory
- cd -: Switch to the previous directory
- cd /: Change to the root directory

- `echo`: Display text or variables
- `mkdir`: Make Directory
- `touch`: Create empty files or update timestamps
- `rm`: Remove files or directories
- `rmdir`: Remove empty directories
- `mv`: Move or rename files

#### `cp`: Copy files and directories

The cp command is used to copy files and directories from one location to another

It's like making a duplicate of your file or folder.

#### `cat`: Concatenate and display file content

The cat command is used to show the content of files in the terminal.

You can also use it to combine multiple files into one.

The cat command has options to change how it shows text:

The cat command can be used to concatenate multiple files into one.

This is useful for combining files or appending content to an existing file.

```sh
cat file1.txt file2.txt > combined.txt
```

-n - Add numbers to each line
-b - Add numbers only to lines with text
-s - Remove extra empty lines
-v - Show non-printing characters (except for tabs and end of line)

- `find`: Search for files in a directory hierarchy
    
 


### `ls`: List directory contents
- The `ls` command is used to list the contents of a directory.
- The `ls` command can display files, directories, and information about them.

### ls Parameter Options
The `ls` command has a variety of options to customize its output:

#### `-l` - Long listing format

The -l option gives you detailed information about files and folders.

It displays information such as:

- file permissions
- number of links
- owner name
- owner group
- file size
- time of last modification
- file or directory name

```sh
-rw-r--r--  1 zain  staff  20 Nov 10 10:25 hello.sh
```
- The letters after the first character show who can read or write the file. Think of them as permission tags.
- The number one is the link count.
- zain is the owner.
- staff is the group.
- twenty is the size of the file in bytes.
- Then the date and time the file was last changed.
- hello.sh is the file name.

#### `-a` - Include hidden files

Hidden files in Unix/Linux systems start with a dot (e.g., `.configts.json`).

This option is helpful when you need to view or manage configuration files that are not visible by default.

#### `-h` - Human-readable sizes

The -h option makes file sizes easier to read by converting byte counts into kilobytes (K), megabytes (M), gigabytes (G), etc.

This option is particularly useful when you want to quickly assess the size of files and directories without manually converting bytes.

```sh
ls -lh
```
#### -t - Sort by modification time

The -t option sorts files and directories by modification time, with the most recently modified files first.

This option is useful when you want to see the most recently updated files first.

#### -r - Reverse order while sorting

The -r option reverses the order of the sort.

When used in combination with other options like -t, it can display the oldest files first.

This option is useful for reversing the default sorting behavior to meet specific needs

#### -R - List subdirectories recursively

The -R option lists directories and their contents recursively.

This is useful for viewing the entire directory tree.

#### -S - Sort by file size

The -S option sorts files by size, with the largest files first.

This is helpful for quickly identifying large files in a directory.

#### -1 - List one file per line

The -1 option lists one file per line, which is useful for scripts or when piping output to other commands.

#### -d - List directories themselves, not their contents

The -d option lists directories themselves rather than their contents.

This is useful for seeing directory names without contents.

#### -F - Append indicator (one of */=@|) to entries

The -F option appends an indicator character to entries (e.g., / for directories, * for executables).

#### Combine Multiple Options

You can combine multiple options to create more complex commands.

For example, `ls -l -a` will display a detailed listing of all files and directories, including hidden files.

You can also combine multiple options without a space between them. For example, ls -la


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
### **View & Search:**
#### `grep`: Search for patterns in files.

The grep command is used to search for text patterns within files.

It's a powerful way to find specific text in large files or across many files.

To search for a pattern in a file, use grep 'pattern' filename

The grep command has options to change how it works:

- -i - Search ignoring case differences (uppercase or lowercase)
- -r - Search through all files in a directory and its subdirectories
- -v - Find lines that do not match the pattern

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
