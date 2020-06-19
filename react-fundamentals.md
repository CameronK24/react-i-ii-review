### Remember

Answer these on your own, then compare answers as a group

1.  What is React?
      A javascript library to make websites more dynamic and interactive.

2.  What is create-react-app?
      Terminal command to create a react library, sets up the tools you need to create a react app.

3.  What is Component Based Architecture?
      Dividing your app into reusable component files.

4.  What is JSX?
      React elements similar to HTML.

5.  What is the virtual DOM?
      A non viewable version of the real DOM that React makes changes too before pushing them to the live DOM

6.  What is unidirectional (one-way) data flow?
      Data flowing from parent to child but it can't flow from child to parent.

### Understand

Discuss these questions in pairs if you have a 4-person group

7.  Summarize what happens when you run `create-react-app my-app`
      Creates a react app with the name you give it in the directory your in.

8.  Explain what this code does:
      Imports react, a functional component named mentor takes its parents "props" that are passed when it is called and returns the JSX code inside it, and exports it.9

```jsx
import React from "react";

const Mentor = props => (
  <div className="mentor-container">
    <h1 className={props.title === "Lead Mentor" ? "lead" : ""}>Tim Biles</h1>
    <ul>
      <li>Fort Worth, TX</li>
      <li>My email address is timbilestimbiles@gmail.com</li>
    </ul>
  </div>
);

export default Mentor;
```

9.  Explain how data is passed from a parent component to a child component.
      By using Props.

### Apply

Try these on your own, but work together if you start to get stuck.

10.  Use `create-react-app` to create a new React application called `student-directory`

11.  Use the code from `Mentor` above to create a new functional, stateless component called `User` with a list of friends. Hard code the list of friends, do not use state or props.

### Analyze, Evaluate, Create

Discuss these questions as a group

12. What are the benefits and drawbacks of using a tool like create-react-app?
      Benefits: 
        We can throw together a react app quickly
        we can install the individual pieces seperately required in a react app
        most of the setup is already done for us
      Drawbacks:
        it could potentially install something we don't need leading to a bigger app size.
        see link: https://reactjs.org/docs/create-a-new-react-app.html

13. Compare and contrast JSX with other templating options, such as those used in Angular or Vue

14. Compare and contrast one-way data flow with two-way data binding.
      one-way = unidirectional
      two-way = bidirectional
