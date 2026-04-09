<h2  style="color:green; text-align:center;">Infinite Scroll (like Instagram feed)</h2>

👉 Load more posts when user reaches bottom

## ✅ Simple Code (Easy Version)

```jsx
import React, { useEffect, useState } from "react";

function InfiniteScroll() {
  const [data, setData] = useState([]);
  const [page, setPage] = useState(1);

  // API call
  const fetchData = async () => {
    const res = await fetch(
      `https://jsonplaceholder.typicode.com/posts?_limit=5&_page=${page}`
    );
    const result = await res.json();

    // append data
    setData((prev) => [...prev, ...result]);
  };

  // call API when page changes
  useEffect(() => {
    fetchData();
  }, [page]);

  // scroll event
  useEffect(() => {
    const handleScroll = () => {
      if (
        window.innerHeight + window.scrollY >=
        document.body.offsetHeight - 10
      ) {
        setPage((prev) => prev + 1);
      }
    };

    window.addEventListener("scroll", handleScroll);

    return () => window.removeEventListener("scroll", handleScroll);
  }, []);

  return (
    <div>
      <h3>Instagram Feed</h3>

      {data.map((item) => (
        <p key={item.id}>{item.title}</p>
      ))}

      <p>Loading...</p>
    </div>
  );
}

export default InfiniteScroll;
```


<h2  style="color:green; text-align:center;">Modal open/close with outside click</h2>

👉 Features:

* Click button → open modal
* Click outside modal → close modal

---

## ✅ Simple Code Example

```jsx id="m2k9lp"
import React, { useState, useRef, useEffect } from "react";

function ModalExample() {
  const [open, setOpen] = useState(false);
  const modalRef = useRef(null);

  // handle outside click
  useEffect(() => {
    const handleClickOutside = (e) => {
      if (modalRef.current && !modalRef.current.contains(e.target)) {
        setOpen(false);
      }
    };

    if (open) {
      document.addEventListener("mousedown", handleClickOutside);
    }

    return () => {
      document.removeEventListener("mousedown", handleClickOutside);
    };
  }, [open]);

  return (
    <div>
      <button onClick={() => setOpen(true)}>Open Modal</button>

      {open && (
        <div style={overlayStyle}>
          <div ref={modalRef} style={modalStyle}>
            <h2>Modal Content</h2>
            <p>This is a modal</p>
            <button onClick={() => setOpen(false)}>Close</button>
          </div>
        </div>
      )}
    </div>
  );
}

// simple styles
const overlayStyle = {
  position: "fixed",
  top: 0,
  left: 0,
  width: "100%",
  height: "100%",
  background: "rgba(0,0,0,0.5)",
  display: "flex",
  justifyContent: "center",
  alignItems: "center"
};

const modalStyle = {
  background: "#fff",
  padding: "20px",
  borderRadius: "8px"
};

export default ModalExample;
```

---

## ✅ Key Points (Interview Ready)

* `useState` → control open/close
* `useRef` → reference modal box
* `contains()` → detect outside click
* Add/remove event listener in `useEffect`

---



<h2  style="color:green; text-align:center;">Tabs switching without page reload</h2>

👉 When user clicks tab:

* Switch content instantly
* No page refresh

---

## ✅ Simple Code Example

```jsx id="t9v2qp"
import React, { useState } from "react";

function TabsExample() {
  const [activeTab, setActiveTab] = useState("tab1");

  return (
    <div>
      <h2>Tabs Example</h2>

      {/* Tabs */}
      <div>
        <button onClick={() => setActiveTab("tab1")}>Tab 1</button>
        <button onClick={() => setActiveTab("tab2")}>Tab 2</button>
        <button onClick={() => setActiveTab("tab3")}>Tab 3</button>
      </div>

      {/* Content */}
      <div style={{ marginTop: "20px" }}>
        {activeTab === "tab1" && <p>Content for Tab 1</p>}
        {activeTab === "tab2" && <p>Content for Tab 2</p>}
        {activeTab === "tab3" && <p>Content for Tab 3</p>}
      </div>
    </div>
  );
}

export default TabsExample;
```

---

## ✅ Key Points (Interview Ready)

* Use `useState` → track active tab
* No routing → no reload
* Conditional rendering → show content
* Fast UI switching

---

## ✅ Short Interview Answer

👉 “I use state to track the active tab and conditionally render content based on it, so switching happens instantly without page reload.”


<h2  style="color:green; text-align:center;">Dark mode toggle with localStorage</h2>

👉 Features:
- Toggle between light / dark mode  
- Save user preference in `localStorage`  
- Load saved theme on refresh  

---

## ✅ Simple Code Example

```jsx id="dm8k2p"
import React, { useState, useEffect } from "react";

function DarkMode() {
  const [dark, setDark] = useState(false);

  // load saved theme
  useEffect(() => {
    const savedTheme = localStorage.getItem("theme");
    if (savedTheme === "dark") {
      setDark(true);
    }
  }, []);

  // save theme
  useEffect(() => {
    if (dark) {
      document.body.style.background = "#222";
      document.body.style.color = "#fff";
      localStorage.setItem("theme", "dark");
    } else {
      document.body.style.background = "#fff";
      document.body.style.color = "#000";
      localStorage.setItem("theme", "light");
    }
  }, [dark]);

  return (
    <div>
      <h2>Dark Mode Toggle</h2>

      <button onClick={() => setDark(!dark)}>
        {dark ? "Light Mode" : "Dark Mode"}
      </button>
    </div>
  );
}

