# 0x15. API

## Background Context
Old-school system administrators often rely solely on Bash scripting, but modern SREs (Site Reliability Engineers) typically have a broader skill set, including Python. APIs are a popular method to expose applications and datasets, allowing for interaction and data manipulation.

In this project, you will use Python to access employee data via an API, organizing and exporting it into different data structures.

## Requirements
### General
- Allowed editors: `vi`, `vim`, `emacs`.
- All your files will be interpreted/compiled on Ubuntu 20.04 LTS using `python3` (version 3.8.5).
- All your files should end with a new line.
- The first line of all your files should be exactly `#!/usr/bin/python3`.
- Libraries imported in your Python files must be organized in alphabetical order.
- A `README.md` file, at the root of the folder of the project, is mandatory.
- Your code should use the `pycodestyle` (version 2.8.*).
- All your files must be executable.
- The length of your files will be tested using `wc`.
- All your modules should have a documentation (`python3 -c 'print(__import__("my_module").__doc__)'`).
- You must use `get` to access dictionary values by key (it won’t throw an exception if the key doesn’t exist in the dictionary).
- Your code should not be executed when imported (by using `if __name__ == "__main__":`).

## Tasks
### 0. Gather data from an API
**Mandatory**

Write a Python script that, using this REST API, for a given employee ID, returns information about his/her TODO list progress.

#### Requirements
- You must use `urllib` or `requests` module.
- The script must accept an integer as a parameter, which is the employee ID.
- The script must display on the standard output the employee TODO list progress in this exact format:
  - First line: `Employee EMPLOYEE_NAME is done with tasks(NUMBER_OF_DONE_TASKS/TOTAL_NUMBER_OF_TASKS):`
    - `EMPLOYEE_NAME`: name of the employee.
    - `NUMBER_OF_DONE_TASKS`: number of completed tasks.
    - `TOTAL_NUMBER_OF_TASKS`: total number of tasks, which is the sum of completed and non-completed tasks.
  - Second and N next lines display the title of completed tasks: `TASK_TITLE` (with 1 tabulation and 1 space before the `TASK_TITLE`).

### 1. Export to CSV
**Mandatory**

Using what you did in task #0, extend your Python script to export data in the CSV format.

#### Requirements
- Records all tasks that are owned by this employee.
- Format must be: "USER_ID","USERNAME","TASK_COMPLETED_STATUS","TASK_TITLE".
- File name must be: USER_ID.csv.

### 2. Export to JSON
**Mandatory**

Using what you did in task #0, extend your Python script to export data in the JSON format.

#### Requirements
- Records all tasks that are owned by this employee.
- Format must be: { "USER_ID": [{"task": "TASK_TITLE", "completed": TASK_COMPLETED_STATUS, "username": "USERNAME"}, {"task": "TASK_TITLE", "completed": TASK_COMPLETED_STATUS, "username": "USERNAME"}, ... ]}.
- File name must be: USER_ID.json.

### 3. Dictionary of list of dictionaries
**Mandatory**

Using what you did in task #0, extend your Python script to export data in the JSON format.

#### Requirements
- Records all tasks from all employees.
- Format must be: { "USER_ID": [ {"username": "USERNAME", "task": "TASK_TITLE", "completed": TASK_COMPLETED_STATUS}, {"username": "USERNAME", "task": "TASK_TITLE", "completed": TASK_COMPLETED_STATUS}, ... ], "USER_ID": [ {"username": "USERNAME", "task": "TASK_TITLE", "completed": TASK_COMPLETED_STATUS}, {"username": "USERNAME", "task": "TASK_TITLE", "completed": TASK_COMPLETED_STATUS}, ... ]}.
- File name must be: todo_all_employees.json.
