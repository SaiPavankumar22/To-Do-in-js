# To-Do Manager Application

A simple command-line-based **To-Do Manager** that helps users organize and manage tasks effectively. This program allows you to add tasks, mark tasks as completed, and view tasks categorized as **Overdue**, **Due Today**, and **Due Later**.

## Features

- **Add new tasks** with a title, due date, and default completion status (`incomplete`).
- **Mark tasks as complete** by selecting their index.
- **Categorize tasks**:
  - **Overdue**: Tasks with a due date before today.
  - **Due Today**: Tasks with today's date.
  - **Due Later**: Tasks with a due date after today.
- **Display tasks** in a user-friendly format:
  - Completed tasks are marked with `[x]`.
  - Incomplete tasks are marked with `[ ]`.
  - Dates are displayed for overdue and due-later tasks, but not for tasks due today.

## Prerequisites

- **Node.js**: To run this application, ensure Node.js is installed on your system.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/SaiPavankumar22/todo-manager.git
   ```
2. Navigate to the project directory:
   ```bash
   cd todo-manager
   ```
3. Open the `index.js` file in your favorite editor.

## Usage

### Running the Application

Run the program using Node.js:
```bash
node index.js
```

### Interactive Menu Options

1. **Add a Task**: Enter the task title and due date when prompted.
2. **Mark a Task as Complete**: Provide the task index to mark it as completed.
3. **View Tasks**: Displays all tasks grouped into **Overdue**, **Due Today**, and **Due Later** categories.
4. **Exit**: Quit the application.

### Sample Output
```plaintext
Options:
1. Add a new task
2. Mark a task as complete
3. View all tasks
4. Exit

Choose an option: 3

My Todo-list

Overdue
[ ] Submit assignment 2024-12-14

Due Today
[x] Pay rent
[ ] Service Vehicle

Due Later
[ ] File taxes 2024-12-16
[ ] Pay electric bill 2024-12-16
```

## Code Structure

- **`todoList` Closure**: Encapsulates all task management functions:
  - `add`: Adds a new task.
  - `markAsComplete`: Marks a task as completed.
  - `overdue`: Returns overdue tasks.
  - `dueToday`: Returns tasks due today.
  - `dueLater`: Returns tasks due later.
  - `toDisplayableList`: Formats tasks for display.
- **`interactWithTodoList` Function**: Handles the interactive command-line interface for user interaction.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request if you have suggestions for improvements.
