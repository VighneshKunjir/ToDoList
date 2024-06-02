# ToDoList Web Application
The ToDoList web application is a simple yet effective tool for organizing your tasks. With ToDoList, you can easily add new tasks to your list and remove them as they are completed.

## Features
- Add Tasks: Quickly add new tasks to your list to keep track of your to-dos.
- Remove Tasks: Remove tasks from your list as you complete them, keeping your list organized and up-to-date.
- User-Friendly Interface: Enjoy a clean and intuitive user interface designed for easy task management.
- Dynamic Functionality: Built with JavaScript, ToDoList offers interactive features that make adding and removing tasks a breeze.
- Responsive Design: Access your to-do list on any device, whether it's your desktop, tablet, or smartphone.


## Usage
- Add Tasks: Simply type your task into the input field and press enter to add it to your list.
- Remove Tasks: Click on the task you want to remove to delete it from your list.

## Node scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you coudn't customize it when you are ready for it.

## Error

While running  `npm start`. if your are facing [ 'error:03000086:digital envelope routines::initialization error' ].
The error comes from your dependency relying on an obsolete version of SSL
## Fix

Edit the package.json file with below changes:

"scripts": {
    "start": "react-scripts --openssl-legacy-provider start",
    "build": "react-scripts --openssl-legacy-provider build"
  }

## More 
for more info read - https://stackoverflow.com/questions/74726224/opensslerrorstack-error03000086digital-envelope-routinesinitialization-e
                   - https://stackoverflow.com/questions/69692842/error-message-error0308010cdigital-envelope-routinesunsupported
