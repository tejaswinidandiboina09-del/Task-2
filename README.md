# To-Do List Manager

A simple command-line to-do list manager written in Python.

## Objective
Implement a simple to-do list manager.

## Tools
- Python 3
- VS Code / terminal

## Deliverable
- `todo.py`

## Features
- Add a new task
- View all tasks (completed tasks are marked with ✔)
- Mark a task as done
- Delete a task
- Input validation for empty tasks, invalid menu choices and invalid task numbers

## How to Run
1. Make sure Python 3 is installed:
   ```
   python --version
   ```
2. Open the folder containing `todo.py` in VS Code (or a terminal).
3. Run the program:
   ```
   python todo.py
   ```
4. Enter a number (1-5) to choose an option from the menu.

## Menu Options
| Option | Action |
|--------|--------|
| 1 | Add task |
| 2 | View tasks |
| 3 | Mark task as done |
| 4 | Delete task |
| 5 | Exit |

## How It Works
- Tasks are stored in a Python list called `tasks`.
- Each task is a dictionary: `{"title": "Study Python", "done": False}`.
- Functions: `add_task()`, `show_tasks()`, `complete_task()`, `delete_task()` and `main()` (the menu loop).
- Tasks are kept in memory only, so they are cleared when the program exits.

## Sample Output
```
=== To-Do List Manager ===
1. Add task
2. View tasks
3. Mark task as done
4. Delete task
5. Exit
Choose an option (1-5): 1
Enter task: Study Python
Added: Study Python

Choose an option (1-5): 1
Enter task: Watch K-drama
Added: Watch K-drama

Choose an option (1-5): 2

Your Tasks:
1. [ ] Study Python
2. [ ] Watch K-drama

Choose an option (1-5): 3
Task number to mark done: 1
Completed: Study Python

Choose an option (1-5): 4
Task number to delete: 2
Deleted: Watch K-drama

Choose an option (1-5): 2

Your Tasks:
1. [✔] Study Python

Choose an option (1-5): 5
Goodbye!
```

## Possible Improvements
- Save tasks to a file (JSON/text) so they persist
- Add due dates and priorities
- Edit an existing task
-
