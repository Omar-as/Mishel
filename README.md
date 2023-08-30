# Mishell - Unix-Style Operating System Shell

Mishell is an interactive Unix-style operating system shell developed as part of COMP 304 - Operating Systems course project. This shell allows users to execute commands, both built-in and external, while providing features such as I/O redirection, background execution, and custom commands. It also includes a unique command to visualize process trees using a kernel module. This README provides essential information about the project structure, usage, and functionality.

## Table of Contents
- [Dependencies](#dependencies)
- [Features](#features)
- [Project Structure](#project-structure)
- [License](#license)

## Dependencies:
- gcc 12.2.0
- dwarfs
- pahole
- python310
- linuxHeaders
- graphvis

## Features
Mishell offers the following features:

### Interactive Command-Line Interface
Mishell provides an intuitive command-line interface for users to interact with the operating system.

### Execution of External Programs
Run external programs seamlessly by entering the program name and arguments.

### Background Execution
Execute programs in the background using the '**&**' symbol to keep the shell responsive.

### Built-in Commands
Mishell includes the following built-in commands:

- **cd**: Change the current working directory.
- **exit**: Terminate the Mishell session.
- **cdh**: List recent directories for easy navigation.
- **roll**: Simulate rolling dice and display the results.
- **cloc**: Count lines of code in source files.

### I/O Redirection
Redirect input and output using the `>` and `>>` operators to customize data flow.

### Visualization of Process Trees
Use the `psvis` command to visualize process trees. This command:

- Uses a kernel module to find subprocess trees.
- Generates a human-friendly graph of processes.
- Highlights heir nodes with a distinct color.
- Requires superuser privileges for kernel module interaction.

## Project Structure
The project is organized as follows:

- **src**: Source code files.
- **Makefile**: Build automation script.
- **kernel_module**: Kernel module for process tree visualization.

## License
This project is licensed under the [MIT License](LICENSE).
