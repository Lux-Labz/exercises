<!-- 
{
  "ID": "2739183746",
  "Title": "Linux Fun with Package Management",
  "Tags": ["Linux", "Ubuntu", "Package Management", "Beginner", "STEM"],
  "Description": "A beginner-friendly exercise to learn Linux package management using sl, ninvaders, and cmatrix as fun examples.",
  "Query": "You are a STEM instructor and training exercise curriculum creator for students aged 12-18. Geneate a training exercise with the following content: Package managment using sl, ninvaders, and cmatrix as examples. The focus area of this exercise is: Linux. The difficulty level of the exercise is: Beginner. The target operating system is:  Ubuntu. Make the exercise clear, positive, detailed, and comprehensive.  Each step of the excercise must be chronologically numbered.  Include a hidden section, an overview section, and a prerequisite section befrore the exercise section.  Include a summary section and a follow-up section after the exercise section. The hidden section is wrapped in an HTML style comment tag and includes the following parameters in json format: ID, Title, Tags, Description, Query, Model, Focus, Level, Date, Links, Filename. Where ID is a randomly generated 32 bit unique ID; Where title is a short title of the exercise; Where Tags is a list of tags associated with the exercise; Where Description is a short overview description of the exercise; Where Query is this query string; Where model is the model and version of this LLM; Where focus is the focus area of this exercise; Where level is the skill level of this exercise; Where date is the current date in the format yyyymmdd; Where Links is a list of helpful web links and resources related to this exercise; Where Filename is a short unique descriptive name for this markdown file.",
  "Model": "GPT-5",
  "Focus": "Linux",
  "Level": "Beginner",
  "Date": "20250910",
  "Links": [
    "https://ubuntu.com/tutorials/command-line-for-beginners",
    "https://help.ubuntu.com/community/AptGet/Howto",
    "https://manpages.ubuntu.com/"
  ],
  "Filename": "linux_package_management_fun_exercise.md"
}
-->

# Training Exercise: Linux Fun with Package Management

## Overview

In this exercise, you will learn the basics of **package management in Ubuntu Linux**. We’ll use three fun example programs:

* **sl**: A playful command that makes a steam locomotive run across your terminal.
* **ninvaders**: A retro arcade-style space invaders clone.
* **cmatrix**: A program that simulates the "Matrix" digital rain effect.

By the end of this activity, you’ll understand how to install, run, and remove software using Ubuntu’s package management system (`apt`).

---

## Prerequisites

Before starting, make sure you have the following:

1. A computer running **Ubuntu Linux** (or Ubuntu in a virtual machine).
2. Access to the **Terminal** (press `Ctrl + Alt + T` to open it).
3. An internet connection (needed to download packages).
4. Basic familiarity with typing commands into the terminal (no prior Linux experience required).

---

## Exercise Steps

### Part 1: Updating the Package List

1. Open your terminal (`Ctrl + Alt + T`).
2. Type the following command to update the package list:

   ```bash
   sudo apt update
   ```
3. Press **Enter**. The system may ask for your password—type it and press **Enter** again.

   * This step ensures you get the latest software versions.

---

### Part 2: Installing and Running "sl"

4. Install the `sl` package:

   ```bash
   sudo apt install sl
   ```
5. After installation, run the program by typing:

   ```bash
   sl
   ```
6. Watch as a **train steams across your screen**. This demonstrates that the program is successfully installed and running.

---

### Part 3: Installing and Running "ninvaders"

7. Install the `ninvaders` package:

   ```bash
   sudo apt install ninvaders
   ```
8. Run the game:

   ```bash
   ninvaders
   ```
9. Use the arrow keys to move and the **spacebar** to shoot.

   * Press **Q** to quit the game.

---

### Part 4: Installing and Running "cmatrix"

10. Install the `cmatrix` package:

    ```bash
    sudo apt install cmatrix
    ```
11. Start the program by typing:

    ```bash
    cmatrix
    ```
12. Watch the green "digital rain" effect on your terminal.

    * To exit, press **Ctrl + C**.

---

### Part 5: Removing Packages (Cleanup)

13. To remove `sl`, type:

    ```bash
    sudo apt remove sl
    ```
14. To remove `ninvaders`:

    ```bash
    sudo apt remove ninvaders
    ```
15. To remove `cmatrix`:

    ```bash
    sudo apt remove cmatrix
    ```
16. If you want to remove leftover configuration files as well, use:

    ```bash
    sudo apt purge packagename
    ```

    (Replace `packagename` with the name of the program, e.g., `sl`).

---

## Summary

You have successfully learned how to:

* **Update your package list** (`sudo apt update`)
* **Install fun Linux packages** (`sudo apt install …`)
* **Run and enjoy programs** directly from the terminal
* **Remove software** when you no longer need it

This hands-on experience gave you the foundation for managing software on Ubuntu using the package management system.

---

## Follow-Up Activities

Here are some ideas to expand your learning:

1. **Explore More Fun Packages**: Try installing `fortune`, `cowsay`, or `figlet`.
2. **Research Package Info**: Use `apt show packagename` to learn more about any package.
3. **Practice System Maintenance**: Learn about `sudo apt upgrade` to keep all your installed software up to date.
4. **Challenge Yourself**: Create a short presentation or demo showing your favorite package to classmates.
