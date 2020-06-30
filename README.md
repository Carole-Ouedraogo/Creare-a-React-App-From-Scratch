# react-from-scratch (06/30/2020)

# 1. initialize a new node package

    npm init

After this command completes, it shows a walks-through of creating a package.json file
it only conves the most common item and triedn to guess sensisble

# 2. use default values
It this okay? Press Enter to say YES

# 3 npm install react
This makes a package-lock.json file : This folder manages the versions of the dependencies

# 4. npm install react dom react scripts
This creates the node module folder: This folder contains all the libraries required for React and all to work

# 5. Create  a public directory

  mkdir public

This will contain all the html files, satic assest and react witll be injected here
 - create index.html file
 
# 6. HTML-boiler plate - basic html

add a single dive with an id and a root
div id ='root'></div>
Next create src folder: entry poin to our app
this folder wil contain all the React components will be.
Add title
<title> React</title> in the <head> tag
 
 # 7. 
`mkdir src
import React`
in the index.html file:
  
`import 'React' from 'react'
import 'ReactDom' from 'react-dom'
ReactDom.render(h1>Hello !</h1>, document.getElementById('root')) method takes 2 arguments`

 # 8.
package.json file and add the following line:
        
`"start" : "react-scripts start"`
    
 # 9. Now we can start the project
Configuration in  production and development will be added under the browselist section.
`npm start`
Type `rsc`  and press  Enter to build out a stateless skeleton of a React file
  
components are functions or classes
all components alwas return a jsx
  everything should be capsulated by one <div>
  
  `exports defaultf app` allow s to use the react compoent in other parts of the project
  
  `ReactDom.render(<App />, document.getElementById('root')`

 # 10. In the components folder, create a new component file DefaultButton.js child component
In the parent component App.js:

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
  
  {} Deconstructor
  
  # 11. In the child component DefaultButton.js:
  
    import 'React' from 'react'

    const DefaultButton = () => {
      return (
        <div>
          <button>Click Here</button>
        </div>
      );
    }

    export default DefaultButton;
  
  
  
  
  
  
  
  
