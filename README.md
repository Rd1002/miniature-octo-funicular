We are going to use create-react-app v0.1.0 which has the CSS Module configured already. Open your terminal and cd to the folder you want the project installed. Then run the below command:
npx create-react-app pagination  --use-npm
The above command will download the project into the folder calledpagination. You need to cd into the folder and run npm start. If everything goes well, you will have a page that looks like below:

HTML and CSS Styling
Open the project in your favorite code editor and locate the App.js file, We need to prepare our App.js to the look exactly like the way we want it by adding the HTML code and CSS style below:
Create a new file called App.module.css in the same directory where you have your App.js, then import it into your App.js using:
import styles from './App.module.css';
I want us to handle the display of the pagination number first, below is the style and HTML structure of what we are going to use.
Add the content below into your App.module.css.
Sorry for the plenty code written so far :), I want us to have a good looking table with pagination style in place before we move into the actual paging
According to the create-react-app docs, create-react-app should not be installed globally:

If you've previously installed create-react-app globally via npm install -g create-react-app, we recommend you uninstall the package using npm uninstall -g create-react-app or yarn global remove create-react-app to ensure that npx always uses the latest version.

This is even stated in the error message you recieved:

You are running create-react-app 4.0.0, which is behind the latest release (4.0.1). We no longer support global installation of Create React App.

(Emphasis mine)

You must uninstall create-react-app with npm uninstall -g create-react-app.

Then each time you want to create a new React app with create-react-app, use the command npx create-react-app my-app.

So to fix the error you're getting, uninstall create-react-app globally, update npm, clear the cache, and retry creating the app.

Run this in your terminal:

npm uninstall -g create-react-app
