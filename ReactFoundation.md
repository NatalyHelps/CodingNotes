 # Basics of React 
 
 :grey_question: **What is React?**
React is a JavaScript library created by Facebook with the purpose of building user interfaces. Facebook created React because they wanted to make it faster to update dynamic information. Instead of going the slower route in traditional web development where the DOM is updated frequently to reflect UI changes, React introduced a virtual DOM to make this more efficient. React also uses component-based architecture for development, which makes things fast and easy to maintain. 
 
 ---
 
### Components
1. **stateless functional component**: any function you write which accepts props and returns JSX
2. **stateless component**: class that extends React.Component
3. **stateful component**: class component that maintains its own internal state

## Vocabulary
**State**: The part in a component that can change. When a component's state changes, React re-renders it. State is used for data like user input, up-to-date application data, or results of async requests. setState() is used to create and update states.
**Hooks**: let *function* components manage state.

## TIPS
*Try to minimize statefulness so only specific areas control it.* (Encapsulation-modularity)

## Questions for Comprehension
:question: What is the difference between a class component vs a function component? 
