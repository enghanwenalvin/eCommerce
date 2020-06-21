############################################ INITIAL SET UP ################################################################

1. In Hyper Terminal, cd into the desired folder (e.g. ..\Projects) and type: npx create-react-app eCommerce   
Note: eCommerce is the name of the new project
This will create a new React app and install the necessary starter packages

2. cd into the new project folder to see the contents. There are items that won't be required so let's clean them up
- In src/index.js, remove the lines of code related to serviceWorker   
- In src/App.js, remove contents inside of <div>. Also remove the className. Remove the import logo as well
- In src/App.css, remove all contents in the css file


############################################ HOME PAGE SET UP ################################################################

3. Create a new component homepage.component.jsx in the src folder (note: if syntax highlighting is not shown, install the language-babel package).
import React from 'react' then
create a function to render the structure of the homepage with a <div> container for the homepage, a <div> container for the directory-menu, a <div> container for the menu-item, and a <div> container for the content. Include a <h1> title and <span> subtitle. It should look something as follows:

const HomePage = () => (
  <div className='homepage'>
    <div className='directory-menu'>
      <div className='menu-item'>
        <div className='content'>
          <h1 className='title'>HATS</h1>
          <span className='subtitle'>SHOP NOW</span>
        </div>
      </div>
    </div>
  </div>
  );

Repeat for menu-items for SNEAKERS, JACKETS, WOMENS, MENS.
export default HomePage

4. In App.js import HomePage from './homepage.component'
Inside the <div>, render <HomePage />

5. In Hyper terminal, type: npm start
This runs the app in development mode. Check to ensure that the HomePage component is rendered properly

6. In Hyper terminal, type: npm install -g sass
This installs the sass package, which is a professional grade css extension language
npm install node-sass

7. Create a new sass file homepage.styles.scss to start styling the homepage.
Add import './homepage.styles.scss' in the homepage.component.jsx file
Run npm start to make sure the styles are rendered properly


#######################################################################################################################

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: https://facebook.github.io/create-react-app/docs/code-splitting

### Analyzing the Bundle Size

This section has moved here: https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size

### Making a Progressive Web App

This section has moved here: https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app

### Advanced Configuration

This section has moved here: https://facebook.github.io/create-react-app/docs/advanced-configuration

### Deployment

This section has moved here: https://facebook.github.io/create-react-app/docs/deployment

### `npm run build` fails to minify

This section has moved here: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify
