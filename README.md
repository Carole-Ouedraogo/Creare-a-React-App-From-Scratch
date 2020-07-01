# Creare a React App From Scratch 

# 1. initialize a new node package

    npm init

After this command completes, it shows a walks-through of creating a package.json file
It only convers the most common items and tries to guess...

# 2. Accept default values if prompted to answer Qs
Last step: It this okay? Press Enter to say YES

# 3 Installing the package

`npm install react`
This makes a package-lock.json file : This folder manages the versions of the dependencies

# 4. Create Node Module

`npm install react dom react scripts`

This creates the node module folder: This folder contains all the libraries required for React and all to work.

# 5. Create a public directory

  `mkdir public`

This will contain all the html files, satic assest and react witll be injected here
 
 
# 6. HTML-boiler plate - Basic HTML

- create index.html file
- add a single div with an id and a root
`div id ='root'></div>`
- create src folder: this is the entry point to our app
this folder wil contain all the React components will be.
- Add title `<title> React</title>` in the <head> tag
- in the index.html file:
  
```javascript
import 'React' from 'react'
import 'ReactDom' from 'react-dom'
ReactDom.render(h1>Hello !</h1>, document.getElementById('root'))`
```
This method takes 2 arguments...

 # 7. Create a src directory
 
 `mkdir src`


 # 8. Settings
Inside the package.json file,  add the following line:
        
`"start" : "react-scripts start"`
    
 # 9. Now we can start the project
Configuration in  production and development will be added under the browselist section.

`npm start`

Type `rsc` in the App.js file and press  Enter to build a stateless (skeleton) the React file.
This is shortcut of a out of Reactjs code snippets  

components are functions or classes
All components always return a jsx
Everything should be incapsulated by one <div>
  
`exports defaultf app` allow s to use the react component in other parts of the project
  
`ReactDom.render(<App />, document.getElementById('root')`

 # 10. In the components folder, create a new component file DefaultButton.js child component
In the parent component App.js:

```javascript
import 'React' from 'react'
import 'DefaultButton from './components/Butons/DefaultButton' 
from 'react-dom'
ReactDom.render(h1>Hello!</h1>)

const App = () => {
  return (
    <div>
      <h1>Select State</h1>
      <DefaultButton/>
    </div>
  );
}

export default App;
```
  
  
  # 11. In the child component DefaultButton.js:
  
  ```javascript
    import 'React' from 'react'

    const DefaultButton = () => {
      return (
        <div>
          <button>Click Here</button>
        </div>
      );
    }

  export default DefaultButton;
``` 

# {} Destructuring Props in React

Imagine you have a person object with the following properties:
```javascript
const person = {
  firstName: "Lindsay",
  lastName: "Criswell",
  city: "NYC"
}
```
With Destructuring Props,

```javascript
const { firstName, lastName, city } = person;
```

is equivalent to:

```javascript
const firstName = person.firstName
const lastName = person.lastName
const city = person.city  
```

Other: emmet cheatsheet https://docs.emmet.io/cheat-sheet/
  
@Carole Ouedraogo
(06/30/2020)
  
