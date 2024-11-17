<!--
ID: PYTHON_INTERMEDIATE_001
Tags: [python, intermediate, data_processing, file_handling]
Description: This exercise focuses on intermediate-level Python skills, including file handling and data processing.
Query: Generate an intermediate-level getting started training exercise for python. Make the exercise very positive and detailed. Include all prerequisites and steps. Add a hidden field to the top of the exercise with the following parameters: ID, Tags, Description, Query, Model, Level. Where ID is a unique ID. Where Tags is a list of tags associated with the exercise. Where Description is a short overview of the exercise. Where Query is this query string. Where model is the model and version of the LLM that I'm submitting the query to. Where level is the skill level of this exercise rated as beginner, intermediate, or advanced. The entire training exercise should be displayed as a wiki file in a markdown-formatted string that I can copy or download.
Model: ChatGPT v4.0
Level: Intermediate
-->

# Intermediate Python Training Exercise: File Handling and Data Processing

## Overview
In this exercise, you will work on intermediate-level Python skills by handling file input/output and processing data. You will create a Python script that reads data from a CSV file, processes it, and writes the results to a new file. This exercise will help you practice working with file operations and basic data processing techniques.

## Prerequisites
- Basic understanding of Python syntax
- Familiarity with data types (lists, dictionaries)
- Basic knowledge of CSV files and how to handle them in Python

## Exercise Steps

### Step 1: Setup
1. **Create a CSV file** named `data.csv` with the following content:
    ```csv
    Name,Age,Occupation
    Alice,30,Engineer
    Bob,25,Data Scientist
    Charlie,35,Teacher
    ```
2. **Create a new Python script** file named `process_data.py` in the same directory as `data.csv`.

### Step 2: Read the CSV File
1. **Import the necessary module** for handling CSV files:
    ```python
    import csv
    ```

2. **Open and read the CSV file**:
    ```python
    with open('data.csv', mode='r') as file:
        reader = csv.DictReader(file)
        data = list(reader)
    ```

3. **Print the data** to verify it has been read correctly:
    ```python
    print(data)
    ```

### Step 3: Process the Data
1. **Create a new list** to store processed data:
    ```python
    processed_data = []
    ```

2. **Process each row** to add a new field `Senior` that is `True` if `Age` is greater than or equal to 30, otherwise `False`:
    ```python
    for row in data:
        row['Senior'] = int(row['Age']) >= 30
        processed_data.append(row)
    ```

### Step 4: Write Data to a New CSV File
1. **Specify the fieldnames** including the new `Senior` field:
    ```python
    fieldnames = ['Name', 'Age', 'Occupation', 'Senior']
    ```

2. **Write the processed data** to a new CSV file named `processed_data.csv`:
    ```python
    with open('processed_data.csv', mode='w', newline='') as file:
        writer = csv.DictWriter(file, fieldnames=fieldnames)
        writer.writeheader()
        writer.writerows(processed_data)
    ```

3. **Verify the new CSV file** has been created and contains the correct data by opening `processed_data.csv`.

### Step 5: Testing and Verification
1. **Run your Python script** to ensure it completes without errors and creates the `processed_data.csv` file.
2. **Check the contents of `processed_data.csv`** to verify that each person’s `Senior` status has been correctly calculated and recorded.

## Conclusion
Congratulations on completing this intermediate-level exercise! You have successfully read, processed, and written data using Python's CSV handling capabilities. This exercise will help you better understand file operations and data processing in Python.

Feel free to modify the CSV file and script to practice with different datasets and processing tasks!

## Additional Resources
- [Python CSV Module Documentation](https://docs.python.org/3/library/csv.html)
- [Intermediate Python Programming](https://realpython.com/tutorials/intermediate/)

