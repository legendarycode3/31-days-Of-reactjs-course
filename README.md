 ## MASTERING REACTJS COURSE WITH EXCERCISES <br/>


➡️ **REACT BASICs, JSX  --  LESSON 1**  </br>
✔️ What is Reactjs ?  </br>
React is an external library that helps us create websites easier. </br>

✔️ What is JSX ? </br> </br>
Javascript XML Is a syntax extension for javascript that allows developers to write HTML -like markup directly within  their Javascript code. </br>
JSX looks very similar to HTML but it is not (becus it has different syntax). </br>

NOTE: JSX is more strict than  normal HTML.  All elements need a closing tag.  </br>
E.g  </br>
<input placeholder="Send a message to Chatbot" size="30"></input>  </br>
But if you not goona put anything inside or nothing inside our element , you can use a “self closing tag” like this <input /> </br>


✔️ What is Babel ?  </br>
Babel is known as a “Javascript compiler”. It basically translate other languages into javascript. </br>
Why do we need Babel: </br>
When using “React”, we actually don’t use normal javascript, we use an “enhanced version of javascript” called JSX.  </br>
JSX stands for “Javascript  XML”. Is the same as javascript but we can also write HTML directly in our javascript code.	</br>



➡️ **COMPONENTS, PROPS, SHORTCUTS IN REACT - LESSON 2** </br>
✔️ What is Component ? </br>
Is one of the most important features of Reactjs called “Component”. </br>
A component is just a piece of  a website.  </br>
To create a “component” in React, we goona use a function. </br>
Components are designed to be reusable(using attribute). </br>
Components lets us create our own  HTML elements. </br>

NOTE: We can have  “components” inside of a component. It helps us split our website , into smaller & smaller components or smaller and smaller pieces. </br>
✔️ Fragment: In Reactjs, we use it to group elements together. It helps us not to have extra div, if we don’t. </br>

✔️ What is Props ?  </br>
Every “component function”, gets one parameter called props. </br>
The “props”  parameter is an object and it will contain all the attributes that we give to any component.  </br>
Props, is the short form for properties. </br>
Using the “props object” we can access our attribute & also make our components reusable. </br>
Props, helps us to be able to pass data from one component to another. To display something specific & not create & not create multiple similar components (for every little change). You typical do it from a parent component to a child component. </br>

✔️ShortCuts Commonly Used In Reactjs ? </br>
Some “shortcuts” that are commonly used in React, they include </br>
1) Using javascript instead of doing this  **const message = props.message; and const sender = props.sender;**  We can use this **const {message, sender} = props;** which is a shortcut for that 2 different const variables. And this shortcut is called “destructuring”. </br>




➡️ **STATE, EVENT HANDLERS - LESSON 3** </br>
✔️ What Is State ?  </br>
State is a built-in object that allows components to store and manage dynamic data that changes over time. State helps us make a website interative. </br>
“State” is a data that is connected to the HTML (meaning , when we update the data , it will update the HTML). To convert data’s into state, we use React.useState() & useState() givs us two values (which are: The current data & Updater function).  </br>
“State” is like a React component brain. It holds the information the components that can change over-time. </br>
When a component state changes (usually in response to users input or an API call),  React automatically re-renders the component to reflect the new data in the UI. </br>

NOTE: Keep in mid that in React (State) , anything that starts with “use” , is typically refered to as a Hook (e.g useState) </br>

✔️ What Is useState? </br>
 The useState hook in React allows functional components to have State. Which is local memory for data that needs to change over time or across user interaction. </br>
In modern React, the useState hook is used to add state to functional components. </br>
- useState hook, for managing state. </br>
This mechanism allows components to be dynamic and interactive , reacting to changes without a full page refresh. </br>

✔️ Differences Between “State” And “useState”?  </br>
State: State is a core concept. It refers to the data or properties that a component needs to remember overtime. The data can always change based on user interactions or network responses, and when it does, React re-renders the component to update the user interface. </br>
useState: useState is a specific tool(a Hook) provided by React to manage that concept within functional components to use State. </br>
To use the “useState” , you call the “useState” within a functional components to declare a state variable ,. It returns an array  containing (the following 2 properties): </br>
1. The current state value. </br>
2. The function to update that value (which triggers a re-render). </br>

“In Summary”, useState is the mechanism for adding  the concept of  “state” to a modern functional component. </br>

✔️ What Is Event Handler ?  </br> 
Event Handler lets us run a function when we interact with the website.  </br>
In React, “Event handlers” we use to manage user interactions, like clicking , typing, or hovering , making your UI dynamic. </br>
Event Handlers , are declared directly in the JSX using a camalCase naming convention (e.g., onClick instead of onclick), and a function is passed as the handler’s value , not a string. </br>
E.g Diagram below shows a brief differenciation between an “Event” & “Event Handler” </br>





