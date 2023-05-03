 # Basics of React 
 
 :grey_question: 
 **What is React?**
React is a JavaScript library created by Facebook with the purpose of building user interfaces. Facebook created React because they wanted to make it faster to update dynamic information. Instead of going the slower route in traditional web development where the DOM is updated frequently to reflect UI changes, React introduced a virtual DOM to make this more efficient. It only updates the DOM when necessary. React also uses component-based architecture for development, which makes things fast and easy to maintain. 

 :grey_question: 
 **What are Components?**
 
 ---
 
### Components
1. **stateless functional component**: any function you write which accepts props and returns JSX
2. **stateless component**: class that extends React.Component
3. **stateful component**: class component that maintains its own internal state

## Vocabulary
**State**
: As in, the current state of the application. It is the part in a component that can change. When a component's state changes, React re-renders it. State is used for data like user input, up-to-date application data, or results of async requests. setState() is used in class components to create and update states. <br>
**Hooks** 
: are *function* components that manage state like useState()<br>In contrast, setState() is used for class components and is not a hook but a method available on class components.

## TIPS
*Try to minimize statefulness so only specific areas control it.* (Encapsulation-modularity)
*If a component is stateful, it will always have access to the data in state in its render() method. You can access the data with this.state.

## Questions for Comprehension
:question: What is the difference between a class component vs function component? <br><br>

:question: How do you create a state? <br>
: :heavy_check_mark: By declaring a state property `this.setstate` on the component class in its constructor. The component is then created with a state and becomes stateful.<br><br>

:question: Where do you initialize the state?<br>
: :heavy_check_mark: In the component's constructor, under `super(props);` <br><br>


:question: How do you access state? <br>
: :heavy_check_mark: 1) In the render method. Inside of the return. <br>
2) Or in the render, before the return, you can write the JavaScript directly. (Without curly braces) Here you can write functions, access data, create variables etc. <br><br>

:question: How do you create a class component? <br>
: :heavy_check_mark: `extend React.Component` (Using ES6 class syntax)<br><br>

:question: What can I do with state? <br>
: :heavy_check_mark: You can update it, render it in your UI, and pass it as props to child components.
