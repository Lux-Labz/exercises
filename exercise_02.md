# Running a "Hello World" Script from the Xubuntu Command Line

Welcome to the **Xubuntu Hello World Script Guide**! In this tutorial, you’ll learn how to create and run your very first "Hello World" script using the Xubuntu command line. It’s a simple and fun way to get started with programming. Let’s dive in!

## Table of Contents
- [Introduction](#introduction)
- [What You'll Need](#what-youll-need)
- [Step 1: Open the Terminal](#step-1-open-the-terminal)
- [Step 2: Create a Hello World Script](#step-2-create-a-hello-world-script)
- [Step 3: Make the Script Executable](#step-3-make-the-script-executable)
- [Step 4: Run the Script](#step-4-run-the-script)
- [Conclusion](#conclusion)

---

## Introduction

In this guide, we’ll create a basic script that displays the message "Hello, World!" when run. You’ll see just how easy it is to write and execute a simple script in Xubuntu, which is a user-friendly version of Linux.

## What You'll Need

- A **computer with Xubuntu installed**.
- **Access to the terminal** (command line).
- A positive attitude — you’re going to do great! 😄

---

## Step 1: Open the Terminal

Let’s start by opening the terminal. This is where you’ll type commands to interact with your system.

1. Click the **Applications Menu** in the top left corner of your screen.
2. Search for **Terminal** and click it to open.

You should now see a terminal window where you can enter your commands. You’re already on the right track!

---

## Step 2: Create a Hello World Script

Now that you’ve got the terminal open, let’s create the script.

1. In the terminal, type the following command to open a text editor called **nano**:
    ```bash
    nano hello_world.sh
    ```

2. You are now inside the nano editor. Type the following lines of code:
    ```bash
    #!/bin/bash
    echo "Hello, World!"
    ```

3. Once you’ve typed the code, press `CTRL + O` to save the file.
4. Hit `Enter` to confirm the file name.
5. Press `CTRL + X` to exit nano.

Awesome! You’ve just written your first script.

---

## Step 3: Make the Script Executable

Before you can run your script, you need to make it executable. This means giving it permission to run as a program.

1. In the terminal, type the following command:
    ```bash
    chmod +x hello_world.sh
    ```

This command gives the script the necessary permissions to be executed. You’re almost there!

---

## Step 4: Run the Script

Now for the exciting part — running your "Hello World" script!

1. In the terminal, type:
    ```bash
    ./hello_world.sh
    ```

You should see the following output:

Hello, World!
