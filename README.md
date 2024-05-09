# React Redux Counter

Build a React Application with help of Redux which renders a counter that displays a counter value and can be toggled

# Steps

## 0. Preparing a New Project

1. create a `README.md` file
2. create a `.gitignore` file to ignore `node_modules`
3. run `npm install`
4. run `npm install redux react-redux`
5. run `npm start`

## 1. Creating a Redux Store for React

1. as the common convention recommends, create a `store` folder to store the Redux related files
2. inside of it, create a `index.js` file in which you will create a store & a reducer
3. connect your React app to this Redux store so that the components of this app can dispatch and listen
   1. export the store as a default
   2. provide this store to the React app
