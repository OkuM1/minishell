
# Minishell

Welcome to **Minishell**! This project is part of the 42 school curriculum and challenges students to implement a Unix-like shell from scratch in C. This shell supports many features of real-world shells, such as parsing and executing commands, handling input/output redirection, and managing processes. 

The **Minishell** project is a fantastic opportunity to dive into system-level programming, understand process management, and improve C programming skills. Here’s a look at the key achievements and features that this implementation brings to the table.

---

## Table of Contents

- [About the Project](#about-the-project)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Achievements](#achievements)
- [License](#license)

---

## About the Project

**Minishell** is a simplified shell designed to mimic the behavior of common Unix shells, such as Bash. It was developed as part of the 42 school curriculum to deepen understanding of command-line interfaces and core shell functionality. The project is a blend of low-level programming, process handling, and Unix system calls.

### Project Objectives
- Recreate a simple command-line interpreter with features like command parsing, process management, and signal handling.
- Handle complex user inputs, implement redirections, pipelines, and manage child processes.
- Gain hands-on experience with C programming in a system-level environment.

---

## Features

This implementation of Minishell includes the following features:

1. **Command Parsing**  
   - Supports complex command parsing including pipes `|`, redirections `>`, `<`, and `>>`.
   - Handles multiple commands on a single line separated by semicolons `;`.

2. **Builtin Commands**  
   - Implements several built-in commands, such as `echo`, `cd`, `pwd`, `export`, `unset`, `env`, and `exit`, with behavior mimicking that of standard shells.

3. **Environment Variable Management**  
   - Supports setting, updating, and retrieving environment variables.
   - Integrates variables directly into commands and parsing to ensure smooth user interaction.

4. **Error Handling**  
   - Implements robust error handling for invalid commands, incorrect syntax, and undefined behavior.
   - Provides informative error messages similar to those found in a Unix shell.

5. **Signal Management**  
   - Responds to `SIGINT` (Ctrl+C), `SIGQUIT`, and `SIGTSTP` signals.
   - Ensures safe handling and termination of processes when signals are sent.

6. **Pipelines and Redirections**  
   - Enables piping output from one command to another (`ls | grep minishell`).
   - Implements input and output redirections, including `>`, `<`, and `>>` for files.

---

## Installation

To install Minishell, clone the repository and compile the source code:

```bash
git clone https://github.com/OkuM1/minishell.git
cd minishell
make
```

This will create an executable named `minishell` in the project directory.

---

## Usage

Once compiled, start Minishell by running the following command:

```bash
./minishell
```

The shell supports both built-in and external commands and many more features. Here are a few examples:

```bash
minishell$ echo Hello, Minishell!
minishell$ pwd
minishell$ ls | grep minishell
minishell$ export PATH=/new/path:$PATH
minishell$ exit
```

---

## Achievements

During the development of **Minishell**, several technical challenges were overcome to implement a fully functional shell environment. Here are the main achievements:

- **Advanced Command Parsing**: Implemented a custom parser to handle complex command structures involving pipelines and redirections, ensuring compatibility with Unix-like syntax.
- **Process and Signal Management**: Learned to manage processes effectively, handling background and foreground processes with real-time signal handling for a seamless user experience.
- **Robust Error Management**: Built custom error messages and handling routines to provide clear feedback, closely resembling the error responses of actual Unix shells.
- **System-Level Programming Expertise**: Gained in-depth understanding of system calls, particularly in areas of process management, file I/O, and inter-process communication.
- **Optimized Resource Usage**: Employed efficient memory management practices, ensuring minimal memory leaks and optimal resource usage even with heavy command sequences.
- **Enhanced Shell Features**: Implemented user-friendly shell features like environment variable expansion and built-in command support for enhanced usability.

---

## License

Distributed under the MIT License. See `LICENSE` for more information.

---

Thank you for exploring **Minishell**! This project was a rewarding experience, offering insight into the inner workings of shell environments and system-level programming. Contributions and suggestions are welcome—feel free to fork this repository and create pull requests to improve the project.

---
