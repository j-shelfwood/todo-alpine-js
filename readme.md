# Alpine.js To-Do List App

## Overview

This project showcases a simple to-do list application built with Alpine.js and styled with Tailwind CSS. The app provides a clean interface for users to input and track their tasks. It also persists task data in the local storage, so your tasks will be saved between page reloads.

## Features

- Task addition: Add tasks easily using the input field.
- Task completion: Toggle the completion state by clicking on the task.
- Data persistence: Tasks are stored in the browser's local storage.

## How It Works

### Initialization

The app uses Alpine.js for declarative data handling and UI manipulations. It initializes an Alpine component with `x-data`, which provides the following methods and properties:

- `init()`: Initialize tasks from local storage or an empty array if local storage is empty.
- `input`: Holds the value of the input field.
- `tasks`: An array to hold task objects. Each object contains a `name` and a `completed` field.
- `saveTask()`: Saves the new task.
- `persistTasks()`: Stores the current tasks array in local storage.
- `toggleCompletion(index)`: Toggles the completion status of a task at a given index.

### UI

Tailwind CSS is used for styling. We use a rounded white box (`rounded-lg`, `bg-white`, `shadow-lg`, `p-6`) to hold the input field and tasks list. Tasks are displayed as list items, and completed tasks get a line-through decoration.

## Installation

To get this app running on your local machine, you need to include the Alpine.js and Tailwind CSS libraries. In this example, they are included from CDNs.

```html
<script src="//unpkg.com/alpinejs" defer></script>
<script src="https://cdn.tailwindcss.com"></script>
```

## Usage

1. To add a task, type into the "Add your task:" input field and hit Enter.
2. Your tasks will appear in a list below the input field.
3. Click on a task to toggle its completion state.
4. All tasks and their states are saved in local storage. They will be available upon reloading the page.

## License

This project is open-source, feel free to use it, modify it or distribute it.

## Contributions

Contributions are always welcome! Please read the contribution guidelines first.

## Acknowledgements

- Alpine.js: For providing a lean and clean way to work with frontend logic.
- Tailwind CSS: For the utility-first CSS framework used for styling.

## Support

If you encounter any issues or have questions, feel free to open an issue or submit a pull request.
