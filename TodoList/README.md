### Todo List Application 

#### Overview

This Todo List application is a simple, client-side React application designed as a warm-up project for getting back into coding. It allows users to add, edit, and delete todos. The state of the todos is persisted in the browser's `localStorage`, ensuring the list is retained even after refreshing the page. This application serves as a quick exercise to refresh coding skills and revisit fundamental concepts.

#### Application Structure

The application consists of the following components:

1. **App**: The main component that manages the state and renders `TodoInput` and `TodoList` components.
2. **TodoInput**: A component that provides an input field and a button to add new todos.
3. **TodoList**: A component that renders the list of todos using `TodoCard` components.
4. **TodoCard**: A component that renders individual todo items with edit and delete functionalities.

#### Components

##### 1. App Component

The `App` component is the main entry point of the application. It manages the state of the todos and handles the addition, deletion, and editing of todos. The state is persisted using `localStorage`.

- **State Management**: The component uses the `useState` hook to manage the list of todos and the current input value.
- **Persistence**: The `localStorage` is used to save and load the todos to ensure persistence across page reloads.
- **Handlers**: It provides functions to add, delete, and edit todos.

##### 2. TodoInput Component

The `TodoInput` component provides an input field and a button for adding new todos.

- **Props**: Receives the current input value, a function to set the input value, and a function to handle adding new todos.
- **Functionality**: Allows the user to enter a new todo and add it to the list.

##### 3. TodoList Component

The `TodoList` component renders a list of `TodoCard` components.

- **Props**: Receives the list of todos and functions to handle editing and deleting todos.
- **Functionality**: Maps through the list of todos and renders each one using the `TodoCard` component.

##### 4. TodoCard Component

The `TodoCard` component renders an individual todo item with edit and delete buttons.

- **Props**: Receives the todo item, index, and functions to handle editing and deleting the todo.
- **Functionality**: Displays the todo item and provides buttons to edit or delete the item.

#### Usage

1. **Adding a Todo**: Enter the todo text in the input field and click the "Add" button. The new todo will appear in the list.
2. **Editing a Todo**: Click the edit button next to a todo item. The todo text will appear in the input field for editing. After making changes, click the "Add" button to save the edited todo.
3. **Deleting a Todo**: Click the delete button next to a todo item to remove it from the list.

#### Local Storage

The application uses `localStorage` to persist the todos. This ensures that the todos are saved even if the page is refreshed or the browser is closed and reopened.

#### Key Features

- **Responsive Design**: The application layout adjusts based on the screen size for an optimal user experience on different devices.
- **User-Friendly Interface**: Easy-to-use input field and buttons for managing todos.
- **State Persistence**: Uses `localStorage` to save and load todos, providing a seamless user experience.
