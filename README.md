
# Course Module: Deepening Knowledge in Hooks by @RocketSeat

In this course, I learned how to build a complete application with routing and various important concepts from the React ecosystem, such as ContextAPI, useReducer, immer, and much more.

I will briefly describe one of the topics I learned during this course.

## Context API in React

The **Context API** in React is a powerful tool for sharing data between components in a React application, avoiding the need to manually pass props at each level of the component tree. This helps solve the problem known as **prop drilling**.

### What is Prop Drilling?

**Prop drilling** occurs when you need to pass data from a parent component to a distant child component in the component hierarchy, traversing several intermediate levels that do not directly use this data. This pattern makes the code difficult to maintain and prone to errors.

### How does Context API help?

The **Context API** allows you to create a context that can be accessed by any component, at any level of the tree, without the need to manually pass props. This is done through two main components: **Provider** and **Consumer**.

### Steps to use Context API

1. **Creation of Context:** Create a context using `React.createContext()`.
2. **Provider:** Use the `Provider` to wrap the part of the component tree where the context should be accessible and provide the value to be shared.
3. **Consumer:** Use the `Consumer` or the `useContext` hook to access the context in child components.

### Code Example
 
[CyclesContext.tsx](src/contexts/CyclesContext.tsx) Creation of context.

![image](https://github.com/user-attachments/assets/74047a24-9b0f-42cc-968c-e72e2b4d19f8)

![image](https://github.com/user-attachments/assets/0fc90750-1c3d-416e-b2e7-6ec44ec73aa8)


[App.tsx](src/App.tsx) Making the context recognized throughout the application by wrapping all routes.

![image](https://github.com/user-attachments/assets/4fb1a7d6-d467-437f-9223-ed4217a5d78b)

