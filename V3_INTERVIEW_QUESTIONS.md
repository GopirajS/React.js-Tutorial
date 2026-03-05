* [What is React and why is it used?](#What_is_React)
* [What are the main features of React?](#main_features_of_React)
* [What is JSX?](#What_is_JSX)
* [What is a component in React?](#component_in_React)
* [What is the difference between functional and class components?](#Functional_and_Class_Components)
* [What are props in React?](#props_in_React)
* [What is state in React?](#state_in_React)
* [Difference between state and props?](#between_State_and_Props)
* [What is the virtual DOM?](#Virtual_DOM)
* [How does React update the DOM?](#React_update_the_DOM)
* [What is reconciliation in React?](#Reconciliation)
* [What are hooks in React?](#Hooks_in_React)
* [What is `useState`?](#useState)
* [What is `useEffect`?](#useEffect)
* [Difference between `useEffect` and `useLayoutEffect`?](#useEffect_useLayoutEffect)
* [What is `useContext`?](#useContext)
* [What is `useRef`?](#useRef)
* [What is `useMemo`?](#useMemo)
* [What is `useCallback`?](#useCallback)
* [What are controlled components?](#Controlled_Components)
* [What are uncontrolled components?](#Uncontrolled_Components)
* [What is lifting state up?](#Lifting_State_Up)
* [What is prop drilling?](#Prop_Drilling)
* [How to avoid prop drilling?](#avoid_prop_drilling)
* [What is context API?](#Context_API)
* [What is React Fragment?](#Fragment)
* [What are keys in React?](#Keys_in_React)
* [Why are keys important in lists?](#keys_important)
* [What is conditional rendering?](#Conditional_Rendering)
* [What is lazy loading in React?](#Lazy_Loading)
* [What is `React.memo`?](#React.memo)
* [What is code splitting?](#Code_Splitting)
* [What is higher-order component (HOC)?](#HOC)
* [What is a pure component?](#Pure_Component)
* [What are lifecycle methods?](#Lifecycle_Method)
* [What is the difference between `useEffect` and lifecycle methods?](#useEffect_Lifecycle_Methods)
* [What is error boundary?](#Error_Boundary)
* [What is suspense in React?](#Suspense)
* [What is server-side rendering (SSR)?](#SSR)
* [What is client-side rendering (CSR)?](#CSR)
* [What is hydration in React?](#Hydration)
* [What is React Router?](#React_Router)
* [What is `useParams`?](#useParams)
* [What is `useNavigate`?](#useNavigate)
* [What is `useLocation`?](#useLocation)
* [What is Redux?](#Redux)
* [Difference between Redux and Context API?](#Redux_Context_API)
* [What is a reducer?](#Reducer)
* [What is an action in Redux?](#Action_in_Redux)
* [What is middleware in Redux?](#Middleware_in_Redux)
* [What is thunk?](#Thunk_in_Redux)
* [What is two-way data binding?](#Two-Way)
* [What is one-way data binding?](#One-Way)
* [What is synthetic event in React?](#Synthetic_Event)
* [What is batching in React?](#Batching)
* [What is concurrent rendering in React?](#Concurrent_Rendering)
* [What is strict mode in React?](#Strict_Mode)
* [Why is `key` not accessible as a prop?](#key)
* [What is portal in React?](#Portal)
* [What are custom hooks?](#Custom_Hooks)
* [Rules of hooks?](#Rules_of_Hooks)
* [What happens if you break the rules of hooks?](#break_Hooks)
* [What is dependency array in `useEffect`?](#Dependency_Array)
* [What is cleanup function in `useEffect`?](#Cleanup_Function)
* [Difference between `useMemo` and `useCallback`?](#useMemo_useCallback)
* [What is memoization?](#Memoization)
* [What is render prop pattern?](#Render_Prop_Pattern)
* [What is compound component pattern?](#Compound_Component_Pattern)
* [What is controlled vs uncontrolled form validation?](#Controlled_Uncontrolled)
* [What is CORS?](#CORS)
* [How do you secure React application?](#secure_React)
* [What is environment variable in React?](#Environment_Variable)
* [What is Webpack?](#Webpack)
* [What is Babel?](#Babel)
* [What is Vite?](#Vite)
* [Difference between Vite and Create React App?](#Vite_Create_React_App)
* [What is tree shaking?](#Tree_Shaking)
* [What is bundling?](#Bundling)
* [What is minification?](#Minification)
* [What is polyfill?](#Polyfill)
* [What is Progressive Web App (PWA)?](#PWA)
* What is service worker?
* What is SEO issue in React apps?
* How to improve performance in React?
* What is lazy() in React?
* What is dynamic import?
* What is suspense fallback?
* What is hydration mismatch?
* What is React Fiber?
* What is time slicing in React?
* What is useTransition?
* What is useDeferredValue?
* What is useId?
* What is useImperativeHandle?
* What is useSyncExternalStore?
* What is error boundary lifecycle?
* What is PureComponent?
* Difference between PureComponent and React.memo?
* What is shallow comparison?
* What is deep comparison?
* What is state normalization?
* What is Flux architecture?
* What is micro frontend?


<hr style="border: 2px solid green;">

<h2 id="What_is_React" style="color:green; text-align:center;">📘 What is React and why is it used?</h2>

**What is React?**
 - React is a JavaScript library
 - It is used to make user interfaces (UI)
 - It is used to build websites and web apps
 - Made by Facebook

**Why is React used?**
 - Makes fast websites
 - Easy to build big apps
 - Reusable components
 - Updates page without reloading
 - Saves time for developers


<hr style="border: 2px solid green;">

<h2 id="main_features_of_React" style="color:green; text-align:center;">What are the main features of React?</h2>


🔹 **Component Based** - App is made using small parts called components

🔹 **Fast Performance**- Uses Virtual DOM to update only needed parts

🔹 **Reusable Code**- Same component can be used many times

🔹 **JSX Support**- Write HTML inside JavaScript

🔹 **One-Way Data Flow**- Data moves in one direction (parent to child)

🔹 **Easy to Learn**- Simple rules and clear structure

🔹 **Strong Community**- Many users and help available



<hr style="border: 2px solid green;">

<h2 id="What_is_JSX" style="color:green; text-align:center;">What is JSX?</h2>

 - JSX means **JavaScript XML**
 - It is used in React to write HTML inside JavaScript
 - It looks like HTML but works with JavaScript
 - It makes code easy to read and write


<hr style="border: 2px solid green;">

<h2 id="component_in_React" style="color:green; text-align:center;">What is a component in React?</h2>


 - A component is a small part of a webpage
 - It is like a block or piece of the UI
 - Each component does one small job
 - Components can be reused many times

🧩 **Examples of components:**
 - Button
 - Header
 - Footer
 - Form

✅ **Why components are used?**
 - Easy to manage
 - Easy to reuse
 - Makes code clean



<hr style="border: 2px solid green;">

<h2 id="Functional_and_Class_Components" style="color:green; text-align:center;">Difference between Functional and Class Components</h2>


🔹 **Functional Component**
 - Written as a simple function
 - Uses **Hooks** (like `useState`, `useEffect`)
 - Less code
 - Easy to read
 - Faster and modern way

🔹 **Class Component**
 - Written using `class` keyword
 - Uses **this.state** and **this.setState()**
 - More code
 - Harder to read
 - Old method

⚖️ **Main Differences:**

🧩 **Functional Component**
 - Simple function
 - Uses Hooks
 - Short code
 - Easy to learn

🏛️ **Class Component**
 - Uses class
 - Uses lifecycle methods
 - Long code
 - Hard to learn

<hr style="border: 2px solid green;">

<h2 id="props_in_React" style="color:green; text-align:center;">What are props in React?</h2>


- Props means **properties**
- Props are used to pass data from one component to another
- Data is sent from **parent to child**
- Props are **read-only** (cannot be changed)

📦 **Example idea:**
- Parent sends name to child using props

✅ **Why props are used?**
- Share data between components
- Make components reusable
- Keep code clean


<hr style="border: 2px solid green;">

<h2 id="state_in_React" style="color:green; text-align:center;">What is state in React?</h2>

- State is used to store data in a component
- State can change during program running
- When state changes, UI also updates
- Each component can have its own state

📦 **Example idea:**
- Counter number
- Input box value
- Button click status

✅ **Why state is used?**
- To save changing data
- To control what is shown on screen

🧠 **In short:**
👉 State is used to store and change data inside a React component.


<hr style="border: 2px solid green;">

<h2 id="between_State_and_Props" style="color:green; text-align:center;">Difference between State and Props</h2>


🔹 **Props**
- Props are used to send data from parent to child
- Props are **read-only** (cannot be changed)
- Props come from outside the component
- Used to share data

🔹 **State**
- State is used to store data inside the component
- State **can be changed**
- State is managed inside the component
- Used for changing data



<hr style="border: 2px solid green;">

<h2 id="Virtual_DOM" style="color:green; text-align:center;">What is the Virtual DOM?</h2>


- Virtual DOM is a **copy of real DOM**
- It is kept in memory (not on screen)
- React uses it to check changes
- It updates only the changed part of the page

⚙️ **How it works (simple):**
- Change happens in data
- Virtual DOM checks what changed
- Only that part is updated on real page

🧠 **In short:**
👉 Virtual DOM is a fast copy of real DOM that helps React update pages quickly.





<hr style="border: 2px solid green;">

<h2 id="React_update_the_DOM" style="color:green; text-align:center;">How does React update the DOM?</h2>

- React uses **Virtual DOM**
- First, React updates the Virtual DOM
- Then it compares old and new Virtual DOM
- It finds only the changed parts
- Only those parts are updated in real DOM

⚙️ **Simple steps:**
- Data changes
- Virtual DOM changes
- React checks difference
- Real DOM updates only needed part


🧠 **In short:**
👉 React updates only the changed part of the page, not the whole page.


<hr style="border: 2px solid green;">

<h2 id="Reconciliation" style="color:green; text-align:center;">What is Reconciliation in React?</h2>



- Reconciliation means **finding changes**
- React compares **old Virtual DOM** with **new Virtual DOM**
- It checks what is changed in the UI
- Then React updates only the changed parts

⚙️ **Simple idea:**
- Old screen = saved
- New screen = created
- React compares both
- Updates only different part

🧠 **In short:**
👉 Reconciliation is the process of comparing old and new Virtual DOM to update the page correctly.


<hr style="border: 2px solid green;">

<h2 id="Hooks_in_React" style="color:green; text-align:center;">What are Hooks in React?</h2>


- Hooks are special functions in React
- Hooks let us use state and other features in functional components
- Hooks make code simple and clean
- Hooks work only in functional components

🪝 **Common Hooks:**
- `useState` – for state
- `useEffect` – for side effects
- `useContext` – for shared data

🧠 **In short:**
👉 Hooks help us use React features inside functional components.


<hr style="border: 2px solid green;">

<h2 id="useState" style="color:green; text-align:center;">What is `useState`?</h2>


- `useState` is a React Hook
- It is used to store and change data in a component
- It works in functional components
- When state changes, screen updates

📦 **Used for:**
- Counter value
- Input box text
- Toggle (on/off)


🧠 **In short:**
👉 `useState` is used to create and change state in a React component.


<hr style="border: 2px solid green;">

<h2 id="useEffect" style="color:green; text-align:center;">What is `useEffect`?</h2>

- `useEffect` is a React Hook
- It is used to run code after the page loads
- It is used for side work (extra work)
- It runs when component renders

🛠️ **Used for:**
- Getting data from API
- Setting timers
- Updating title
- Listening to events
  

<hr style="border: 2px solid green;">

<h2 id="useEffect_useLayoutEffect" style="color:green; text-align:center;">Difference between `useEffect` and `useLayoutEffect`</h2>




🔹 **`useEffect`**
- Runs **after** screen is painted (shown)
- Does not block screen drawing
- Used for normal work
- Safe and most used

🛠️ Used for:
✔ API calls
✔ Event listeners
✔ Timers

---

🔹 **`useLayoutEffect`**
- Runs **before** screen is painted
- Blocks screen until work is done
- Used for UI size and position work
- Less used

🛠️ Used for:
✔ Measure height/width
✔ Fix layout before showing

---

🧠 **In short:**
- `useEffect` = after screen shows
- `useLayoutEffect` = before screen shows



<hr style="border: 2px solid green;">

<h2 id="useContext" style="color:green; text-align:center;">What is `useContext`?</h2>

- `useContext` is a React Hook
- It is used to share data between many components
- It avoids passing props again and again
- It works with Context API

📦 **Used for:**
- User login data
- Theme (dark/light)
- Language setting

⚙️ **Simple idea:**
- One place stores data
- Many components can use it
- No need prop drilling


🧠 **In short:**
- `useContext` is used to get shared data from Context in React.


<hr style="border: 2px solid green;">

<h2 id="useRef" style="color:green; text-align:center;">What is `useRef`?</h2>


- `useRef` is a React Hook
- It is used to store a value without re-rendering the page
- It is also used to access HTML elements directly
- Value stays same between renders

**Used for:**

* Access input box
* Focus on input field
* Store previous value
* Work with DOM elements

**Simple idea:**

* `useRef` = store value
* Change value
* UI does not re-render

🧠 **In short:**
`useRef` is used to access elements and store values without changing the UI.


<hr style="border: 2px solid green;">

<h2 id="useMemo" style="color:green; text-align:center;">What is `useMemo`?</h2>

- `useMemo` is a React Hook
- It is used to save (remember) a calculated value
- It runs calculation only when needed
- It helps make app faster

**Used for:**

* Heavy calculations
* Avoid repeat calculation
* Improve performance

**Simple idea:**

* Do calculation once
* Save result
* Use it again

🧠 **In short:**
`useMemo` is used to remember a value so React does not calculate it again and again.



<hr style="border: 2px solid green;">

<h2 id="useCallback" style="color:green; text-align:center;">What is `useCallback`?</h2>


- `useCallback` is a React Hook
- It is used to save (remember) a function
- It does not create the function again and again
- It helps make app faster

**Used for:**

* Passing function to child component
* Avoid re-creating same function
* Improve performance

**Simple idea:**

* Create function once
* Save it
* Reuse it

🧠 **In short:**
`useCallback` is used to remember a function so React does not create it again and again.



<hr style="border: 2px solid green;">

<h2 id="Controlled_Components" style="color:green; text-align:center;">What are Controlled Components?</h2>


- Controlled component means form input is controlled by React
- Input value is stored in **state**
- React decides what is shown in input box
- Changes are handled using `onChange`


**How it works (simple):**

* User types in input
* Value goes to state
* State updates input value

**Why used:**

* Easy to control form data
* Easy validation
* Easy to handle submit

🧠 **In short:**
Controlled components are form inputs whose value is controlled by React state.



<hr style="border: 2px solid green;">

<h2 id="Uncontrolled_Components" style="color:green; text-align:center;">What are Uncontrolled Components?</h2>

🔹 Uncontrolled component means form input is controlled by **DOM**, not React state
🔹 Value is taken using **ref**
🔹 React does not control the input value
🔹 Data is read only when needed (like on submit)


**How it works (simple):**

* User types in input
* Browser stores value
* React reads value using ref


🧠 **In short:**
Uncontrolled components are form inputs whose value is handled by the browser, not by React state.


<hr style="border: 2px solid green;">

<h2 id="Lifting_State_Up" style="color:green; text-align:center;">What is Lifting State Up?</h2>

- Lifting state up means moving state to a **parent component**
- It is done when two or more child components need same data
- Parent keeps the state
- Parent sends data to children using props

**Simple idea:**

* Two children need same data
* Put state in parent
* Share with both children

**Why used:**

* Data is same for many components
* Easy to manage data
* Avoid duplicate state

🧠 **In short:**
Lifting state up means keeping shared data in the parent component instead of child components.


<hr style="border: 2px solid green;">

<h2 id="Prop_Drilling" style="color:green; text-align:center;">What is Prop Drilling?</h2>

- Prop drilling means passing data through levels of components
- Data goes from **Parent → Child → Grandchild**
- The **Child** does not need the data
- Child only passes it to **Grandchild**

**Simple example:**

* Parent has data (user name)
* Parent sends it to Child
* Child sends it to Grandchild
* Only Grandchild uses the data

This is called **prop drilling** ❌

**Why it is a problem:**

* Extra props passing
* Child carries data it does not use
* Code becomes hard to read
* Hard to maintain


🧠 **In short:**
Prop drilling = **Parent → Child → Grandchild** passing data, even when middle child does not need it.


<hr style="border: 2px solid green;">

<h2 id="avoid_prop_drilling" style="color:green; text-align:center;">How to avoid prop drilling?</h2>

🔹 Do not pass data through many components
🔹 Use **Context API** to share data directly
🔹 Use `useContext` hook to get data
🔹 Keep common data in one place
🔹 Use state manager if app is big (like Redux)

**Simple ways:**

* Use Context API
* Use `useContext`
* Lift state to common parent
* Avoid deep Parent → Child → Grandchild passing

🧠 **In short:**
To avoid prop drilling, use Context API or shared state instead of passing props again and again.



<hr style="border: 2px solid green;">

<h2 id="Context_API" style="color:green; text-align:center;">What is Context API?</h2>


🔹 Context API is a React feature
🔹 It is used to share data with many components
🔹 It avoids prop drilling
🔹 Data can be used without passing props step by step


<hr style="border: 2px solid green;">

<h2 id="Fragment" style="color:green; text-align:center;">What is React Fragment?</h2>


🔹 React Fragment is used to group many elements
🔹 It does not add extra HTML tag to the page
🔹 It helps return multiple elements from a component
🔹 It keeps the DOM clean

**Used for:**

* Wrap multiple elements
* Avoid extra `div`
* Clean UI structure

**Simple idea:**

* Group items
* No extra tag in browser

🧠 **In short:**
React Fragment lets you return many elements without adding extra HTML element to the page.


<hr style="border: 2px solid green;">

<h2 id="Keys_in_React" style="color:green; text-align:center;">What are Keys in React?</h2>


🔹 Keys are special values used in lists
🔹 They help React identify each item
🔹 Each list item should have a unique key
🔹 Keys help React update list correctly

**Used for:**

* List of items
* Table rows
* Menu items

**Why keys are important:**

* Helps React find which item changed
* Makes updates fast
* Avoids wrong UI update

🧠 **In short:**
Keys are unique values given to list items so React can update them correctly.


<hr style="border: 2px solid green;">

<h2 id="keys_important" style="color:green; text-align:center;">Why are keys important in lists?</h2>


🔹 Keys help React identify each list item
🔹 They tell React which item is new, changed, or removed
🔹 They help React update only the needed items
🔹 They keep UI correct when list changes

**Without keys:**

* React gets confused
* Wrong item may update
* Performance becomes slow

**With keys:**

* Fast update
* Correct item update
* Better performance

🧠 **In short:**
Keys are important because they help React update list items correctly and fast.


<hr style="border: 2px solid green;">

<h2 id="Conditional_Rendering" style="color:green; text-align:center;">What is Conditional Rendering?</h2>


- Conditional rendering means showing content based on a condition
- React shows different UI when condition is true or false
- It works like `if` or `else` in JavaScript

**Used for:**

* Show login or logout button
* Show loader or data

🧠 **In short:**
Conditional rendering means showing different content based on a condition.

<hr style="border: 2px solid green;">

<h2 id="Lazy_Loading" style="color:green; text-align:center;">What is Lazy Loading in React?</h2>


🔹 Lazy loading means loading something **only when needed**
🔹 React loads components later, not at first
🔹 It makes the app start faster
🔹 It saves internet data

**Used for:**

* Large components
* Pages in routing
* Images or heavy files

**Simple idea:**

* Open page
* Load only needed part
* Load other parts later

🧠 **In short:**
Lazy loading means loading components only when they are needed, not all at once.


<hr style="border: 2px solid green;">

<h2 id="React.memo" style="color:green; text-align:center;">What is `React.memo`?</h2>

🔹 `React.memo` is used to remember a component
🔹 It stops the component from re-rendering if props do not change
🔹 It helps improve performance
🔹 Used with functional components

**Used for:**

* Child components
* Heavy UI components
* Avoid extra re-render

**Simple idea:**

* Props same → no re-render
* Props changed → re-render

🧠 **In short:**
`React.memo` prevents a component from re-rendering when its props have not changed.


<hr style="border: 2px solid green;">

<h2 id="React.memo" style="color:green; text-align:center;">What is `React.memo`?</h2>

🔹 `React.memo` is used to remember a component
🔹 It stops the component from re-rendering if props do not change
🔹 It helps improve performance
🔹 Used with functional components

**Used for:**

* Child components
* Heavy UI components
* Avoid extra re-render


🧠 **In short:**
`React.memo` prevents a component from re-rendering when its props have not changed.


<hr style="border: 2px solid green;">

<h2 id="Code_Splitting" style="color:green; text-align:center;">What is Code Splitting?</h2>

🔹 Code splitting means breaking big code into small parts
🔹 App loads only needed code first
🔹 Other code loads later when needed
🔹 It makes app load faster

### ✅ Without Code Splitting (all loaded at once)

```jsx
import Home from "./Home";
import About from "./About";
```

👉 Both pages load together ❌

---

### ✅ With Code Splitting (load when needed)

```jsx
import React, { lazy, Suspense } from "react";

const Home = lazy(() => import("./Home"));
const About = lazy(() => import("./About"));

function App() {
  return (
    <Suspense fallback={<div>Loading...</div>}>
      <Home />
      <About />
    </Suspense>
  );
}

export default App;
```

**Used for:**

* Large applications
* Different pages
* Heavy components

**Simple idea:**

* Load home page code
* Load other page code when user opens it

🧠 **In short:**
Code splitting means loading only required code first and rest later to make app faster.


<hr style="border: 2px solid green;">

<h2 id="HOC" style="color:green; text-align:center;">What is Higher-Order Component (HOC)?</h2>


🔹 HOC is a function
🔹 It takes a component as input
🔹 It returns a new component
🔹 It is used to reuse logic

**Simple idea:**

* Component goes in
* New component comes out

**Used for:**

* Authentication
* Logging
* Data fetching
* Permission check

🧠 **In short:**
HOC is a function that takes a component and returns a new component with extra features.

---

### 🎯 Normal Component

```jsx
function MyComponent() {
  return <h2>Hello User</h2>;
}
```

---

### 🎁 HOC Function

```jsx
function withWelcome(Component) {
  return function () {
    return (
      <div>
        <h1>Welcome!</h1>
        <Component />
      </div>
    );
  };
}
```

---

### 🔁 Create New Component using HOC

```jsx
const NewComponent = withWelcome(MyComponent);
```

---

### 🧾 Use New Component

```jsx
function App() {
  return <NewComponent />;
}
```

---

### 🧠 How it works (simple)

* `withWelcome` takes `MyComponent`
* Adds extra UI (`Welcome!`)
* Returns new component
* New component is used in App

---

🧠 **In short:**
HOC = wrap a component to add extra behavior.



<hr style="border: 2px solid green;">

<h2 id="Pure_Component" style="color:green; text-align:center;">What is a Pure Component?</h2>


🔹 Pure component is a component that avoids unnecessary re-render
🔹 It re-renders only when **props or state change**
🔹 It compares old and new values before re-render
🔹 It improves performance

**Used for:**

* Same data UI
* Large lists
* Heavy components

**Simple idea:**

* Data same → no re-render
* Data changed → re-render

🧠 **In short:**
A pure component re-renders only when its props or state change, making the app faster.


<hr style="border: 2px solid green;">

<h2 id="Lifecycle_Method" style="color:green; text-align:center;">What are Lifecycle Method?</h2>


🔹 Lifecycle methods are special functions in React
🔹 They are used in **class components**
🔹 They run at different times in a component’s life
🔹 They control what happens when component:

* is created
* is updated
* is removed

**Main lifecycle methods:**

* `componentDidMount` – runs when component is shown
* `componentDidUpdate` – runs when data changes
* `componentWillUnmount` – runs when component is removed

**Used for:**

* API calls
* Updating data
* Cleaning timers or events

🧠 **In short:**
Lifecycle methods are functions that run at different stages of a component’s life in class components.


<hr style="border: 2px solid green;">

<h2 id="useEffect_Lifecycle_Methods" style="color:green; text-align:center;">Difference between `useEffect` and Lifecycle Methods</h2>

🔹 **`useEffect`**

* Used in **functional components**
* One hook can do many jobs
* Replaces lifecycle methods
* Easy and short code

**Used for:**

* Data fetching
* Timer
* Event listener

---

🔹 **Lifecycle Methods**

* Used in **class components**
* Different methods for different work
* More code
* Old way

**Examples:**

* `componentDidMount`
* `componentDidUpdate`
* `componentWillUnmount`

---

⚖️ **Main Difference**

**`useEffect`**

* For function components
* One place for side work
* Modern way

**Lifecycle Methods**

* For class components
* Many methods
* Old way

---

🧠 **In short:**
`useEffect` is the new way in functional components.
Lifecycle methods are the old way in class components.


<hr style="border: 2px solid green;">

<h2 id="Error_Boundary" style="color:green; text-align:center;">What is Error Boundary?</h2>


🔹 Error Boundary is a special React component
🔹 It is used to catch JavaScript errors in UI
🔹 It prevents the whole app from crashing
🔹 It shows a fallback UI when error happens

**Used for:**

* Catch component errors
* Show error message
* Protect main app

**Simple idea:**

* Error happens in child
* Error Boundary catches it
* Shows “Something went wrong” instead of breaking app

🧠 **In short:**
Error Boundary is used to catch errors in components and show a safe UI instead of crashing the app.


<hr style="border: 2px solid green;">

<h2 id="Suspense" style="color:green; text-align:center;">What is Suspense in React?</h2>

🔹 Suspense is used to show a loading message
🔹 It waits while something is loading
🔹 It is used with lazy loading
🔹 It improves user experience

**Used for:**

* Lazy loaded components
* Data loading
* Images or heavy files

**How it works (simple):**

* Component is loading
* Suspense shows “Loading…”
* When ready, component shows

🧠 **In short:**
Suspense shows a fallback UI (like “Loading…”) while something is loading in React.


<hr style="border: 2px solid green;">

<h2 id="SSR" style="color:green; text-align:center;">What is Server-Side Rendering (SSR)?</h2>

🔹 SSR means page is created on the **server**
🔹 Server sends ready HTML to browser
🔹 Page shows fast to user
🔹 Good for SEO

**How it works (simple):**

* User requests page
* Server builds HTML
* Server sends HTML
* Browser shows page

**Used for:**

* Better SEO
* Faster first load
* Public websites

🧠 **In short:**
SSR means the server creates the page and sends ready HTML to the browser.


<hr style="border: 2px solid green;">

<h2 id="CSR" style="color:green; text-align:center;">What is Client-Side Rendering (CSR)?</h2>


🔹 CSR means page is created in the **browser**
🔹 Server sends only empty HTML and JavaScript
🔹 Browser builds the page using JavaScript
🔹 Page loads after JavaScript runs

**How it works (simple):**

* User opens page
* Server sends JS file
* Browser runs JS
* Page is created on screen

**Used for:**

* Single Page Applications (SPA)
* Dashboards
* Web apps

🧠 **In short:**
CSR means the browser creates the page using JavaScript, not the server.


<hr style="border: 2px solid green;">

<h2 id="Hydration" style="color:green; text-align:center;">What is Hydration in React?</h2>


🔹 Hydration happens after **Server-Side Rendering (SSR)**
🔹 Server sends ready HTML to browser
🔹 React adds JavaScript to that HTML
🔹 Page becomes interactive (buttons work, events work)

**Simple idea:**

* Server makes page
* Browser shows page
* React connects JavaScript to it

**Why hydration is needed:**

* To make page clickable
* To make app interactive
* To use React features on server HTML

🧠 **In short:**
Hydration means React adds JavaScript to server-made HTML so the page can work like a normal React app.




<hr style="border: 2px solid green;">

<h2 id="React_Router" style="color:green; text-align:center;">What is React Router?</h2>

- React Router is a library for navigation
- It is used to move between pages in a React app
- It helps create Single Page Application (SPA)
- It changes page without full reload

**Simple idea:**

* Click link
* URL changes
* New component shows
* Page does not reload

🧠 **In short:**
React Router is used to change pages in a React app without reloading the whole page.


<hr style="border: 2px solid green;">

<h2 id="useParams" style="color:green; text-align:center;">What is `useParams`?</h2>

- `useParams` is a React Router hook
- It is used to get values from the URL
- It reads **dynamic route parameters**
- It is used inside a component

**Used for:**

* Get user id or product id from URL
* Show data based on URL

**Simple idea:**

* URL = `/user/10`
* `useParams` gets `10`

🧠 **In short:**
`useParams` is used to read values from the URL in React Router.


<hr style="border: 2px solid green;">

<h2 id="useNavigate" style="color:green; text-align:center;">What is `useNavigate`?</h2>

🔹 `useNavigate` is a React Router hook
🔹 It is used to change page using code
🔹 It helps move from one route to another
🔹 No page reload happens

**Used for:**

* Go to another page
* Redirect after login
* Go back to previous page

**Simple idea:**

* Button click
* Call `useNavigate`
* Page changes

🧠 **In short:**
`useNavigate` is used to move to another page using JavaScript in React Router.


<hr style="border: 2px solid green;">

<h2 id="useLocation" style="color:green; text-align:center;">What is `useLocation`?</h2>

🔹 `useLocation` is a React Router hook
🔹 It is used to get current URL information
🔹 It tells which page is open now
🔹 It gives path and query data

**Used for:**

* Check current route
* Highlight active menu
* Read query string

**Simple idea:**

* URL = `/profile`
* `useLocation` gives `/profile`

🧠 **In short:**
`useLocation` is used to get current URL details in React Router.


<hr style="border: 2px solid green;">

<h2 id="Redux" style="color:green; text-align:center;">What is Redux?</h2>

🔹 Redux is a **state management library**
🔹 It stores application data in one place
🔹 That place is called **Store**
🔹 Many components can use the same data

**Used for:**

* User login data
* Shopping cart
* App settings
* Large application state

**Main parts of Redux:**

* **Store** – keeps all data
* **Action** – tells what to do
* **Reducer** – updates the data

🧠 **In short:**
Redux stores application data in one central place so many components can use it.

---

### Action

```javascript
const increment = {
  type: "INCREMENT"
};
```

---

### Reducer

```javascript
function counter(state = 0, action) {
  if (action.type === "INCREMENT") {
    return state + 1;
  }
  return state;
}
```

---

### Store

```javascript
import { createStore } from "redux";

const store = createStore(counter);
```

---

### Use in Component (simple idea)

```javascript
store.dispatch({ type: "INCREMENT" });
```

---

### 🧠 How it works (simple)

* Component sends **Action**
* **Reducer** changes data
* **Store** saves new data
* UI updates


<hr style="border: 2px solid green;">

<h2 id="Redux_Context_API" style="color:green; text-align:center;">Difference between Redux and Context API</h2>

🔹 **Redux**

* External library
* Used for large applications
* Has store, action, reducer
* More setup and code
* Powerful state management

🔹 **Context API**

* Built inside React
* Used for small or medium apps
* Simple to use
* Less setup
* Good for sharing simple data

---

⚖️ **Main Difference**

**Redux**

* External library
* Complex state handling
* Best for large apps

**Context API**

* Built-in React feature
* Simple state sharing
* Best for small apps

---

🧠 **In short:**
Redux is a powerful state manager for large apps.
Context API is a simple way to share data in React.


<hr style="border: 2px solid green;">

<h2 id="Reducer" style="color:green; text-align:center;">What is a Reducer?</h2>


🔹 A reducer is a **function**
🔹 It is used to **update the state**
🔹 It receives **current state and action**
🔹 It returns a **new state**

**Reducer has three things:**

* Current state
* Action
* New state

**Simple flow:**

* Action is sent
* Reducer checks action type
* Reducer updates state
* New state is returned

**Simple example:**

```javascript
function counter(state = 0, action) {
  if (action.type === "INCREMENT") {
    return state + 1;
  }
  return state;
}
```

**Used for:**

* Counter update
* Cart items update
* User data update

🧠 **In short:**
A reducer is a function that changes the state based on an action.



<hr style="border: 2px solid green;">

<h2 id="Action_in_Redux" style="color:green; text-align:center;">What is an Action in Redux?</h2>

🔹 An action is a **simple JavaScript object**
🔹 It tells Redux **what happened**
🔹 It is used to request a state change
🔹 It must have a **type**

**Action contains:**

* `type` – what action happened
* `payload` (optional) – extra data

**Simple example:**

```javascript
const action = {
  type: "INCREMENT"
};
```

**Example with data:**

```javascript
const action = {
  type: "ADD_ITEM",
  payload: "Apple"
};
```

**Used for:**

* Increase counter
* Add item to cart
* Login user

🧠 **In short:**
An action is an object that tells Redux what change should happen in the state.


<hr style="border: 2px solid green;">

<h2 id="Middleware_in_Redux" style="color:green; text-align:center;">What is Middleware in Redux?</h2>


🔹 Middleware is a function in Redux
🔹 It runs **between action and reducer**
🔹 It can change, delay, or handle actions
🔹 It is used for extra work

**Used for:**

* API calls
* Logging actions
* Handling async work

**Simple flow:**

* Action is sent
* Middleware runs
* Then reducer updates state

**Common middleware:**

* `redux-thunk`
* `redux-logger`

🧠 **In short:**
Middleware is a function that runs between dispatching an action and the reducer to handle extra work.


<hr style="border: 2px solid green;">

<h2 id="Thunk_in_Redux" style="color:green; text-align:center;">What is Thunk in Redux?</h2>

🔹 Thunk is a **middleware** for Redux
🔹 It allows you to write **functions** as actions instead of plain objects
🔹 Used to handle **asynchronous tasks** (like API calls)
🔹 Helps dispatch actions **after async work is done**

**Used for:**

* Fetching data from API
* Delayed actions
* Async updates

**Simple idea:**

* Normal action: `{ type: "INCREMENT" }`
* Thunk action: function that can run async code, then dispatch action

---

### ✅ Simple Example

```javascript id="lqed01"
// Thunk function (async action)
const fetchData = () => {
  return async (dispatch) => {
    const data = await fetch("https://jsonplaceholder.typicode.com/todos/1")
      .then(res => res.json());
    dispatch({ type: "SET_DATA", payload: data });
  };
};
```

**How it works:**

* Call `fetchData()`
* Middleware (thunk) runs it
* Waits for API
* Dispatches action with data

---

🧠 **In short:**
Thunk lets Redux handle async actions by allowing **functions as actions** instead of plain objects.


<hr style="border: 2px solid green;">

<h2 id="Two-Way" style="color:green; text-align:center;">What is Two-Way Data Binding?</h2>


🔹 Two-way data binding means **UI and data are connected**
🔹 When **data changes**, UI updates automatically
🔹 When **UI changes**, data updates automatically

**Used for:**

* Forms
* Input boxes
* Checkboxes

**Simple idea:**

* User types in input → state updates
* State changes → input shows updated value

**Example:**

```jsx
const [name, setName] = React.useState("");
<input value={name} onChange={(e) => setName(e.target.value)} />
```

🧠 **In short:**
Two-way data binding keeps **data and UI always in sync**.


<hr style="border: 2px solid green;">

<h2 id="One-Way" style="color:green; text-align:center;">What is One-Way Data Binding?</h2>


🔹 One-way data binding means **data flows in one direction only**
🔹 From **state/props → UI**
🔹 UI cannot directly change the data

**Used for:**

* Displaying data
* Passing props to child
* Read-only components

**Simple idea:**

* State = `"Hello"`
* UI shows `"Hello"`
* UI cannot change state directly

**Example:**

```jsx id="cb1qf8"
const [message, setMessage] = React.useState("Hello");
<p>{message}</p>
```

🧠 **In short:**
One-way data binding means **data flows from state to UI only**, not the other way.


<hr style="border: 2px solid green;">

<h2 id="Synthetic_Event" style="color:green; text-align:center;">What is Synthetic Event in React?</h2>

- Synthetic Event is a **wrapper around browser event**
- React creates it to make events work the same in all browsers
- It follows the same interface as normal DOM events
- It improves performance

**Simple idea:**

* Browser event happens
* React wraps it as **Synthetic Event**
* React handles it in a consistent way

**Example:**

```jsx
function App() {
  function handleClick(event) {
    console.log(event);
  }

  return <button onClick={handleClick}>Click</button>;
}
```

🧠 **In short:**
Synthetic Event is a React wrapper around the browser event to make events work the same in all browsers.


<hr style="border: 2px solid green;">

<h2 id="Batching" style="color:green; text-align:center;">Batching in React</h2>

- **Batching** means React **groups multiple state updates together** and does **only one re-render**.
- This helps React **improve performance**.
- Instead of updating the UI many times, React **updates it once**.

---

📌 **Example idea**

If we write:

```javascript
setCount(count + 1);
setName("John");
```

React will:

 - group both updates
 - update the component **one time**

---

🎯 **Why batching is useful**

🔹 Reduces unnecessary re-render
🔹 Makes React **faster**
🔹 Improves **application performance**

---

📖 **Short Definition**

👉 **Batching is the process of combining multiple state updates into a single re-render.**


<hr style="border: 2px solid green;">

<h2 id="Concurrent_Rendering" style="color:green; text-align:center;">What is Concurrent Rendering in React?</h2>


- Concurrent rendering is a React feature
- It lets React work on many tasks at the same time
- React can pause and continue rendering when needed
- It keeps the UI smooth and responsive

**Used for:**

* Large UI updates
* Heavy components
* Better user experience

**Simple idea:**

* React starts rendering
* If important work comes → React pauses
* React finishes important work first
* Then continues other work

🧠 **In short:**
Concurrent rendering lets React handle multiple rendering tasks smoothly without blocking the UI.


<hr style="border: 2px solid green;">

<h2 id="Strict_Mode" style="color:green; text-align:center;">What is Strict Mode in React?</h2>

🔹 Strict Mode is a tool in React
🔹 It helps find problems in the code
🔹 It works only in **development mode**
🔹 It does not affect production

**What it does:**

* Shows warnings for bad code
* Finds unsafe lifecycle methods
* Detects unexpected side effects

**Simple idea:**

* React checks your code
* Shows warnings
* Helps improve code quality

**Example:**

```jsx id="g5kzq3"
import React from "react";

function App() {
  return <h1>Hello</h1>;
}

export default function Main() {
  return (
    <React.StrictMode>
      <App />
    </React.StrictMode>
  );
}
```

🧠 **In short:**
Strict Mode helps developers find problems and warnings in React code during development.


<hr style="border: 2px solid green;">

<h2 id="key" style="color:green; text-align:center;">key</h2>

📘 **Why is `key` not accessible as a prop?**

🔹 `key` is a special attribute in React
🔹 It is used **only by React** to identify list items
🔹 React uses it during **reconciliation (DOM update)**
🔹 Because of this, `key` is **not passed to the component as a prop**

**Simple idea:**

* React uses `key` internally
* Component cannot read `key`

**Example:**

```jsx
<MyComponent key="1" name="John" />
```

Inside `MyComponent`:

* `props.name` → available ✅
* `props.key` → not available ❌

**If you need the value inside component:**

Pass it with another prop.

```jsx
<MyComponent key="1" id="1" name="John" />
```

Now inside component:

* `props.id` → available ✅

🧠 **In short:**
`key` is used internally by React to track elements, so it is not accessible as a normal prop inside components.


<hr style="border: 2px solid green;">

<h2 id="Portal" style="color:green; text-align:center;">What is Portal in React?</h2>

* Portal is a React feature
* It allows a component to render outside the parent DOM
* It is created using `ReactDOM.createPortal()`
* Useful when UI needs to appear above other elements

**Why is Portal used in React?**

* To create modal popups
* To show dialog boxes
* To display tooltips
* To show notifications
* Helps place UI elements outside the normal component structure

**Simple Example:**

```javascript
import ReactDOM from "react-dom";

function Modal({ children }) {
  return ReactDOM.createPortal(
    <div className="modal">{children}</div>,
    document.getElementById("modal-root")
  );
}
```


<hr style="border: 2px solid green;">

<h2 id="Custom_Hooks" style="color:green; text-align:center;">What are Custom Hooks in React?</h2>


* Custom Hook is a **user-created hook**
* It is used to **reuse logic in different components**
* Custom Hooks always **start with `use`**
* Helps make code **clean and reusable**

**Simple Example**

```javascript
function useCounter() {
  const [count, setCount] = React.useState(0);

  function increment() {
    setCount(count + 1);
  }

  return { count, increment };
}
```

**Using Custom Hook**

```javascript
function App() {
  const { count, increment } = useCounter();

  return (
    <div>
      <p>{count}</p>
      <button onClick={increment}>Increase</button>
    </div>
  );
}
```

**Why Custom Hooks are used?**

* Reuse logic
* Reduce duplicate code
* Make components cleaner
* Easy to maintain code


<hr style="border: 2px solid green;">

<h2 id="Rules_of_Hooks" style="color:green; text-align:center;">Rules of Hooks in React</h2>


**Rule 1: Only call Hooks at the top level**

* Do not call Hooks inside loops
* Do not call Hooks inside conditions
* Always call Hooks at the top of the component

**Rule 2: Only call Hooks inside React functions**

* Use Hooks inside **React functional components**
* Or inside **custom hooks**

**Rule 3: Hooks must start with `use`**

* Example: `useState`, `useEffect`
* Custom hooks also start with `use`

**Simple Example**

```javascript
function Example() {
  const [count, setCount] = useState(0); // correct

  return <p>{count}</p>;
}
```

**Short Interview Answer**

* Hooks must be called **at the top level**
* Hooks must be used **only in React functions**
* Hooks **must start with `use`**


<hr style="border: 2px solid green;">

<h2 id="break_Hooks" style="color:green; text-align:center;">What happens if you break the Rules of Hooks?</h2>


* ⚠️ React will show an **error or warning**
* ❌ Hooks may **not work correctly**
* 🔄 Component state may become **incorrect**
* 🐞 Application may have **bugs or unexpected behavior**
* 🚫 React cannot track the **correct order of Hooks**

**Simple Example (Wrong)**

```javascript
if (condition) {
  const [count, setCount] = useState(0); // ❌ Wrong
}
```

**Reason:**
React Hooks must always be called **in the same order** every time the component renders.


<hr style="border: 2px solid green;">

<h2 id="Dependency_Array" style="color:green; text-align:center;">What is Dependency Array in `useEffect`?</h2>


* Dependency array is the **second argument** of `useEffect`
* It tells React **when the effect should run**
* React checks the values in the array
* If a value changes, the effect runs again

**Example**

```javascript
useEffect(() => {
  console.log("Count changed");
}, [count]);
```

* The effect runs **only when `count` changes**

**Types of Dependency Array**

* 🔁 **No array** → runs on **every render**
* 📌 **Empty array `[]`** → runs **only once (on mount)**
* 🔄 **With values `[count]`** → runs when **that value changes**


<hr style="border: 2px solid green;">

<h2 id="Cleanup_Function" style="color:green; text-align:center;">What is Cleanup Function in `useEffect`?</h2>

* Cleanup function is a **function returned inside `useEffect`**
* It is used to **clean or remove side effects**
* It runs **before the component unmounts**
* It also runs **before the effect runs again**

**Example**

```javascript
useEffect(() => {
  const timer = setInterval(() => {
    console.log("Running...");
  }, 1000);

  return () => {
    clearInterval(timer); // cleanup
  };
}, []);
```

**Why Cleanup Function is used?**

* 🧹 Stop timers
* 🔌 Remove event listeners
* 📡 Close subscriptions
* 🚫 Prevent memory leaks


<hr style="border: 2px solid green;">

<h2 id="useMemo_useCallback" style="color:green; text-align:center;">Difference between `useMemo` and `useCallback`</h2>


**What is `useMemo`?**

* `useMemo` is a React Hook
* It **memoizes a value**
* Used to **store the result of a calculation**
* Runs only when dependencies change

**Example**

```javascript
const total = useMemo(() => {
  return price * quantity;
}, [price, quantity]);
```

**What is `useCallback`?**

* `useCallback` is a React Hook
* It **memoizes a function**
* Prevents the function from being recreated on every render
* Runs only when dependencies change

**Example**

```javascript
const handleClick = useCallback(() => {
  console.log("Button clicked");
}, []);
```

**Main Difference**

* `useMemo` → **returns a value**
* `useCallback` → **returns a function**



<hr style="border: 2px solid green;">

<h2 id="Memoization" style="color:green; text-align:center;">What is Memoization?</h2>


* Memoization is a **performance optimization technique**
* It **stores the result of a function**
* If the same input comes again, it **returns the stored result**
* It **avoids recalculating the same value**

**Why Memoization is used?**

* 🚀 Improves performance
* 🔁 Avoids repeated calculations
* ⚡ Makes applications faster

**Simple Example**

```javascript
const result = useMemo(() => {
  return num * 2;
}, [num]);
```

* React **remembers the result**
* It recalculates **only when `num` changes**.


<hr style="border: 2px solid green;">

<h2 id="Render_Prop_Pattern" style="color:green; text-align:center;">What is Render Prop Pattern in React?</h2>

* Render Prop is a **technique to share code between components**
* A component **passes a function as a prop**
* That function **returns JSX to render**
* It helps **reuse logic**

**Simple Example**

```javascript
function DataProvider(props) {
  const data = "Hello";

  return props.render(data);
}
```

**Using the Component**

```javascript
<DataProvider render={(data) => <h1>{data}</h1>} />
```

**Why Render Prop is used?**

* ♻️ Reuse component logic
* 🧩 Share data between components
* 🧹 Makes code more flexible


<hr style="border: 2px solid green;">

<h2 id="Compound_Component_Pattern" style="color:green; text-align:center;">What is Compound Component Pattern in React?</h2>

* Compound Component Pattern is a **design pattern in React**
* Multiple components **work together as one component**
* Parent component **controls the state**
* Child components **share that state**

**Example**

```javascript
function Tabs({ children }) {
  return <div>{children}</div>;
}

function Tab() {
  return <button>Tab</button>;
}

Tabs.Tab = Tab;
```

**Using the Component**

```javascript
<Tabs>
  <Tabs.Tab />
  <Tabs.Tab />
</Tabs>
```

**Why Compound Component Pattern is used?**

* 🧩 Group related components
* 🔁 Reuse components easily
* 🧹 Keep code organized



<hr style="border: 2px solid green;">

<h2 id="Controlled_Uncontrolled" style="color:green; text-align:center;">What is controlled vs uncontrolled form validation?</h2>

**Controlled Form Validation**

* Form data is **controlled by React state**
* Input value is stored in **`useState`**
* Validation is done **inside React code**
* React updates the input value

**Example**

```javascript
const [name, setName] = useState("");

<input 
  value={name} 
  onChange={(e) => setName(e.target.value)} 
/>
```

**Uncontrolled Form Validation**

* Form data is **controlled by the DOM**
* React uses **`ref` to access the value**
* Input value is **not stored in React state**
* Validation is done **using DOM values**

**Example**

```javascript
const inputRef = useRef();

<input ref={inputRef} />
```

**Main Difference**

* Controlled → **React controls form data (state)**
* Uncontrolled → **DOM controls form data (ref)**



<hr style="border: 2px solid green;">

<h2 id="CORS" style="color:green; text-align:center;">What is CORS?</h2>


* CORS stands for **Cross-Origin Resource Sharing**
* It is a **security feature in browsers**
* It controls **requests between different domains**
* It prevents **unauthorized access to resources**

**Example**

* Frontend: `https://example.com`
* API: `https://api.example.com`

If the frontend tries to access the API, the **server must allow CORS**.

**Why CORS is used?**

* 🔒 Improves security
* 🌐 Controls cross-domain requests
* 🛡️ Prevents unauthorized access


<hr style="border: 2px solid green;">

<h2 id="secure_React" style="color:green; text-align:center;">How do you secure a React application?</h2>


- 🔐 **Use HTTPS**  
  Protects data between client and server.

- 🛡️ **Prevent XSS attacks**  
  Avoid using `dangerouslySetInnerHTML`.

- 🔑 **Use authentication**  
  Use **JWT or OAuth** for user login.

- 🚫 **Do not store sensitive data in localStorage**  
  Store tokens securely.

- 🔒 **Protect API endpoints**  
  Use authentication and authorization.

- 📦 **Keep dependencies updated**  
  Update React and npm packages regularly.

- 🧹 **Validate user input**  
  Check user data before sending to server.


<hr style="border: 2px solid green;">

<h2 id="Environment_Variable" style="color:green; text-align:center;">What is Environment Variable in React?</h2>

* Environment variables are **special variables used to store configuration values**
* They help store **API URLs, keys, and settings**
* Values can change **for different environments** (development, production)
* In React, variables must start with **`REACT_APP_`**

**Example**

`.env` file

```
REACT_APP_API_URL=https://api.example.com
```

**Using in React**

```javascript
const apiUrl = process.env.REACT_APP_API_URL;
```

**Why Environment Variables are used?**

* 🔒 Hide configuration values
* ⚙️ Manage different environments
* 🧹 Keep code clean


<hr style="border: 2px solid green;">

<h2 id="Webpack" style="color:green; text-align:center;">What is Webpack?</h2>


* Webpack is a **module bundler**
* It **combines multiple files into one bundle**
* Used in **modern JavaScript applications**
* Helps manage **JS, CSS, images, and other files**

**Example**

* Combines files like:

  * `index.js`
  * `style.css`
  * images

➡️ Into a **single bundled file**

**Why Webpack is used?**

* 📦 Bundles project files
* ⚡ Improves performance
* 🧹 Organizes project dependencies
* 🚀 Makes apps faster to load


<hr style="border: 2px solid green;">

<h2 id="Babel" style="color:green; text-align:center;">What is Babel?</h2>

* Babel is a **JavaScript compiler**
* It **converts modern JavaScript (ES6+) into older JavaScript (ES5)**
* Helps code run in **older browsers**
* Commonly used in **React applications**

**Example**

**Modern JavaScript (ES6)**

```javascript
const add = (a, b) => a + b;
```

**Converted by Babel (ES5)**

```javascript
var add = function(a, b) {
  return a + b;
};
```

**Why Babel is used?**

* 🌐 Supports old browsers
* ⚙️ Converts modern JS syntax
* 🚀 Helps run React and modern JavaScript code


<hr style="border: 2px solid green;">

<h2 id="Vite" style="color:green; text-align:center;">What is Vite?</h2>


* Vite is a **modern frontend build tool**
* It is used to **create and run web applications**
* It provides **very fast development server**
* Commonly used for **React, Vue, and other frameworks**

**Example**

Create a React app using Vite:

```bash
npm create vite@latest my-app
```

**Why Vite is used?**

* ⚡ Very fast startup
* 🔄 Fast hot reload (HMR)
* 📦 Simple configuration
* 🚀 Faster than traditional build tools like Webpack


<hr style="border: 2px solid green;">

<h2 id="Vite_Create_React_App" style="color:green; text-align:center;">Difference between Vite and Create React App</h2>


**What is Vite?**

* ⚡ Very fast development server
* 🚀 Faster project startup
* 🔄 Fast Hot Module Replacement (HMR)
* 🧹 Simple and lightweight configuration

**What is Create React App (CRA)?**

* 📦 Official React setup tool
* 🛠 Uses Webpack internally
* ⏳ Slower startup compared to Vite
* ⚙️ More configuration behind the scenes

**Main Differences**

* ⚡ **Vite** → Faster build and reload
* 🐢 **CRA** → Slower development server
* 🧹 **Vite** → Lightweight and modern
* 📦 **CRA** → Older but stable setup tool


<hr style="border: 2px solid green;">

<h2 id="Tree_Shaking" style="color:green; text-align:center;">What is Tree Shaking?</h2>


* Tree Shaking is a **process to remove unused code**
* It helps **reduce the final bundle size**
* Used in build tools like **Webpack and Vite**
* Keeps only the **code that is actually used**

**Example**

```javascript
export function add(a, b) {
  return a + b;
}

export function multiply(a, b) {
  return a * b;
}
```

If the app only uses **`add()`**, the **`multiply()`** function will be removed during build.

**Why Tree Shaking is used?**

* 📦 Smaller bundle size
* ⚡ Faster website loading
* 🧹 Removes unused code


<hr style="border: 2px solid green;">

<h2 id="Bundling" style="color:green; text-align:center;">What is Bundling?</h2>

* Bundling is the **process of combining multiple files into one file**
* It combines **JavaScript, CSS, and other files**
* Helps reduce the **number of requests to the server**
* Done by tools like **Webpack, Vite, and Parcel**

**Example**

Files in project:

* `app.js`
* `utils.js`
* `style.css`

➡️ After bundling → **one bundled file (bundle.js)**

**Why Bundling is used?**

* 📦 Combines project files
* ⚡ Improves website loading speed
* 🧹 Organizes application code


<hr style="border: 2px solid green;">

<h2 id="Minification" style="color:green; text-align:center;">What is Minification?</h2>


* Minification is the **process of removing unnecessary characters from code**
* It removes **spaces, comments, and line breaks**
* It makes the **file size smaller**
* Helps the website **load faster**

**Example**

**Before Minification**

```javascript
function add(a, b) {
  return a + b;
}
```

**After Minification**

```javascript
function add(a,b){return a+b;}
```

**Why Minification is used?**

* 📦 Reduces file size
* ⚡ Improves website speed
* 🚀 Faster loading time



<hr style="border: 2px solid green;">

<h2 id="Polyfill" style="color:green; text-align:center;">What is Polyfill?</h2>

* Polyfill is **JavaScript code that adds support for modern features in older browsers**
* It helps old browsers **run new JavaScript features**
* Used when a browser **does not support a feature**

**Example**

`Array.includes()` may not work in older browsers.

Polyfill adds support for it.

```javascript
if (!Array.prototype.includes) {
  Array.prototype.includes = function(value) {
    return this.indexOf(value) !== -1;
  };
}
```

**Why Polyfill is used?**

* 🌐 Supports older browsers
* ⚙️ Enables modern JavaScript features
* 🚀 Improves browser compatibility


<hr style="border: 2px solid green;">

<h2 id="PWA" style="color:green; text-align:center;">What is Progressive Web App (PWA)?</h2>


* PWA is a **web application that works like a mobile app**
* It runs in a **web browser**
* Users can **install it on their device**
* It can work **offline or with slow internet**

**Examples of PWA Features**

* 📱 Installable on mobile and desktop
* 🌐 Works offline using service workers
* 🔔 Supports push notifications
* ⚡ Fast loading and good performance

**Why PWA is used?**

* 🚀 Better user experience
* 📱 App-like behavior in browser
* 🌐 Works without internet
* 🧹 No need to install from app store