➡️  **USING CSS WITH REACT, HOOKS () - LESSON 4** </br>
✔️ CSS WITH REACT (What is CSS) ?  </br>
Change the appearance of the website. We can use Css in React.js ,the normal ways. </br>
Some Ways We Can Use CSS With React.js:- Here are the primary ways to use CSS in React, they include: </br>

1.) External CSS Files(Standard Method): </br>
This method is similar to traditional HTML development. Styles are defined in separate .css files and imported into the relevant component file. </br>
Best For: Global styles and large components. </br>
Pros: Familiar syntax, separation of concerns. </br>
Cons: Styles are global and can cause naming conflicts across different components in large applications. </br>

2.) Inline Styles: </br>
Internal CSS styling are suitable for styles that are unique to a single page. They are defined within the <style> tag. </br>
You can apply styles directly to elements using the style attribute, which accepts a JavaScript object where keys are camelCase CSS properties. </br>  
Best For:  simple, one-off cases.

3.) CSS Modules: </br>
This approach uses standard CSS files but automatically scopes class names locally to the component they are imported into, preventing naming conflicts and style overrides. </br>
Best For: Preventing naming conflicts in large projects.. </br>
Pros: Uses familiar CSS syntax, avoids global scope issues, and works well for component-specific styles. </br>
Cons: Requires a specific file naming convention (.module.css), and dynamic styling based on component props is more complex than with CSS-in-JS libraries. </br>

4.) Styled Components (CSS-in-JS): </br>
This library allows you to write actual CSS in your JavaScript using tagged template literals, creating components with styles embedded within them. </br>
Libraries like styled-components allow you to write actual CSS code directly within your JavaScript files using tagged template literals.  </br>
Best For:  Encapsulated, reusable, styleable components. </br>
Pros: Enables dynamic styling using JavaScript logic (props and state), automatically generates unique class names for scoping, and keeps styles and component logic in one place. </br>

5.) Tailwind CSS(Utility First framework): </br>
A utility-first CSS framework that provides a vast set of pre-defined utility classes directly in your JSX markup. </br>
Tailwind CSS provides a vast set of pre-defined utility classes that you apply directly to your elements in the JSX. </br>
Pros: Speeds up development, minimizes the need for writing custom CSS files. 
Accelerates development and promotes design consistency by using a fixed set of classes, is highly customizable, and purges unused styles for small file sizes in production. </br>
Cons: Can make the markup look cluttered; requires setup and configuration. 
Can lead to verbose HTML markup, has a steep learning curve if unfamiliar with the utility-first concept, and customization beyond its core utilities may require additional CSS. 

5.) Internal Style: </br>
NOTE:In React.js , we use className (to set the class),  that’s becus , </br>
i.  React, is actually just javascript code. </br>
ii.  And Javascript already have a feature called class. </br>
iii.  So class, is a reserved word. </br>
NOTE: Best Practices (in General) for Any Approach: 
Regardless of the chosen method, following general best practices will improve maintainability and scalability: </br>
a) Ultimately, CSS Modules provide a balanced, scalable solution without requiring a third-party library </br>
b) while Styled Components offer powerful dynamic styling capabilities. </br>
c) Tailwind CSS excels at rapid prototyping and development speed. </br>

The right choice depends on your project's specific context…..  </br>
For most use cases beyond simple dynamic values(in-line styling), using external CSS files or CSS modules provides better style management 
and separation of concerns than strictly inline styles. </br>

✔️ Hooks ?  One of the important features in Reactjs.  </br>
Hooks lets us insert “React” features into our component. </br>
Hooks, are special functions in react, that allows you tap into react features (e.g like “state management”) </br>
 Meanwhile, we have actually used “hooks”  before , React.useState()  is a hook </br>
E.g const [inputText, setInputText] = React.useState(‘’); </br>

Reactjs , has other hooks we can use in a project (e.g useState() , useEffect() , useRef() and more ) </br>

1. useEffect() Hook: </br>
This hook is used for handling side effects like data fetching. </br>
- This hook lets us run some code after the component is created or updated.  </br>
It allows you to perform side effects in functional components, such as data fetching , subscriptions, or manual DOMupdates. 
 It runs after the component has rendered and the browser has updated the screen.  </br>
- useEffect(), lets us do things outside of just displaying stuff on the screen (e.g like fetching data from the server, or doing some cleanup after the data has been rendered). </br>
If you give useEffect(), an empty array [] - which is called a “dependency array.  
It lets use control when useEffects runs”, useEffect() will only run once. </br>

2. useRef() Hook: </br>
Automaticallly save an HTML element from the component.  This code, will create a “ref”. </br>
A ref is a container with spacial React features. </br>

3. useContext() Hook: </br>
Is used for sharing  data across somponents. </br>

