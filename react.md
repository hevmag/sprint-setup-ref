# Getting Started with Create React App

To first initialise your React app run the command:

```
npx create-react-app my-app
```

What does this mean?

-   npx executes the package
-   create-react-app "bootstraps" a React project for you
-   you can replace my-app with whatever you would like your app folder to be called!

It might take a little while to install all of the dependencies, but once it's done you will have all of the setup files you need to start building your React app.

*Note:* If you want to initialise a React app in your current working directory, you can run:
```
npx create-react-app .
```
where the dot represents your current location in the terminal.

## 🔥 HOT TIP 🔥

We can use the flag _--template min_ to give us a blank React app template with only the essential src files we need to start coding. This let's us skip a lot of the necessary "cleaning up" mentioned later on in this setup guide. Give it a go!

```
npx create-react-app my-app --template min
```

## Viewing your React app in browser

Once we have our files setup, cd into your project folder i.e.

```
cd my-app
```

then, in your terminal, run

```
npm start
```

This start script will load up your React app and display it in your browser.

## Cleaning up your React App

The base React template has a lot of stuff going on that we don't necessarily always want in our app.

Start by deleting the contents of the public folder excluding the index.html file.

We can delete the files in src folder apart from the App.js and index.js too, as we won't be using them for our React sprints at NC.

Make sure to delete any imports from the files that no longer exist to get rid of any consequential undefined errors. You can also delete the html code in the App.js, and replace it with something simple of your own, just to get something to render on the page and make sure everything is working OK.

E.g.

```
function App() {
  return (
    <div>
      <h1>My React App</h1>
    </div>
  );
}

export default App;
```

Your index.js should look something like this:

```
import React from 'react';
import ReactDOM from 'react-dom/client';
import App from './App';

const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(
  <React.StrictMode>
    <App />
  </React.StrictMode>
);

reportWebVitals();
```

At this point, you should have a bit of a tidier folder set up and be ready to start coding!
