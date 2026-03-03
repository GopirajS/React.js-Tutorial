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

