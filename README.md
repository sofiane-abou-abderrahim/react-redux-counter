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

## 2. Providing the Store

1. go to the `src/index.js`
2. import the `Provider` component from `react-redux`
3. wrap the root component with `<Provider>`
4. import `store` from `store/index`
5. set the `store` prop on the `<Provider>` component to `store`

## 3. Using Redux Data in React Components

1. utilize this Provider store in the `Counter.js` component
2. get access to the Redux store into the data to output the current counter value
   1. import the React Redux's `useSelector` custom hook
   2. use `useSelector()` inside of the `Counter` function
3. output the `counter` value

## 4. Dispatching Actions From Inside Components

1. in `Counter.js`, add 2 buttons to increment & decrement the counter
2. use `useDispatch()` to dispatch actions & wire up these buttons with help of 2 functions

## 5. Redux with Class-based Components

1. add a new `Counter` class in `Counter.js` & extend it to `Component`
2. render the JSX code inside of it
3. add all the relevant methods
4. add the `this` keyword to refer to these methods
5. get access to Redux with help of the `connect` feature

## 6. Attaching Payloads to Actions

1. add a new `button` to increase the counter by 5 (or any other number) in `Counter.js`
2. add a new `action.type === increase` in `store/index.js` & set an `action.amount`
3. add a new `increaseHandler` function in `Counter.js`

## 7. Working with Multiple State Properties

1. add a new state to the Redux store to show/display the counter
2. dispatch the `toggle` action inside of the `toggleCounterHandler` in `Counter.js`
3. get access to this `toggle` state with help of `useSelector()` inside of the `Counter` component & store it in a `show` constant
4. render the counter conditionally by using this `show` constant
