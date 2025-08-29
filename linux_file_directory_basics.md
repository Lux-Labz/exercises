<!--  
{
  "ID": "f3b1c9d2-7e4a-4a2d-9b6e-3a8e7f5c2d1b",
  "Title": "Linux File and Directory Management Basics",
  "Tags": ["Linux", "Ubuntu", "File Management", "Directories", "CLI", "Beginner"],
  "Description": "A beginner-friendly exercise to practice managing files and directories in Ubuntu Linux using the command line.",
  "Query": "You are a STEM instructor and training exercise curriculum creator for students aged 12-18. Geneate a training exercise with the following content: Manage files and directories. The focus area of this exercise is: Linux. The difficulty level of the exercise is: Beginner. The target operating system is: Ubuntu. Make the exercise clear, positive, detailed, and comprehensive. Each step of the excercise must be chronologically numbered. Include a hidden section, an overview section, and a prerequisite section befrore the exercise section. Include a summary section and a follow-up section after the exercise section. The hidden section is wrapped in an HTML style comment tag and includes the following parameters in json format: ID, Title, Tags, Description, Query, Model, Focus, Level, Date, Links, Filename. Where ID is a randomly generated 32 bit unique ID; Where title is a short title of the exercise; Where Tags is a list of tags associated with the exercise; Where Description is a short overview description of the exercise; Where Query is this query string; Where model is the model and version of this LLM; Where focus is the focus area of this exercise; Where level is the skill level of this exercise; Where date is the current date in the format yyyymmdd; Where Links is a list of helpful web links and resources related to this exercise; Where Filename is a short unique descriptive name for this markdown file. Do not place the hidden section in a code block.",
  "Model": "GPT-5-mini",
  "Focus": "Linux",
  "Level": "Beginner",
  "Date": "20250828",
  "Links": ["https://ubuntu.com/tutorials/command-line-for-beginners", "https://linuxcommand.org/"],
  "Filename": "linux_file_directory_basics"
}  
-->

# Overview

In this exercise, you will learn how to manage files and directories in Ubuntu Linux using basic command-line tools. By the end of this session, you will be able to navigate the file system, create and delete files and directories, and understand basic Linux file operations. This exercise is beginner-friendly and suitable for students aged 12–18.

# Prerequisites

Before starting this exercise, make sure you have:

1. Access to an Ubuntu system (physical or virtual).
2. A terminal application installed and ready to use.
3. Basic familiarity with typing commands in a terminal.
4. A positive attitude and curiosity to experiment safely in the command line.

# Exercise: Managing Files and Directories in Linux

1. **Open the Terminal**

   * Press `Ctrl + Alt + T` to open the terminal in Ubuntu.

2. **Check your current directory**

   * Type `pwd` and press `Enter`.
   * Observe the output. This is your current working directory.

3. **List files and directories**

   * Type `ls` to see all files in your current directory.
   * Type `ls -l` for a detailed view, including permissions and file sizes.

4. **Create a new directory**

   * Use the command `mkdir MyFirstDirectory` to create a folder called `MyFirstDirectory`.

5. **Navigate into the new directory**

   * Type `cd MyFirstDirectory` to enter your new folder.
   * Verify with `pwd` to ensure you are inside it.

6. **Create a new file**

   * Type `touch example.txt` to create an empty text file named `example.txt`.
   * Use `ls` to verify the file exists.

7. **Write some content into the file**

   * Type `echo "Hello, Linux!" > example.txt` to add text to the file.
   * Check the content with `cat example.txt`.

8. **Copy a file**

   * Type `cp example.txt copy_example.txt` to make a duplicate.
   * Use `ls` to see both files.

9. **Rename a file**

   * Type `mv copy_example.txt renamed_example.txt` to rename the copy.
   * Verify with `ls`.

10. **Move a file to a different directory**

    * Create another folder: `mkdir AnotherDirectory`.
    * Move the file using `mv renamed_example.txt ../AnotherDirectory/`.

11. **Delete a file**

    * Navigate into `AnotherDirectory`: `cd ../AnotherDirectory`
    * Remove the file: `rm renamed_example.txt`
    * Use `ls` to confirm deletion.

12. **Delete a directory**

    * Navigate back: `cd ..`
    * Remove the directory you created: `rmdir AnotherDirectory`
    * Note: `rmdir` works only for empty directories.

13. **Experiment with hidden files**

    * Create a hidden file: `touch .hiddenfile`
    * Use `ls -a` to see hidden files in the directory.

14. **Exit the terminal**

    * Type `exit` or simply close the terminal window.

# Summary

You have successfully learned how to:

* Navigate directories using `cd` and `pwd`.
* List files with `ls`.
* Create, rename, copy, and delete files and directories.
* Handle hidden files in Linux.

# Follow-up

To reinforce your skills:

1. Try creating a project folder with multiple subdirectories and files.
2. Experiment with different file permissions using `chmod`.
3. Learn about `man` pages (`man ls`, `man mkdir`) to explore more command options.
4. Practice combining commands to streamline file management tasks.

---

If you want, I can also create a **visual cheat sheet** of the commands used in this exercise, which makes it much easier for students aged 12–18 to memorize and practice. Do you want me to create that?
