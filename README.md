Creating the TaskList Component:

In this step, we will build the TaskList component, which will be responsible for displaying the list of tasks.
The TaskList component will receive the tasks as a prop and render them dynamically, showing each task's
name, priority, category, and completion status. It will also allow users to mark tasks as complete or delete
them.

Creating the TaskList Component:
In the TaskList.jsx file, we will create a component that displays each task along with options to mark it as
complete or delete it.

Explanation of TaskList:
1. Props:
• tasks : An array of tasks passed from the App.js component.
• toggleComplete : A function to marka task as complete or undo it
• delete Task : A function to delete a task from the list.

2. Rendering Tasks:
• The TaskList component maps over the tasks array and renders each task's name, priority, and
ca tegory.
• If the task is marked as complete, it will be displayed with a completed class (which can be styled to
show a strikethrough or change color).

3. Actions:
• Complete/Undo Button: This button toggles the task's completion status. If the task is completed, it
shows "Undo"; otherwise, it shows "Complete".
• Delete Button: This button deletes the task from the list.

4. Conditional Rendering:
• If there are no tasks, it shows a message: "No tasks available. Add some tasks!"
• If tasks exist, it maps over the tasks array and renders each task with the provided details.