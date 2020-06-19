# Code organization with MVC: Model-View-Controller
The big idea behind MVC is that each section of your code has a different purpose. Some of your code holds the data of your app (MODEL), some of your code makes your app look nice (VIEW), and some of your code controls how your app functions (CONTROL).

This makes thinking about your app, revisiting your app, and sharing your app with others much easier and cleaner.

## Example:
The MODEL in a todo app might define what what a task is and that a list is a collection of tasks. This is where the database schema comes into play.

The VIEW code will define what the todos and lists looks like, visually. This will be mainly HTML code that links up with STATIC files such as CSS and images.

CONTROLLER code acts as a liaison between the Model and the View, receiving user input and deciding what to do with it. It's the brains of the application. The EXPRESS server code, as a good example.

Thus when a user clicks 'add task', the CONTROLLER makes sure that the Model adds a new task in the database, and redirects the user to the updated list on a page.

The entry point for the CONTROLLER CODE is the app.js in the root app folder. This main app.js file may require various other dependency files that store parts of the applications logic.