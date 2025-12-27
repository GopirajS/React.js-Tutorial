## 1. React Basics


* [What is React?](#What_is_React)

* [Why is React used?](#Why_is_React_used)

* [What are the main features of React?](#main_features_of_React)

* [What is JSX?](#What_is_JSX)

* [Why JSX is faster than normal JavaScript?](#JSX_faster_than_normal)

* [What is Virtual DOM?](#What_is_Virtual_DOM)

* [Difference between Virtual DOM and Real DOM](#Virtual_DOM_and_Real_DOM)

* [How React works internally?](#How_React_works_internally)

* What is `create-react-app`?

---

## 2. Components


* [What is a component in React?](#What_is_a_Component_in_React)

* [Difference between Functional and Class components](#Functional_and_Class_components)

* [What is component composition?](#Component_Composition)

* Why Functional components are preferred now?

* What is component reusability?

* What is a pure component?

* What is memoized component?

---

## 3. Props


* [What are props?](#Props_in_React)

* [Are props mutable or immutable?](#Are_Props_Mutable_or_Immutable)

* [Difference between props and state](#Difference_between_props_and_state)

* [How to pass data from parent to child?](#pass_data_from_parent_to_child)

* [How to pass data from child to parent?](#pass_data_from_child_to_parent)

* [What is prop drilling. How to avoid prop drilling?](#What_is_prop_drilling)

---

## 4. State

* [What is state in React?](#What_is_State_in_React)

* [Why state is needed?](#Why_State_is_Needed_in_React)

* [How to update state correctly?](#Update_State_Correctly)

* [Why state updates are asynchronous?](#state_updates_are_asynchronous)

* [How to manage multiple states?](#Manage_Multiple_States_in_React)

---

## 5. Events


* [How event handling works in React?](#Event_Handling_Works)

* [Difference between React events and DOM events](#between_React_Events_and_DOM_Events)

* [What is synthetic event?](#What_is_a_Synthetic_Event)

* [How to pass arguments to event handlers?](#pass_arguments_to_event_handlers)

* [How to prevent default behavior in React?](#Prevent_Default_Behavior_in_React)

---


## 6. Conditional Rendering


* [What is conditional rendering?](#Conditional_Rendering)

* Different ways to do conditional rendering

* When to use ternary operator in JSX?

* When to use logical AND (`&&`)?

* How to render components conditionally?


---


<h1 style="text-align:center;" > React Basics</h1>

<span style="color:green;">================================================================ </span>

<h2 id="What_is_React" style="color:green">⚛️ What is React?</h2>

 **React** is a **JavaScript library** used to build **user interfaces**, mainly for **single-page applications**.

👉 It helps you create **reusable UI components**
👉 It updates the screen **fast** using a virtual DOM
👉 It is maintained by **Meta (Facebook)**

📌 In simple words:
**React makes building interactive and dynamic websites easier and faster.**



<span style="color:green;">================================================================ </span>

<h2 id="Why_is_React_used" style="color:green"> 🚀 Why is React used? </h2>


✅ **Fast performance** – Uses **Virtual DOM** to update only changed parts
✅ **Reusable components** – Write once, use anywhere
✅ **Easy to manage UI** – UI updates automatically when data changes
✅ **Large community** – Lots of support, libraries, and tools
✅ **Used by big companies** – Facebook, Instagram, Netflix, etc.

📌 In simple words:
**React is used to build fast, scalable, and interactive user interfaces easily.**


<span style="color:green;">================================================================ </span>

<h2 id="main_features_of_React" style="color:green"> ✨ Main features of React? </h2>


🔹 **Component-Based** – UI is built using small, reusable components
🔹 **Virtual DOM** – Improves performance by updating only necessary parts
🔹 **JSX** – Write HTML-like code inside JavaScript
🔹 **One-Way Data Binding** – Data flows in one direction, easy to debug
🔹 **Fast Rendering** – Quick UI updates
🔹 **Strong Community Support** – Backed by Meta and large ecosystem

📌 In simple words:
**React helps build fast, reusable, and easy-to-manage user interfaces.**


<span style="color:green;">================================================================ </span>

<h2 id="What_is_JSX" style="color:green"> What is JSX? </h2>


![Image](./Reference/Imgs/jsx.png)

![Image](./Reference/Imgs/compiler-part.svg)


🧠 **JSX (JavaScript XML)** is a **syntax extension** used in React that allows us to write **HTML-like code inside JavaScript**.

✅ Makes code **easy to read and write**
✅ Used to describe **UI structure**
✅ Compiled into normal JavaScript by Babel

📌 Example idea:
HTML + JavaScript together in one place

📌 In simple words:
**JSX lets you write UI code in a simple and readable way inside JavaScript.**


<span style="color:green;">================================================================ </span>

<h2 id="JSX_faster_than_normal" style="color:green"> ⚡ Why is JSX faster than normal JavaScript? </h2>


✅ **JSX is not actually faster by itself**
👉 JSX is converted into **JavaScript** by Babel

🚀 **Real reason for speed in React:**
🔹 **Virtual DOM** – Updates only changed elements
🔹 **Efficient diffing algorithm** – Finds minimum changes
🔹 **Optimized rendering** – Reduces direct DOM manipulation

📌 JSX helps React **understand UI structure clearly**, which makes updates **more efficient**.

📌 In simple words:
**JSX feels faster because React optimizes UI updates, not because JSX is faster than JavaScript.**


<span style="color:green;">================================================================ </span>

<h2 id="What_is_Virtual_DOM" style="color:green"> 🧠 What is Virtual DOM? </h2>

![Image](./Reference/Imgs/virtual_dom.png)

🌳 **Virtual DOM** is a **lightweight copy of the real DOM** used by React.

🔹 React first updates the **Virtual DOM**
🔹 It compares old and new Virtual DOM (**diffing**)
🔹 Finds only the **changed parts**
🔹 Updates **only those parts** in the real DOM

🚀 This makes React **fast and efficient**.

📌 In simple words:
**Virtual DOM helps React update the UI quickly by changing only what is needed.**



<span style="color:green;">================================================================ </span>

<h2 id="Virtual_DOM_and_Real_DOM" style="color:green"> 🆚 Difference between Virtual DOM and Real DOM </h2>


| 🔹 Virtual DOM                  | 🔸 Real DOM                    |
| ------------------------------- | ------------------------------ |
| 🧠 Lightweight copy of Real DOM | 🌐 Actual browser DOM          |
| ⚡ Faster updates                | 🐌 Slower updates              |
| 🔄 Updates only changed parts   | 🔁 Re-renders full DOM nodes   |
| 💻 Stored in memory             | 🌍 Directly affects browser UI |
| 🚀 Used by React                | 🧩 Used by normal JavaScript   |

📌 In simple words:
**Virtual DOM is faster because it updates only required changes, while Real DOM updates everything.**



<span style="color:green;">================================================================ </span>

<h2 id="How_React_works_internally" style="color:green"> ⚙️ How React works internally? </h2>

![Image](./Reference/Imgs/how_to_work_react.png)


🔹 **Component creation** – You write UI as components
🔹 **JSX compilation** – JSX is converted into JavaScript
🔹 **Virtual DOM creation** – React creates a Virtual DOM tree
🔹 **State / props change** – Data changes trigger re-render
🔹 **Diffing (Reconciliation)** – React compares old vs new Virtual DOM
🔹 **Efficient update** – Only changed parts update in Real DOM

🚀 This process makes React **fast and efficient**.

📌 In simple words:
**React updates only what changes instead of reloading the whole page.**


<span style="color:green;">================================================================ </span>


<h1 style="text-align:center;" > Components </h1>

![image](./Reference/Imgs/component.png)

<span style="color:green;">================================================================ </span>

<h2 id="What_is_a_Component_in_React" style="color:green"> 🧩 What is a Component in React? </h2>

📦 A **component** is a **small, reusable piece of UI** in React.

🔹 Components can be **buttons, forms, headers, pages**, etc.

🔹 Each component has its **own logic and UI**

🔹 Components can be **reused** multiple times

📌 Example idea:
One website = many small components

📌 In simple words:
**A component is a reusable building block of the React UI.**


<span style="color:green;">================================================================ </span>

<h2 id="Functional_and_Class_components" style="color:green"> 🆚 Difference between Functional and Class Components
 </h2>

![image](./Reference/Imgs/diff_function_class_component.png)


| 🔹 Functional Component                  | 🔸 Class Component            |
| ---------------------------------------  | ----------------------------- |
| 🧩 Simple JavaScript function            | 🏗️ JavaScript class           |
| ⚛️ Uses **Hooks** (useState, useEffect)  | 🔁 Uses **lifecycle methods** |
| ✍️ Less code, easy to read               | 📄 More code, complex         |
| 🚀 Better performance                    | 🐌 Slightly slower            |
| ✅ Most used in modern React             | ❌ Less used now              |

📌 In simple words:
**Functional components are simpler and preferred over class components in modern React.**



<span style="color:green;">================================================================ </span>

<h2 id="Component_Composition" style="color:green"> What is Component Composition? </h2>

![image](./Reference/Imgs/component_composition.png)

🧱 **Component composition** means **building components by combining other components**.

🔹 One component can **contain** other components
🔹 Helps create **clean, reusable, and flexible UI**
🔹 Avoids code duplication

📌 Example idea:
Page = Header + Sidebar + Content + Footer

📌 In simple words:
**Component composition is creating complex UI by joining small components together.**


```jsx
function Header() {
  return <h1>My Website</h1>;
}

function Footer() {
  return <p>© 2025</p>;
}

function Page() {
  return (
    <div>
      <Header />
      <p>Welcome to my website</p>
      <Footer />
    </div>
  );
}
```

🔹 **Header** and **Footer** are small components
🔹 **Page** component **uses (composes)** them together

📌 In simple words:
**Using components inside another component is called component composition.**


<span style="color:green;">================================================================ </span>

<h1 style="text-align:center;" > Props </h1>

![img](./Reference/Imgs/Props_usage.png)

<span style="color:green;">================================================================ </span>

<h2 id="Props_in_React" style="color:green"> What are Props in React? </h2>

📦 **Props (Properties)** are used to **pass data from one component to another**.

🔹 Data flows **from parent to child**
🔹 Props are **read-only** (cannot be changed by child)
🔹 Used to make components **dynamic and reusable**

📌 Example idea:
Same button, different text

📌 In simple words:
**Props are inputs that allow components to receive data from their parent.**

```jsx
function Welcome(props) {
  return <h1>Hello {props.name}</h1>;
}

function App() {
  return <Welcome name="React" />;
}
```

🔹 `name` is a **prop**
🔹 Data is passed from **App → Welcome**
🔹 `Welcome` uses the value but **cannot change it**

📌 **Query-style answer:**
**Props are used to pass data from parent component to child component.**


<span style="color:green;">================================================================ </span>

<h2 id="Are_Props_Mutable_or_Immutable" style="color:green"> 🧩 Are Props Mutable or Immutable?
 </h2>

❌ **Props are immutable** (cannot be changed by the child component)

🔹 Props are **read-only**
🔹 Only the **parent component** can change them

### ✅ Example

```jsx
function Child(props) {
  // ❌ Wrong (cannot change props)
  // props.name = "New Name";

  return <h1>Hello {props.name}</h1>;
}

function Parent() {
  return <Child name="React" />;
}
```

📌 Even if you try to change `props.name`, React **does not allow it**.

📌 In simple words:
**Props cannot be modified by the component that receives them.**


<span style="color:green;">================================================================ </span>

<h2 id="Difference_between_props_and_state" style="color:green"> Difference between props and state </h2>

![img](./Reference/Imgs/state_props.png)

🆚 **Difference between Props and State**

| 🔹 Props                                       | 🔸 State                             |
| ---------------------------------------------  | ------------------------------------ |
| 📦 Used to pass data to components             | 🧠 Used to manage component data     |
| ⬇️ Data comes from parent                      | 🔁 Data is managed inside component  |
| ❌ Immutable (read-only)                       | ✅ Mutable (can be changed)          |
| ⚛️ Used in both functional & class components  | ⚛️ Mostly used inside components     |
| 🔄 Changes come from parent                    | 🔄 Changes using setState / useState |

📌 **Query-style answer:**
**Props are used to pass data, while state is used to manage data inside a component.**


<span style="color:green;">================================================================ </span>

<h2 id="pass_data_from_parent_to_child" style="color:green"> How to pass data from parent to child? </h2>

🧩 **How to Pass Data from Parent to Child?**

👉 Data is passed using **props**

### ✅ Simple Example

```jsx
function Parent() {
  return <Child name="React" />;
}

function Child(props) {
  return <h2>Hello {props.name}</h2>;
}

```

🔹 `Parent` sends data using `name`
🔹 `Child` receives data using `props.name`

📌 **Query-style answer:**
**Data is passed from parent to child using props.**


<span style="color:green;">================================================================ </span>

<h2 id="pass_data_from_child_to_parent" style="color:green"> 🧩 How to Pass Data from Child to Parent? </h2>

👉 By using a **function passed as a prop**

### ✅ Simple Example

```jsx
function Child(props) {
  return (
    <button onClick={() => props.sendData("Hello Parent")}>
      Send Data
    </button>
  );
}

function Parent() {
  const getData = (msg) => {
    console.log(msg);
  };

  return <Child sendData={getData} />;
}
```

🔹 Parent passes a **function** to Child
🔹 Child **calls the function** with data
🔹 Parent receives the data

📌 **Query-style answer:**
**Data is passed from child to parent using callback functions via props.**


<span style="color:green;">================================================================ </span>

<h2 id="What_is_prop_drilling" style="color:green"> 🧩 What is Prop Drilling? and How to Avoid Prop Drilling? </h2>

![img](./Reference/Imgs/props_drilling.png)

📦 **Prop drilling** means **passing props through multiple components** even when intermediate components don’t need them.

🔹 Data goes: Parent → Child → Grandchild
🔹 Makes code **hard to manage**

### ❌ Prop Drilling Example

```jsx
function Parent() {
  return <Child name="React" />;
}

function Child({ name }) {
  return <GrandChild name={name} />;
}

function GrandChild({ name }) {
  return <h1>Hello {name}</h1>;
}
```

---

### 🚫 How to Avoid Prop Drilling?

👉 Use **Context API**

### ✅ Simple Context Example

```jsx
import { createContext, useContext } from "react";

const NameContext = createContext();

function Parent() {
  return (
    <NameContext.Provider value="React">
      <Child />
    </NameContext.Provider>
  );
}

function Child() {
  return <GrandChild />;
}

function GrandChild() {
  const name = useContext(NameContext);
  return <h1>Hello {name}</h1>;
}
```

📌 **Query-style answer:**
**Prop drilling is passing data through many components. It can be avoided using Context API.**


<h1 style="text-align:center;" > State </h1>

<span style="color:green;">================================================================ </span>

<h2 id="What_is_State_in_React" style="color:green"> 🧩 What is State in React?</h2>

![img](./Reference/Imgs/state_Libraries.png)

🧠 **State** is used to **store and manage data inside a component**.

🔹 State can **change over time**
🔹 When state changes, **UI re-renders**
🔹 State is **local to the component**

---

### ✅ Simple Example

```jsx
import { useState } from "react";

function Counter() {
  const [count, setCount] = useState(0);

  return (
    <button onClick={() => setCount(count + 1)}>
      Count: {count}
    </button>
  );
}
```

🔹 `count` is **state**
🔹 `setCount` updates the state
🔹 Button click updates UI

📌 **Query-style answer:**
**State is a component’s own data that controls its behavior and UI.**



<span style="color:green;">================================================================ </span>

<h2 id="Why_State_is_Needed_in_React" style="color:green"> 🧠 Why State is Needed in React?</h2>


✅ To **store dynamic data**
✅ To **update UI automatically** when data changes
✅ To **handle user interactions** (clicks, input, etc.)
✅ To **control component behavior**

📌 Example idea:
Counter value, form input, toggle button

📌 **Query-style answer:**
**State is needed to manage changing data and keep the UI in sync with user actions.**


<span style="color:green;">================================================================ </span>

<h2 id="Update_State_Correctly" style="color:green"> 🧩 How to Update State Correctly in React? </h2>


👉 Always use the **state update function** (`setState` / `setCount`)
❌ Never update state directly

---

### ❌ Wrong Way (Do NOT do this)

```jsx
count = count + 1;
```

🔹 React will **not re-render** the UI

---

### ✅ Correct Way

```jsx
setCount(count + 1);
```

---

### ✅ Best Practice (When using previous state)

```jsx
setCount(prevCount => prevCount + 1);
```

🔹 Ensures correct value
🔹 Avoids bugs in multiple updates

---

📌 **Query-style answer:**
**State should be updated using the provided setter function, not directly.**


<span style="color:green;">================================================================ </span>

<h2 id="state_updates_are_asynchronous" style="color:green">🧠 Why state updates are asynchronous? </h2>


🔹 React **does not update state immediately**
🔹 It **groups (batches) multiple state updates together**
🔹 This improves **performance** and avoids unnecessary re-renders

🚀 **What happens internally?**
✔ React schedules state updates
✔ Updates UI in one efficient render

---


### ⚠️ Problem Example

```jsx
import { useState } from "react";

function Counter() {
  const [count, setCount] = useState(0);

  const handleClick = () => {
    setCount(count + 1);
    setCount(count + 1);
    console.log(count);
  };

  return <button onClick={handleClick}>Count: {count}</button>;
}
```

🔹 You clicked once
🔹 You expect count = **2**
❌ But result is **1**

👉 **Why?**
React **batches** both updates and uses the **same old value** of `count`

---

### ✅ Correct Example (Best Practice)

```jsx
const handleClick = () => {
  setCount(prev => prev + 1);
  setCount(prev => prev + 1);
};
```

🔹 React uses **latest previous state**
🔹 Final count = **2** ✅

---

📌 **Query-style answer:**
**State updates are asynchronous because React batches updates for better performance, so we must use the previous state when updating multiple times.**



<span style="color:green;">================================================================ </span>

<h2 id="Manage_Multiple_States_in_React" style="color:green"> 🧠 How to Manage Multiple States in React? </h2>

### ✅ Method 1: Use Multiple `useState` Hooks

```jsx
const [name, setName] = useState("");
const [age, setAge] = useState(0);
```

🔹 Simple and clear
🔹 Best for **unrelated data**

---

### ✅ Method 2: Use Single State Object

```jsx
const [user, setUser] = useState({
  name: "",
  age: 0
});

setUser({ ...user, name: "React" });
```

🔹 Good for **related data**
🔹 Use spread operator to avoid mutation

---

### ✅ Method 3: Use `useReducer` (for complex state)

```jsx
const [state, dispatch] = useReducer(reducer, initialState);
```

🔹 Best for **large or complex logic**

---

📌 **Query-style answer:**
**Multiple states can be managed using multiple useState hooks, a single state object, or useReducer for complex cases.**

<span style="color:green;">================================================================ </span>

<h1 style="text-align:center;" > Events </h1>

<span style="color:green;">================================================================ </span>

![img](./Reference/Imgs/event_handling.png)

<h2 id="Event_Handling_Works" style="color:green"> How Event Handling Works in React? </h2>


🔹 React uses **synthetic events** (wrapper around browser events)
🔹 Events are written in **camelCase**
🔹 You pass a **function**, not a function call

---

### ✅ Simple Example

```jsx
function Button() {
  const handleClick = () => {
    alert("Button clicked");
  };

  return <button onClick={handleClick}>Click Me</button>;
}
```

🔹 `onClick` is a React event
🔹 `handleClick` runs when button is clicked

---

📌 **Query-style answer:**
**Event handling in React is done by passing functions to event handlers like onClick, onChange, etc.**


<span style="color:green;">================================================================ </span>

<h2 id="between_React_Events_and_DOM_Events" style="color:green"> 🆚 Difference between React Events and DOM Events </h2>


| 🔹 React Events                          | 🔸 DOM Events                           |
| ---------------------------------------- | --------------------------------------- |
| ⚛️ Uses **Synthetic Events**             | 🌐 Uses **Native browser events**       |
| 🧩 Works same across all browsers        | 🌍 Browser-dependent behavior           |
| 🖊️ Written in **camelCase** (`onClick`)  | ✍️ Written in **lowercase** (`onclick`) |
| 📌 Passed as function                    | 📎 Uses event listeners                 |
| 🚀 Better performance (event pooling)    | 🐌 No optimization                      |

📌 **Query-style answer:**
**React events are synthetic, cross-browser, and optimized, while DOM events are native browser events.**



<span style="color:green;">================================================================ </span>

<h2 id="What_is_a_Synthetic_Event" style="color:green"> 🧩 What is a Synthetic Event? </h2>

![img](./Reference/Imgs/synthetic_event.png)

⚛️ A **Synthetic Event** is a **wrapper around the browser’s native event** used by React.

🔹 Works the **same across all browsers**
🔹 Improves **performance**
🔹 Follows the same interface as native events

---

### ✅ Simple Example

```jsx
function InputBox() {
  const handleChange = (e) => {
    console.log(e.target.value);
  };

  return <input onChange={handleChange} />;
}
```

🔹 `e` is a **Synthetic Event**
🔹 React handles it internally

---

📌 **Query-style answer:**
**A synthetic event is React’s cross-browser wrapper around native DOM events.**



<span style="color:green;">================================================================ </span>

<h2 id="pass_arguments_to_event_handlers" style="color:green"> How to Pass Arguments to Event Handlers in React? </h2>

```jsx
// Event handler example
function Button() {

  // Function that receives an argument
  const handleClick = (msg) => {
    alert(msg); // shows the message
  };

  return (
    // Passing argument to the event handler using arrow function
    <button onClick={() => handleClick("Hello React")}>
      Click
    </button>
  );
}
```

📝 **Explanation (simple):**
🔹 `onClick` expects a **function**, not a function call
🔹 Arrow function `() =>` is used to **pass arguments**
🔹 `"Hello React"` is passed to `handleClick` when button is clicked

📌 **Query-style answer:**
**Arguments are passed to event handlers using arrow functions inside JSX.**


<span style="color:green;">================================================================ </span>

<h2 id="Prevent_Default_Behavior_in_React" style="color:green"> 🧩 How to Prevent Default Behavior in React? </h2>

👉 Use **`event.preventDefault()`**

---

### ✅ Simple Example

```jsx
function Form() {

  const handleSubmit = (e) => {
    e.preventDefault(); // prevents page refresh
    alert("Form submitted");
  };

  return (
    <form onSubmit={handleSubmit}>
      <button type="submit">Submit</button>
    </form>
  );
}
```

🔹 `e` is a **Synthetic Event**
🔹 `preventDefault()` stops browser default action

📌 **Query-style answer:**
**Default browser behavior in React is prevented using `event.preventDefault()`.**


<span style="color:green;">================================================================ </span>


<h1 style="text-align:center;" > Conditional Rendering </h1>


<span style="color:green;">================================================================ </span>

<h2 id="Conditional_Rendering" style="color:green"> 🧩 What is Conditional Rendering in React? </h2>

![img](./Reference/Imgs/conditional_rendering.png)

🔀 **Conditional rendering** means **showing UI based on a condition**.

🔹 UI changes depending on state or props
🔹 Similar to conditions in JavaScript (`if`, `&&`, `?:`)

---

### ✅ Simple Example

```jsx
function LoginStatus({ isLoggedIn }) {
  return (
    <h1>
      {isLoggedIn ? "Welcome User" : "Please Login"}
    </h1>
  );
}
```

🔹 If `isLoggedIn` is `true` → shows **Welcome User**
🔹 If `isLoggedIn` is `false` → shows **Please Login**

---

📌 **Query-style answer:**
**Conditional rendering is used to display different UI based on conditions.**


<span style="color:green;">================================================================ </span>
