 # Basics of React 
 
 :grey_question: 
 **What is React?**
React is a JavaScript library created by Facebook with the purpose of building user interfaces. Facebook created React because they wanted to make it faster to update dynamic information. Instead of going the slower route in traditional web development where the DOM is updated frequently to reflect UI changes, React introduced a virtual DOM to make this more efficient. It only updates the DOM when necessary. React also uses component-based architecture for development, which makes things fast and easy to maintain. 

 :grey_question: 
 **What are Components?**<BR>
 Each react component is a different part of the interface such as Navbar and Searchbar. 
 ---
 
### Components
1. **stateless functional component**: a JavaScript function used to define a React component. It accepts props and returns JSX. Must have a return statement. Simple calculations can come before the return statement. 
2. **stateless component**: class that extends React.Component
3. **stateful component**: class component that maintains its own internal state

## Vocabulary
**State**
: As in, the current state of the application. It is the part in a component that can change. When a component's state changes, React re-renders it. State is used for data like user input, up-to-date application data, or results of async requests. setState() is used in class components to create and update states. <br>
**Hooks** 
: are *function* components that manage state like useState()<br>In contrast, setState() is used for class components and is not a hook but a method available on class components.

## TIPS
*Try to minimize statefulness so only specific areas control it.* (Encapsulation-modularity)<br>
*If a component is stateful, it will always have access to the data in state in its render() method. You can access the data with this.state.*<br>
*You can't rely on the previous value of this.state or this.props when calculating the next value because React may batch multiple setState() calls into a single update.*<br>

## Questions for Comprehension
:question: **What is the difference between a class component vs function component?** <br><br>

:question: **How do you create a state?** <br>
: :heavy_check_mark: By declaring a state property `this.setstate` on the component class in its constructor. The component is then created with a state and becomes stateful.<br><br>

:question: **Where do you initialize the state?**<br>
: :heavy_check_mark: In the component's constructor, under `super(props);` <br><br>


:question: **How do you access state?** <br>
: :heavy_check_mark: 1) In the render method. Inside of the return. <br>
2) Or in the render, before the return, you can write the JavaScript directly. (Without curly braces) Here you can write functions, access data, create variables etc. <br><br>

:question: **How do you change state?** <br>
: :heavy_check_mark: In your component class, call this.setState(). You pass in an object with key-value pairs. The key is your property and the value is your updated state data. <br><br>
:question: **How do you create a class component?** <br>
: :heavy_check_mark: `extend React.Component` (Using ES6 class syntax)<br><br>

:question: **What can I do with state?** <br>
: :heavy_check_mark: You can update it, render it in your UI, and pass it as props to child components.

:question: **How do you bind this to a class method like handleClick?** <br>
: :heavy_check_mark: Example used with the method handleClick() <br>
`this.handleClick = this.handleClick.bind(this);`<br><br>

:question: **What is a controlled component?** <br>
: :heavy_check_mark:
In React, a controlled component is a component where the value of its form elements, such as input, textarea, and select, are controlled by React state. In other words, the React component state serves as the single source of truth for the input's value, instead of the DOM. When a user types into an input field, the React component state is updated, and the input value is set to the updated state value. This way, the React component has full control over the input, and can modify or validate its value before rendering it. Controlled components are commonly used in React forms to achieve a more predictable and deterministic behavior.<br><br>
 
 :question: **What is a React root container?**<br> 
: :heavy_check_mark: top-level container element into which all the React components are rendered. It's usually a div element in the HTML file where the React application is mounted using the ReactDOM.render() method.
 
 When the React application is initialized, the root container is used to render the root component of the application. From there, all other child components are rendered inside the root container as necessary.<br><br>
Example:<br>
 `ReactDOM.render(`<br>
  `<React.StrictMode>`<br>
  `  <App />`<br>
 ` </React.StrictMode>,`<br>
 ` document.getElementById('root')`<br>
`);`
 <BR>
 Here, `document.getElementById('root')` specifies the root container element, where the React application is mounted.<BR>
 
  
 :question: **What is the `createRoot()` method?** <br>
 : :heavy_check_mark: we call the createRoot method to create a React root container for displaying content. 
  React applications typically have a single root DOM node, and everything inside it is managed by React DOM.
 <BR><BR>
   In other words, we give createRoot a DOM element to render in, and React will take over managing the DOM inside it.
   In `ReactDOM.createRoot(document.getElementById('app'));`<br><BR>
     ` document.getElementById('app')` returns a DOM element from index.html.<br><BR>
`.createRoot()` receives the DOM element as the first argument and creates a root for it.<br><BR>
`.createRoot()` returns a reference to the root container on which you can call methods like `.render()`.<br><BR>
  After the root is created, all that’s left to do is call the .render() method on the returned root and display the React component like so:<BR>
  `ReactDOM.createRoot(document.getElementById('app')).render(<MyComponent />);`<BR><BR>
  passing props:  in React, the attributes that you pass to a component when you render it become part of the props object 
  
   :question: **What does useState() return?**<br>
 : :heavy_check_mark: The useState hook in React returns an array containing two elements: the current state value and a function to update that state value. <br>
  Note that setState() is not a hook, but just a method available on class components. 
  `const [state, setState] = useState(initialValue);`<BR><BR>
  state is the state variable, while setState is a function that allows you to update the state value. <BR>
  With setState you can provide a new state value or a callback function that receives the previous state and returns the new state.




