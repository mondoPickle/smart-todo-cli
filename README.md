# smart-todo-cli

A secure, encrypted command-line to-do list manager with task priorities, due dates, and categories.

## Features

- Local encrypted storage of tasks (using Fernet symmetric encryption).
- Add, list, and mark tasks done via simple CLI commands.
- Task metadata: priority, due date, category.
- Keeps your task data private on your machine.
- No network communication or external dependencies.

## Usage

```bash
# Add a task
python smart_todo.py add --desc "Finish project" --priority high --due 2025-08-10 --category work

# List pending tasks
python smart_todo.py list

# List all tasks including done
python smart_todo.py list --all

# Mark a task done by ID
python smart_todo.py done --id 1
