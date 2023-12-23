# Jsh Shell for Job Control
[![Job-Control-Shell-Emulator](https://github.com/mathusanMe/Job-Control-Shell-Emulator/actions/workflows/main.yml/badge.svg)](https://github.com/mathusanMe/Job-Control-Shell-Emulator/actions/workflows/main.yml)

As part of our Operating Systems course, our team is ambitiously crafting an advanced shell emulator. This project, a work-in-progress as of December 2023, focuses on sophisticated job control and system call integration, specifically tailored for Linux environments.

Our team, consisting of three dedicated members, is utilizing the C programming language for development. We leverage the robustness of the [GNU Compiler Collection (GCC)](https://gcc.gnu.org/) and the efficiency of the [GNU Make](https://www.gnu.org/software/make/) build automation tool. To ensure the reliability and stability of our shell emulator, we are also employing the [Valgrind](https://valgrind.org/) tool for meticulous memory debugging. An integral part of our development process is the continuous integration (CI) pipeline, hosted and managed via GitHub Actions.

## Table of Contents
1. [Description](#description)
2. [Visual Previews](#visual-previews)
3. [Getting Started](#getting-started)
4. [Usage Instructions](#usage-instructions)
5. [Testing](#testing)
6. [Debugging](#debugging)

## Description
Our shell emulator, developed in C, is a compact yet powerful tool, designed with an emphasis on advanced job control and seamless system call integration. Optimized for Linux systems, it supports an array of features and commands:

### Supported Commands
- Navigation (`cd`)
- Display current directory (`pwd`)
- Exit functionality (`exit`)
- Last command exit value (`?`)
- Execution of external commands

### Advanced Features
- Command history logging
- Comprehensive job control
- Input/Output redirection
- Piping capabilities
- Management of background processes
- Efficient signal handling

## Visual Previews

<p align="center">
  <img src="images/job-control-shell.png" alt="Job Control Shell">
  <br>
  <sub>Job Control Shell</sub>
</p>

<br>

<p align="center">
  <img src="images/basic-prompt-view.jpeg" alt="Basic Prompt View">
  <br>
  <sub>Basic Prompt View</sub>
</p>

<br>

<p align="center">
  <img src="images/listing-files.jpeg" alt="Listing Files">
  <br>
  <sub>Listing Files</sub>
</p>

<br>

<p align="center">
  <img src="images/date.jpeg" alt="Executing an External Command: Date">
  <br>
  <sub>Executing an External Command: Date</sub>
</p>

<br>

<p align="center">
  <img src="images/redirections.jpeg" alt="I/O Redirections">
  <br>
  <sub>I/O Redirections</sub>
</p>

<br>

<p align="center">
  <img src="images/jobs.jpeg" alt="Jobs">
  <br>
  <sub>Jobs</sub>
</p>

## Getting Started

### System Requirements
- **Operating System**: Linux-based or use Docker (Dockerfile provided).
- **Required Tools & Packages**: 
  - [GNU Compiler Collection (GCC)](https://gcc.gnu.org/) 
  - [GNU Make](https://www.gnu.org/software/make/)
  - [GNU Debugger (GDB)](https://www.gnu.org/software/gdb/)
  - [Valgrind](https://valgrind.org/)
  - [Git](https://git-scm.com/)
  - [Clang-Format](https://clang.llvm.org/docs/ClangFormat.html)
  - [libreadline-dev](https://packages.debian.org/sid/libreadline-dev)

### Installation Guide
1. **Clone the Repository**: First, clone the repository to your local machine.
2. **Compilation**: Open your terminal and navigate to the cloned repository's directory. Compile the project by executing:
   ```bash
   make all
   ```

## Usage Instructions
- **Running the Shell Emulator**: To start the shell, enter the following command in your terminal:
  ```bash
  make run
  ```
- **Cleaning the Project**: To remove all compiled files, use:
  ```bash
  make clean
  ```

## Testing
- **Running Tests**: For testing, execute:
  ```bash
  make test
  ```

This will run the provided test suite to ensure everything is functioning correctly.

## Debugging
- **GNU Debugger**: To debug the shell emulator using GDB, execute:
  ```bash
  make gdb
  ```
