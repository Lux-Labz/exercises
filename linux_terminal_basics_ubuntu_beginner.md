<!-- 
{
  "ID": "2837461920",
  "Title": "Getting Started with the Linux Terminal",
  "Tags": ["Linux", "Ubuntu", "Beginner", "Terminal Basics", "STEM"],
  "Description": "A beginner-friendly training exercise to introduce students to basic Linux terminal commands on Ubuntu.",
  "Query": "You are a STEM instructor and training exercise curriculum creator for students aged 12-18. Geneate a training exercise with the following content: Use the linux terminal. The focus area of this exercise is: Linux. The difficulty level of the exercise is: Beginner. The target operating system is:  Ubuntu. Make the exercise clear, positive, detailed, and comprehensive.  Each step of the excercise must be chronologically numbered.  Include a hidden section, an overview section, and a prerequisite section befrore the exercise section.  Include a summary section and a follow-up section after the exercise section. The hidden section is wrapped in an HTML style comment tag and includes the following parameters in json format: ID, Title, Tags, Description, Query, Model, Focus, Level, Date, Links, Filename. Where ID is a randomly generated 32 bit unique ID; Where title is a short title of the exercise; Where Tags is a list of tags associated with the exercise; Where Description is a short overview description of the exercise; Where Query is this query string; Where model is the model and version of this LLM; Where focus is the focus area of this exercise; Where level is the skill level of this exercise; Where date is the current date in the format yyyymmdd; Where Links is a list of helpful web links and resources related to this exercise; Where Filename is a short unique descriptive name for this markdown file.  Do not place the hidden section in a code block.",
  "Model": "GPT-5",
  "Focus": "Linux",
  "Level": "Beginner",
  "Date": "20250910",
  "Links": [
    "https://ubuntu.com/tutorials/command-line-for-beginners",
    "https://linuxjourney.com/",
    "https://man7.org/linux/man-pages/"
  ],
  "Filename": "linux_terminal_basics_ubuntu_beginner.md"
}
-->

# Training Exercise: Getting Started with the Linux Terminal on Ubuntu

---

## Overview

This training exercise will introduce students (ages 12–18) to the **Linux terminal** in Ubuntu. By the end of this activity, students will understand how to open the terminal, navigate the file system, create and manage files and directories, and use a few essential commands. The exercise encourages exploration, builds confidence, and lays a foundation for future Linux learning.

---

## Prerequisites

Before starting this exercise, students should:

* Have access to an Ubuntu system (desktop or virtual machine).
* Be able to log in and open applications.
* Be familiar with basic computer navigation (folders, files, and clicking icons).
* No prior terminal experience is required!

---

## Exercise: Step-by-Step

### Part 1: Opening the Terminal

1. **Locate the Terminal application**

   * Click the **“Show Applications”** button (grid of dots) in the bottom-left corner of your Ubuntu desktop.
   * Type **“Terminal”** in the search box.
   * Click on the **Terminal** icon to open it.

2. **Confirm you are in the Terminal**

   * You should see a prompt that looks something like:

     ```
     username@computer:~$
     ```

---

### Part 2: Exploring the File System

3. **Check your current directory**

   * Type:

     ```
     pwd
     ```
   * This shows the **present working directory** (usually `/home/username`).

4. **List the files and folders**

   * Type:

     ```
     ls
     ```
   * This displays the files and directories in your current location.

5. **Show detailed information**

   * Type:

     ```
     ls -l
     ```
   * Notice the file permissions, owner, size, and date information.

---

### Part 3: Creating and Navigating Directories

6. **Create a new folder**

   * Type:

     ```
     mkdir practice_folder
     ```

7. **Move into your new folder**

   * Type:

     ```
     cd practice_folder
     ```

8. **Confirm you moved successfully**

   * Type:

     ```
     pwd
     ```
   * The output should end with `/practice_folder`.

---

### Part 4: Working with Files

9. **Create a text file**

   * Type:

     ```
     touch hello.txt
     ```

10. **List the files**

    * Type:

      ```
      ls
      ```
    * You should see `hello.txt`.

11. **Write text into the file**

    * Type:

      ```
      echo "Hello, Linux world!" > hello.txt
      ```

12. **View the contents of the file**

    * Type:

      ```
      cat hello.txt
      ```
    * The message should appear on the screen.

---

### Part 5: Clean Up

13. **Go back to your home directory**

    * Type:

      ```
      cd ~
      ```

14. **Remove the practice folder and its contents**

    * Type:

      ```
      rm -r practice_folder
      ```

15. **Check that it’s gone**

    * Type:

      ```
      ls
      ```
    * The folder should no longer be listed.

---

## Summary

In this exercise, you learned how to:

* Open the Ubuntu terminal.
* Navigate the file system with `pwd`, `ls`, and `cd`.
* Create and manage directories using `mkdir` and `rm`.
* Create and edit files using `touch`, `echo`, and `cat`.

You’ve just taken your **first steps in Linux command-line navigation**!

---

## Follow-Up

To continue building your Linux skills, try:

* Using `ls -a` to show hidden files.
* Exploring the manual pages with `man ls`.
* Creating multiple files and practicing `mv` (move) and `cp` (copy).
* Reading more tutorials: [Ubuntu Command Line for Beginners](https://ubuntu.com/tutorials/command-line-for-beginners).