export default DarkMode;
```

---

## ✅ Key Points (Interview Ready)
- `useState` → track theme  
- `localStorage` → persist user choice  
- `useEffect` → load & apply theme  
- Toggle UI using state  

---

## ✅ Short Interview Answer  
👉 “I store the theme in localStorage and use state to control UI. On load, I read the saved value and apply the theme using useEffect.”


<h2  style="color:green; text-align:center;">Pagination with API</h2>

👉 Features:

* Load data page by page
* Click **Next / Previous**
* Fetch data from API

---

## ✅ Simple Code Example

```jsx id="pg4k9x"
import React, { useEffect, useState } from "react";

function PaginationExample() {
  const [data, setData] = useState([]);
  const [page, setPage] = useState(1);

  const limit = 5;

  // fetch API
  const fetchData = async () => {
    const res = await fetch(
      `https://jsonplaceholder.typicode.com/posts?_limit=${limit}&_page=${page}`
    );
    const result = await res.json();
    setData(result);
  };

  useEffect(() => {
    fetchData();
  }, [page]);

  return (
    <div>
      <h2>Pagination Example</h2>

      {/* Data */}
      {data.map((item) => (
        <p key={item.id}>{item.title}</p>
      ))}

      {/* Buttons */}
      <button onClick={() => setPage(page - 1)} disabled={page === 1}>
        Prev
      </button>

      <span> Page {page} </span>

      <button onClick={() => setPage(page + 1)}>
        Next
      </button>
    </div>
  );
}

export default PaginationExample;
```

---

## ✅ Key Points (Interview Ready)

* `page` → controls API data
* `_page` & `_limit` → pagination params
* `useEffect` → fetch when page changes
* Disable **Prev** on first page

---

## ✅ Short Interview Answer

👉 “I manage the page state and pass it to the API. When the page changes, I fetch new data using useEffect and display it.”

---

<h2  style="color:green; text-align:center;">Prevent multiple API calls</h2>

👉 Problem:

* User clicks button multiple times OR component re-renders
* API gets called many times ❌

👉 Solution:

* Control API call using a flag / loading state

---

## ✅ Simple Code Example (Using `loading`)

```jsx id="api7kq"
import React, { useState } from "react";

function PreventMultipleCalls() {
  const [loading, setLoading] = useState(false);
  const [data, setData] = useState(null);

  const fetchData = async () => {
    if (loading) return; // prevent multiple calls

    setLoading(true);

    try {
      const res = await fetch("https://jsonplaceholder.typicode.com/posts/1");
      const result = await res.json();
      setData(result);
    } catch (err) {
      console.log(err);
    }

    setLoading(false);
  };

  return (
    <div>
      <h2>API Call</h2>

      <button onClick={fetchData} disabled={loading}>
        {loading ? "Loading..." : "Fetch Data"}
      </button>

      {data && <p>{data.title}</p>}
    </div>
  );
}

export default PreventMultipleCalls;
```

---

## ✅ Key Points (Interview Ready)

* Use `loading` state as a **lock**
* `if (loading) return` → stop duplicate calls
* Disable button while loading
* Reset loading after API completes

---

## ✅ Short Interview Answer

👉 “I use a loading state to block duplicate API calls. If a request is already in progress, I prevent triggering another call.”


<h2  style="color:green; text-align:center;">How to manage global state in React?</h2>

👉 Global state = data shared across components (e.g., user, theme, cart)

## ✅ 1. Simple Way → Context API (Most asked ⭐)

### 🔹 Step 1: Create Context

```jsx id="ctx1ab"
import React, { createContext, useState } from "react";

export const AppContext = createContext();

export function AppProvider({ children }) {
  const [user, setUser] = useState("Gopi");

  return (
    <AppContext.Provider value={{ user, setUser }}>
      {children}
    </AppContext.Provider>
  );
}
```

---

### 🔹 Step 2: Wrap App

```jsx id="ctx2cd"
import React from "react";
import ReactDOM from "react-dom";
import App from "./App";
import { AppProvider } from "./AppContext";

ReactDOM.render(
  <AppProvider>
    <App />
  </AppProvider>,
  document.getElementById("root")
);
```

---

### 🔹 Step 3: Use in Any Component

```jsx id="ctx3ef"
import React, { useContext } from "react";
import { AppContext } from "./AppContext";

function Profile() {
  const { user, setUser } = useContext(AppContext);

  return (
    <div>
      <h2>{user}</h2>
      <button onClick={() => setUser("Raj")}>Change Name</button>
    </div>
  );
}

export default Profile;
```

---

## ✅ Key Points (Interview Ready)

* `createContext()` → create global store
* `Provider` → wrap app
* `useContext()` → access data anywhere
* Avoid prop drilling

---

## ✅ Short Interview Answer

👉 “For simple global state, I use React Context API. I create a context, wrap the app with a provider, and access state using useContext in any component.”

---

## 🔥 Bonus (Advanced Options)

👉 For large apps:

* **Redux Toolkit** → best for complex state
* **Zustand** → simple & lightweight
* **Recoil** → modern state management

---

## 🚀 One-Line Tip (Impress Interviewer)

👉 “I prefer Context for small apps and Redux Toolkit or Zustand for scalable applications.”

---


<h2  style="color:green; text-align:center;">QUESTION</h2>
<h2  style="color:green; text-align:center;">QUESTION</h2>
<h2  style="color:green; text-align:center;">QUESTION</h2>
<h2  style="color:green; text-align:center;">QUESTION</h2>
<h2  style="color:green; text-align:center;">QUESTION</h2>
<h2  style="color:green; text-align:center;">QUESTION</h2>
<h2  style="color:green; text-align:center;">QUESTION</h2>
<h2  style="color:green; text-align:center;">QUESTION</h2>