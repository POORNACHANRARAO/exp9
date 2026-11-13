# Exp 9 – React Lab Exercise: React Fragments

## NAME:  kunam poorna chandra rao
## REG NO: 2305001012

## Aim
To understand and implement React Fragments to group multiple JSX elements without creating unnecessary HTML elements in the DOM.

## Objectives
- Understand the concept of React Fragments.
- Use Fragment shorthand syntax.
- Use the explicit Fragment syntax.
- Group multiple JSX elements without an extra DOM node.
- Understand the difference between Fragments and div elements.

## Program

### Step 1: Create a React Project

```bash
npm create vite@latest react-fragments
cd react-fragments
npm install
npm run dev
```

Select React as the framework and JavaScript as the variant.

### Step 2: App.jsx – Using Fragment Shorthand

```
function Student() {
  return (
    <>
      <h2>Student Details</h2>

      <h3>Name: KUNAM POORNA CHANDRA RAO</h3>

      <p>Register Number: 2305001012</p>

      <p>Department: Computer Science and Engineering</p>
    </>
  );
}

function App() {
  return (
    <>
      <h1>College Information System</h1>

      <Student />
    </>
  );
}

export default App;
```

### Step 3: Using Explicit Fragment Syntax

```jsx
import { Fragment } from "react";

function Student() {
  return (
    <Fragment>
      <h2>Student Details</h2>
      <p>Name: KUNAM POORNA CHANDRA RAO</p>
      <p>Department: CSE</p>
    </Fragment>
  );
}

function App() {
  return (
    <Fragment>
      <h1>College Information System</h1>
      <Student />
    </Fragment>
  );
}

export default App;
```

## Output

### Fragment Shorthand Syntax
<img width="773" height="427" alt="image" src="https://github.com/user-attachments/assets/29ecb584-3c32-4785-9b99-f6981895ff83" />



### Explicit Fragment Syntax
<img width="830" height="418" alt="image" src="https://github.com/user-attachments/assets/09ac463a-2dc5-4204-bc2e-2cdd4ad3dc1e" />



## Result

Thus, React Fragments were successfully implemented using shorthand and explicit syntax to group multiple JSX elements without creating unnecessary DOM elements.
