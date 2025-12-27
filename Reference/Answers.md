<h1 style="text-align:center;" > Routing (React Router) </h1>


<span style="color:green;">================================================================ </span>

<h2 id="What_is_React_Router" style="color:green"> 🧭 What is React Router? </h2>


⚛️ **React Router** is a **library** used for **navigation and routing** in React **single-page applications (SPA)**.

🔹 Allows multiple pages **without page reload**
🔹 Changes URL and UI **dynamically**
🔹 Most commonly used: **React Router DOM**

---

## ✅ Simple Example

### 1️⃣ Setup Routes

```jsx
import { BrowserRouter, Routes, Route } from "react-router-dom";

function App() {
  return (
    <BrowserRouter>
      <Routes>
        <Route path="/" element={<Home />} />
        <Route path="/about" element={<About />} />
      </Routes>
    </BrowserRouter>
  );
}
```

---

### 2️⃣ Components

```jsx
function Home() {
  return <h1>Home Page</h1>;
}

function About() {
  return <h1>About Page</h1>;
}
```

---

### 3️⃣ Navigation Link

```jsx
import { Link } from "react-router-dom";

<Link to="/about">Go to About</Link>
```

🔹 `Link` prevents page reload
🔹 URL changes, component updates

---

📌 **Query-style answer:**
**React Router is used to handle navigation and routing in React single-page applications.**



<span style="color:green;">================================================================ </span>

<h2 id="BrowserRouter_and_HashRouter" style="color:green"> 🆚 Difference between `BrowserRouter` and `HashRouter` </h2>


| 🔹 BrowserRouter               | 🔸 HashRouter               |
| ------------------------------ | --------------------------- |
| Uses **HTML5 history API**     | Uses **URL hash (#)**       |
| Clean URLs (`/about`)          | Hash URLs (`/#/about`)      |
| Needs **server configuration** | No server config needed     |
| Better for **production apps** | Good for **static hosting** |
| SEO friendly                   | Less SEO friendly           |

---

### ✅ Example URLs

🔹 **BrowserRouter**

```
https://example.com/about
```

🔹 **HashRouter**

```
https://example.com/#/about
```

---

📌 **Query-style answer:**
**BrowserRouter gives clean URLs but needs server setup, while HashRouter works without server configuration using hash-based URLs.**





<span style="color:green;">================================================================ </span>

<h2 id="demo_test" style="color:green"> Question_name </h2>






<span style="color:green;">================================================================ </span>

<h2 id="demo_test" style="color:green"> Question_name </h2>
