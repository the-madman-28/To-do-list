# Todo List App

This is a simple React-based Todo List application with the ability to add, toggle, and delete tasks. The application uses local storage to persist the todo items even after a page refresh.

## Table of Contents

- [Project Structure](#project-structure)
- [Components](#components)
  - [App](#app)
  - [NewTodoForm](#newtodoform)
  - [TodoItem](#todoitem)
  - [TodoList](#todolist)
- [Usage](#usage)
- [Local Storage](#local-storage)
- [Running the App](#running-the-app)

## Project Structure

- **App.jsx:** The main component that orchestrates the entire Todo List application. It manages the state of todos, handles adding, toggling, and deleting todos.

- **NewTodoForm.jsx:** A form component for adding new todo items. It takes user input and triggers the `onSubmit` callback provided by the parent component (App).

- **TodoItem.jsx:** Represents an individual todo item. It includes a checkbox to toggle completion status and a delete button.

- **TodoList.jsx:** Renders a list of todo items. It maps through the array of todos passed to it and renders TodoItem components.

- **main.jsx:** The entry point of the application, rendering the App component into the root element.

## Components

### App

The `App` component is the main component that holds the state of the todo items. It includes functions to add, toggle, and delete todos. The state is persisted in local storage to maintain todos across page refreshes.

### NewTodoForm

The `NewTodoForm` component is a simple form for adding new todo items. It takes user input and triggers the `onSubmit` callback provided by the parent component (App).

### TodoItem

The `TodoItem` component represents an individual todo item. It includes a checkbox for toggling completion status and a delete button.

### TodoList

The `TodoList` component renders a list of todo items. It maps through the array of todos passed to it and renders TodoItem components.

## Usage

To use the Todo List application, simply enter a new task in the input field of the `NewTodoForm` and click "Add." The tasks will be displayed in the `TodoList`, and you can toggle their completion status or delete them.

## Local Storage

The application uses local storage to persist the todo items. The todos are stored in local storage under the key "ITEMS," and they are retrieved during the initialization of the `App` component.

## Running the App

1. Clone this repository.

```bash
git clone https://github.com/your-username/todo-list-app.git
cd todo-list-app

```
2. Install dependencies.
```bash
npm install
```

3. Run the application.
```bash
npm start
```

Visit 'http://localhost:3000' in your web browser to see the Todo List app in action.
