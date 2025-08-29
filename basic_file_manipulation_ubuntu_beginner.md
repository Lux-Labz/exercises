<!--
{
  "ID": "3487261590",
  "Title": "Basic File Manipulation in Ubuntu",
  "Tags": ["Ubuntu", "Linux", "file management", "computer basics", "beginner"],
  "Description": "A beginner-friendly exercise to practice basic file manipulation commands in Ubuntu.",
  "Query": "You are a STEM instructor and training exercise curriculum creator for students aged 12-18. Geneate a training exercise with the following content: Learn basic file manipulation in Ubuntu. The focus area of this exercise is: Computer Basics. The difficulty level of the exercise is: Beginner. Make the exercise clear, positive, detailed, and comprehensive.  Each step of the excercise must be chronologically numbered.  Include a hidden section, an overview section, and a prerequisite section befrore the exercise section.  Include a summary section and a follow-up section after the exercise section. The hidden section is wrapped in an HTML style comment tag and includes the following parameters in json format: ID, Title, Tags, Description, Query, Model, Focus, Level, Date, Links, Filename. Where ID is a randomly generated 32 bit unique ID; Where title is a short title of the exercise; Where Tags is a list of tags associated with the exercise; Where Description is a short overview description of the exercise; Where Query is this query string; Where model is the model and version of this LLM; Where focus is the focus area of this exercise; Where level is the skill level of this exercise; Where date is the current date in the format yyyymmdd; Where Links is a list of helpful web links and resources related to this exercise; Where Filename is a short unique descriptive name for this markdown file.",
  "Model": "GPT-5",
  "Focus": "Linux",
  "Level": "Beginner",
  "Date": "20250828",
  "Links": [
    "https://help.ubuntu.com/community/UsingTheTerminal",
    "https://ubuntu.com/tutorials/command-line-for-beginners",
    "https://linuxcommand.org/"
  ],
  "Filename": "basic_file_manipulation_ubuntu_beginner.md"
}
-->

### Overview

This exercise introduces students to basic file manipulation in Ubuntu using the terminal. Students will learn how to create, view, rename, move, and delete files and directories. By the end of this activity, students will feel confident navigating their system and managing files using fundamental Linux commands.

### Prerequisites

1. A computer with Ubuntu installed (either directly or through a virtual machine).
2. Access to the Ubuntu terminal.
3. Basic understanding of what a file and a folder (directory) are.
4. No prior experience with Linux commands is required.

### Exercise: Basic File Manipulation in Ubuntu

1. Open the Ubuntu terminal by pressing **Ctrl + Alt + T**.
2. Check your current location in the file system using:
   `pwd`
3. List all files and folders in your current location using:
   `ls`
4. Create a new directory called `practice` using:
   `mkdir practice`
5. Move into the `practice` directory using:
   `cd practice`
6. Create a new empty file called `notes.txt` using:
   `touch notes.txt`
7. Verify the file exists by listing files:
   `ls`
8. Add text to the file using a simple editor like nano:
   `nano notes.txt`

   * Type: *This is my first practice file.*
   * Save and exit (Ctrl+O, Enter, then Ctrl+X).
9. Display the contents of the file without editing using:
   `cat notes.txt`
10. Rename the file to `my_notes.txt` using:
    `mv notes.txt my_notes.txt`
11. Create another file called `extra.txt` using:
    `touch extra.txt`
12. Create a new subfolder called `backup` using:
    `mkdir backup`
13. Move the file `extra.txt` into the `backup` folder using:
    `mv extra.txt backup/`
14. Copy the file `my_notes.txt` into the `backup` folder using:
    `cp my_notes.txt backup/`
15. Navigate into the `backup` folder:
    `cd backup`
16. List files inside to confirm both are present:
    `ls`
17. Delete the file `extra.txt` using:
    `rm extra.txt`
18. Navigate back one level to the `practice` folder:
    `cd ..`
19. Remove the entire `backup` folder and its contents using:
    `rm -r backup` ⚠️
20. Confirm the folder is gone by listing files again:
    `ls`

### Summary

In this exercise, you practiced navigating directories, creating files and folders, editing files, moving and copying files, and deleting them. These are the foundation of managing data in Ubuntu through the terminal.

### Follow-up

1. Explore other commands such as `man` (to read manuals) and `ls -l` (for detailed listings).
2. Practice creating nested folders and organizing files into categories.
3. Learn how to use the `find` command to locate files in your system.
4. Research safe deletion methods such as using the `trash-cli` tool.

Recommendation: Reinforce learning by repeating the steps until they feel natural.
Next step: Try creating a personal project folder and organize different text files inside it.
