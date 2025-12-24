src/
│
├── components/
│   ├── Header.jsx
│   ├── TaskInput.jsx
│   ├── TaskItem.jsx
│   ├── TaskList.jsx
│
├── pages/
│   ├── Home.jsx
│   ├── Stats.jsx
│
├── store/
│   ├── taskContext.jsx
│
├── styles/
│   ├── global.css
│
├── App.jsx
├── main.jsx


 **What Each File Does**
 **store/taskContext.jsx (Global State)**
This is the global state manager of the app.
It uses React Context API to store:
All tasks
Dark mode state
It also:
Handles adding, deleting, and updating tasks
Saves tasks and dark mode preference to localStorage
Makes task data accessible across all pages (Home & Stats)

 **components**/
Header.jsx
Displays the app title, navigation links, and the dark mode toggle button.
TaskInput.jsx
Contains the input field and button used to add new tasks.
TaskItem.jsx
Represents a single task.
Includes:
Checkbox to mark complete
Task text
Delete button
TaskList.jsx
Displays all tasks by looping through them and rendering TaskItem.

 **pages**/
Home.jsx
The main page where users add tasks and see the task list.
Stats.jsx
Shows task statistics:
Total tasks
Completed tasks
Remaining tasks

 **styles/global.css**
Contains all styling for the app, including:
Light and dark mode styles
Layout styling
Responsive design for small screens

**App.jsx**
Handles page routing using React Router and applies light/dark mode styles.

**main.jsx**
The entry point of the app.
Wraps the entire application with the TaskProvider so global state is available everywhere.

**Features Summary**
Add, complete, and delete tasks
Global state using Context API
Dark mode with persistence
Task data saved in localStorage
Statistics page using React Router
Responsive design

