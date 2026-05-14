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
├── Components
  ├── Card.js
```

---

# 🚀 Example

## Card.js

```jsx
import React from 'react'

const Card = (props) => {
  return (
      <div className="card">
        <img src={props.img} alt="" />
        <h1>{props.user}</h1>
        <p>{props.para}</p>
        <button>view profile</button>
      </div>
  )
}

export default Card
```

---

## App.js

```jsx
import React from 'react'
import Card from './components/Card'
const App = () => {
  return (
    <div className="card-container">
      <Card user ='Subhasish' para="This is Subhasish's card." img="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSi6bfvI53IKkEsh7UbcxXyQnkzzAj0pPWlgQ&s"/>
      <Card user ='Mohit' para="This is Mohit's card." img="https://static.vecteezy.com/system/resources/thumbnails/041/166/062/small/ai-generated-hawk-high-quality-image-free-photo.jpg"/>
      <Card user ='Jane' para="This is Jane's card." img="https://st4.depositphotos.com/3516927/22348/i/450/depositphotos_223489912-stock-photo-girl-is-walking-a-dog.jpg"/>
      <Card user ='Bob' para="This is Bob's card." img ="https://m.media-amazon.com/images/I/91ZhFnr13LL.png"/>
      <Card user ='Alice' para="This is Alice's card." img ="https://img.freepik.com/free-photo/dramatic-sunset-rocky-ocean-cliffs-with-waves-crashing_9975-33096.jpg?semt=ais_rp_progressive&w=740&q=80"/>
      <Card user ='Charlie' para="This is Charlie's card." img ="https://img.freepik.com/free-photo/animal-lizard-nature-multi-colored-close-up-generative-ai_188544-9072.jpg?semt=ais_hybrid&w=740&q=80"/>
    </div>
  )
}

export default App
```

---

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
git clone https://github.com/Subhasish-MoveCore/Frontend-react-NextJS-Backend-NodeJS/tree/main/01_React_Frontend/04_Props

cd 04_Props

npm install

npm start
```

---

# 📚 Technologies Used

- React.js
- CSS

---

# 👨‍💻 Author

Made with ❤️ using React