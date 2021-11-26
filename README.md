## Ya welcome , we will explain how to get started with React  how to make a counter in react
---------------------------------------------------------------
> **_NOTE:_** 
> - React is a javascript library and use jsx extension for her files [Read more](https://www.geeksforgeeks.org/jsx-full-form/)<br>.
> - React create a single page application [Read more ](https://en.wikipedia.org/wiki/Single-page_application).
> - For linux to get full permissions (root) in terminal: sudo su -
> - className attribute in react used instead of class [Read more ](https://www.geeksforgeeks.org/why-react-uses-classname-over-class-attribute/).
> - in this explanation we will use vs code editor .
> - we will use "simple react snnipets" vs code extension to make it easy [Read more](https://www.digitalocean.com/community/posts/write-react-faster-with-simple-react-snippets).
> - we will use bootstrap css framework [Read more](https://websuggestion.com/why-bootstrap-is-better-than-css/).
> - when are you running server the page will refersh automatically when you edit any thing in code
> - and will give you if there was any error in the code in the console .

## 1- First we will download node js which will need him in npm to create react app
 **Windows** [Download](https://nodejs.org/dist/v16.13.0/node-v16.13.0-x64.msi) <br>
 after download setup the program <br>
 
 **Linux DEB** in terminal <br>
 ```bash
 sudo apt install nodejs  
 sudo apt install npm 
 ```
 ## 2- We will install create-react-app package
 in terminal(cmd) type
 ```bash
 npm i -g create-react-app
 # npm : node js package manager
 # i: install
 # -g : global to install create-react-app
 
 ```
 ## Now we will create  first-app in terminal :
 ```bash
 create-react-app first-app 
 ```
 If you have a message "happy hacking" congratulation 
 elseif you have a problem tell me 
 ## 
## 3- we will check the server 
in terminal:
```bash
cd first-app
npm start 
# wait a minute then your default browser will open in localhost:3000 and react logo will appear 
# now get back to the terminal and click ctrl + c to close server 
```
## 4- Now we will install bootstrap framework inside application so in terminal :
```bash
 npm i bootstrap 
```
## 5- Install vs code extension (simple react snnipets) 
Now we are in first-app (in terminal i mean ) so open your editor in same file 
```bash
in terminal: 
code . 
# you can use your editior 
# code . mean open visual code in same file 
```
Go to extensions click `ctrl` `+` `shift` `+` `x`:
serach "simple react snnipets" and install it 

## 6- Import bootstrap 
git back to explorer click `ctrl` `+` `shift` `+` `E` , go to the src folder to index.js file type inside him 
```python
import "bootstrap/dist/css/bootstrap.css";
```
> _**NOTE:**_ now we will create counter ,import him and use it instead app then return app in counters 
## 7- Create counter file 
in src folder create new folder name him "components"
inside components create a new file name him "counter.jsx" 
now inside him type 
```javascript 
imrc 
cc
```
imrc to import react component 
cc to class component 
now our code will be like this 
```python 
import React, { Component } from 'react';


class  extends React.Component {
    render() { 
        return <div></div>;
    }
}
 
export default ;
```
## 8- Now we'll name the class : 
class name after class and after export default 
look to the new code 👀 :
```python 
class Counter extends React.Component {
    render() { 
        return <div></div>;
    }
}
 
export default Counter ;
``` 
## 9- Now if we want to show our content in page we must write in render function and return our data:
we need an increment button and span to show the number 
html structure 
```python 

class Counter extends React.Component {
    render() { 
        return <div>
            <button>Increment </button>
            <span> 0 </span>
        </div>;
    }
}
 
export default Counter ;
```
## Style By bootstrap 
```html 
        <span   className="badge bg-primary m-2"> 0 </span>
        <button className="btn btn-secondary">Increment </button>
```
## 10- --Cross step-- We want to show our page and what is going on 
  in src folder in index.js file (where we import bootstrap )<br>
  comment importing app class (we comment it just for now we will use it later )
  ```javascript
   // import App from './App';
   ```
   import our Counter (counter class )
   ```javascript
   import Counter from './components/counter';
   ```
   between react.strictmode replace app and type Counter 
   `don't forget captalize c `
   ```javascript 
   <React.StrictMode>
    <Counter/>
  </React.StrictMode>,
  ``` 
  ## now we will run the server and see the counter page 
  open terminal in this app  as we do it before and type :
   `npm start`
   now we will get back to counter.jsx file 
  ## 11- Make the counter alive (make the functions)
  first we will put default value in span (in page)
  so in Counter class add this 
  ```python 
  state = {
        count: 0
    };
   ```
  then go to span tag  replace zero and type : 
  ```html
      <span className="badge bg-primary m-2"> {this.state.count}</span>
  ```
  
  the first function is Increment which will increase the number
  




