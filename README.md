[Link to codecademy lesson](https://www.codecademy.com/courses/react-101/lessons/react-forms/exercises/input-onchange)

### React Forms

***Input onChange**

Let’s talk about how forms are handled in React.

In a regular HTML form, the state of the form is typically managed by the browser. It doesn’t update the server until the user hits submit.

Things work a bit differently in React. In a React form, the state of the form can be managed by the component, and updates are triggered by the onChange event. When the user interacts with an input, such as entering or deleting any characters, the onChange event fires and updates the component state.

This allows the component to immediately reflect any changes made by the user and update the view accordingly.

Let’s dive into how it works.






[React Forms
Controlled vs Uncontrolled
](https://www.codecademy.com/courses/react-101/lessons/react-forms/exercises/controlled-vs-uncontrolled)


### React Forms

**Controlled vs Uncontrolled**

There are two terms that will probably come up when you talk about React forms: controlled component and uncontrolled component.

An uncontrolled component is a component that maintains its own internal state. A controlled component is a component that does not maintain any internal state. Since a controlled component has no state, it must be controlled by someone else.

Think of a typical <input type='text' /> element. It appears on the screen as a text box. If you need to know what text is currently in the box, then you can ask the <input> element, possibly with some code like this:

let input = document.querySelector('input[type="text"]');

let typedText = input.value; // input.value will be equal to whatever text is currently in the text box.

The important thing here is that the <input> element keeps track of its own text. You can access what its text is at any time.

The fact that <input> keeps track of information makes it an uncontrolled component. It maintains its own internal state by remembering data about itself.

A controlled component, on the other hand, has no memory. If you ask it for information about itself, then it will have to get that information through props. Most React components are controlled.

In React, when you give an <input> element a value attribute, then something strange happens: the <input> element becomes controlled. It stops using its internal storage. This is a more “React” way of doing things.

Recall that in our exercises, the page updated every time we typed into the input. React controlled the input’s value with the state. We’ve been demonstrating the idea of a controlled component all along!

You can find more information about controlled and uncontrolled components in the React documentation.