4.  useMemo() Hook :- </br>
is a performance optimization tool that caches (memoizes) the result of an expensive calculation and reuses the cached value unless its dependencies change. </br>

5. useCallback() Hook: </br>
For optimizing callback function.

6. useReducer() Hook: </br>
The useReducer() Hook is a powerful alternative to useState() in React used for managing more complex state logic.  </br>
It centralizes the state management logic into a single, separate function called a reducer, which makes the code more predictable, maintainable, and testable.  </br>

7. useTransition() Hook:  </br>
User interactions and keeps the application responsive. </br>
NOTE:   Things to note about using “Hooks”, they include:  </br>
i. Always put your “Hook” at the Top of your component . </br>
ii. Hooks should not be inside anything. (e.g never put inside a “if-statement” , inside a function) </br>





➡️  **PROPER REACT SET-UP - LESSON 4**  </br>
✔️ Proper React Setup : Will let us split up our codes (e.g javascript, React, Css) into different files and folder. </br>
NOTE: To create this “React” , we need to review the following 2 key notes. </br>
1.  Reviewing The CommandLines() using it on VSCode terminal:  They include: </br>
    mkdir  =  make directory (A directory is another name for a “folder”).
    Make diectory creates a new folder. </br>
    E.g  mkdir test </br>
    pwd    =   Print the  work directory / folder.  It  displays the full absolutely path of the directory  you are currently in.
    cd  =   Change directory. Allows us to change the current working directory / folder. </br>
    Cd  ..  =   It is used to move up one level in the directory / folder hierarchy  (.. represents the outer folder or directory). It is used to get-out of a folder. </br>
2.  Reviewing Nodejs (some) using it on VSCode terminal:  They include: </br>
   - node    =  This command lets us run JavaScript code outside  of the browser. </br>
      Used to execute JavaScript code outside of a web browser. </br>
      It is the primary tool for running Node.js scripts and interacting with the Node.js environment. </br>
   - npm    =  The command stands for  Node Package Manager. A “package” is basically a library .  </br>
     So therefore, npm , lets us install external libraries (or packages) into our project. </br>
     E.g  npm install legendarycode </br>
  - npm install   =  Contains the list of packages needed for a particular project folder </br>
  - npm run dev   =  Starts up our new React Website (when we created it using the npx create-vite) </br>
  - npm create vite@latest  my-react-app   =  For creating a new React app. </br>
   https://vite.dev/guide/ </br>
  - npm run dev how it works  = “npm run”  tells the computer to look inside  package.json for a section called “scripts” for “dev” and run the command on the right side of “dev” (which is vite). </br>
  NOTE: package.json contains all the “list of packages needed for a particular project folder” </br>
  - So when you type npm install (on the terminal , on the folder you want which was just created) it going to install all of the packages the same time(when you just created a proper react setup).   </br>
  - After this is done, all of the packages will be downloaded on node_modules folder. </br>

  Below Are SomeFiles Found In Reactjs (when Newly Created Projects): </br>
  - .gitignore file, allows developers to specify which files and directories should be excluded from version control (Git).  
   This helps keep repositories tidy, preventing sensitive information from being exposed , and ensures that only essential files are tracked. 
   This file tells git which files and folders to ignore when pushing your code. 
   E.g node_modules, .env , should never be pushed to github </br>

 - eslint Highlights problems in our JavaScript Code. </br>
   EG. Lets say you mistakely mispelled something when writing code in VSCode. 
   VSCode will not show you the error, but eslint will indentify the error for you when you install it, the extension. </br>
   A good tool that highlights problem in our javascript tool. 
   eslint.config.js  Is a config file used to define the rule s and settings for ESLINT. </br>

- package-lock.json , has a list of packages that we need to install to run the Reactjs (newly created Vite project) </br>
  package-lock.json , saves the version numbers of all the packages that we installed. 
  Npm automatically updates package-lock.json , so we don’t need to change any file on it. </br>

- package.json contains all the “list of packages needed for a particular project folder”. </br>
  Package.json contains the meta-data of our project (such as it: “name”, “scripts”, “dependencies”)
  The “dev” : “vite” -  the script starts the development server. </br> 
  The “build”: “vite build” - the script create the production build. </br>

- README.md  This is just text, it provides more information about the project.  
  It is not code, it is just forinformational purposes (don’t need to be changed). </br>
This file contains the information about the project (like: how to run it, what the project those & other documentation). </br>

- vite.config.js : Configures Vite. </br>
Vite is the tool that we use to setup a particular project. </br>
Vite also helps us build a Website (it takes all the javascript and css and then load then into the html file). </br>
Vite also creates a server.  A server puts our websiteat a URL (localhost:5173).
Vite server  is a replacement for the “Live Server” we normally use to refresh some code. </br>
