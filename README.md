## Problem

- Create the following APP: [Products Routes WebApp](https://rct-101-e3.netlify.app/) using the Provided Boilerplate,

**_Note_**: Make sure you start `json-server` on `8080` port with provided `db.json` file, then only you will be able to see data on this website.

## Getting Started

1. Fork this repository [https://github.com/riteshf/rct-101-e3.git](https://github.com/riteshf/rct-101-e3)
2. Clone the Forked repository.
   - **_Note_**: This Clone repository should be on your github account.
3. navigate to the folder `cd rct-101-e3`
4. npm install
5. npm start
6. Make sure your `json-server` is running on port `8080`, `db.json` file is provided.

**_Note_**: Libraries are not installed, you need to install `axios` and `react-router-dom` yourself.

## Understanding Component Structure

- [App](./src/App.js)
  - [Home](./src/pages/Home.jsx) // Protected Route, accessible post login
    - [Products](./src/components/Products/Products.jsx)
      - [Product](./src/components/Products/Product/Product.jsx)
  - [Login](./src/pages/Login.jsx) //Public Route

**Note** - `Make sure you use only the given components and dont create new files and folders. Changing component name, structures might result in giving you zero marks.`

## Understanding Data Structure

- [db.json](./db.json)
  - Initial Products should be fetched using json-server only after user logs in.
  - cartItems has following operations, accessible post login
    - Add
    - Delete
    - Update Count

**Note** - `Make sure you use only the given data and dont create new data. Changing data might result in giving you zero marks`

## Features to build

1. `/`: `Home` is a protected route, accessible post login.
2. App should redirect to `/login`: `Login` page as soon as he visits the `/` : Home Url.
3. Post `Login`, user should be re-directed to `/`: Home Page.
4. Only Post login User should fetch `/products` and `/cartItems` and populate at required place.
5. Products
   - User Should be able to Add Product to cart, if that product is not already existing in `/cartItems`.
     - Initial Count is 1
   - Increment/Decrement Cart Item Count by Matching Product ID
   - Remove Product from Cart only if Added.

## General Instructions (**_IMPORTANT_**)

1. Do not use Global CSS, instead use `<componentName>.module.css` convention for Css in that file.
2. Do Not Remove `data-cy="xxxx"` from anywhere, this are used by testing tools to test your code, removal of this will lead to low score.
3. Make sure you use only the given components and dont create new files and folders as chaging component name, structures might result in giving you zero marks
4. Make sure you use only the given data and dont create new data, as chaging data might result in giving you zero marks.

## Knowledge Required

1. [React](https://reactjs.org/)
   - useEffect
   - useState
   - useRef
   - createContext
   - useContext
2. [axios](https://axios-http.com/)
   - GET
   - POST
   - PATCH
   - Delete

**Note** - This might not be all the things, you are free to use other components.

#### Submission

- You need to Submit Github Link as well as netify link.
- Make sure you use masai github account provided by MasaiSchool(submit link to root folder of your repository on github).
- Make Sure you have netify account, else you will be getting zero marks as netify takes down your app in few days if your account does not exist.
