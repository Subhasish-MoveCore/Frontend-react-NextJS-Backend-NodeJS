# React Props Example

This project demonstrates how to use **Props** in React.

## 📌 What are Props?

Props (short for Properties) are used to pass data from one component to another in React.

- Props are read-only
- They help make components reusable
- Data flows from parent → child component

---

# 📂 Project Structure

```bash
src/
│
├── App.js
├── Student.js
└── index.js
```

---

# 🚀 Example

## App.js

```jsx
import React from "react";
import Student from "./Student";

function App() {
  return (
    <div>
      <h1>React Props Example</h1>

      <Student name="Subhasish" branch="CSE" />
      <Student name="Rahul" branch="ECE" />
    </div>
  );
}

export default App;
```

---

## Student.js

```jsx
import React from "react";

function Student(props) {
  return (
    <div>
      <h2>Name: {props.name}</h2>
      <p>Branch: {props.branch}</p>
    </div>
  );
}

export default Student;
```

---

# ✅ Output

```bash
React Props Example

Name: Subhasish
Branch: CSE

Name: Rahul
Branch: ECE
```

---

# 🔥 Using Destructuring Props

```jsx
function Student({ name, branch }) {
  return (
    <div>
      <h2>{name}</h2>
      <p>{branch}</p>
    </div>
  );
}
```

---

# 📖 Key Points

- Props are used to send data to components
- Props make components reusable
- Parent component passes props
- Child component receives props

---

# 🛠️ Installation

```bash
git clone <your-repository-link>

cd react-props-example

npm install

npm start
```

---

# 📚 Technologies Used

- React.js
- JavaScript
- CSS

---

# 👨‍💻 Author

Made with ❤️ using React