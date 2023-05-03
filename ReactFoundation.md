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
: The part in a component that can change. When a component's state changes, React re-renders it. State is used for data like user input, up-to-date application data, or results of async requests. setState() is used to create and update states. <br>
**Hooks** *function* components manage state.

## TIPS
*Try to minimize statefulness so only specific areas control it.* (Encapsulation-modularity)
*If a component is stateful, it will always have access to the data in state in its render() method. You can access the data with this.state.

## Questions for Comprehension
:question: What is the difference between a class component vs function component? <br><br>

:question: How do you create a state? <br>
: :heavy_check_mark: You create state in a React component by declaring a state property on the component class in its constructor. This initializes the component with state when it is created <br><br>

:question: Where do you initialize the state?<br><br>
: :heavy_check_mark: In the component's constructor, under `super(props);` <br><br>

:question: How do you create a class component? <br>
: :heavy_check_mark: extend React.Component<br><br>

:question: What can I do with state? <br>
: :heavy_check_mark: You can update it, render it in your UI, and pass it as props to child components.
