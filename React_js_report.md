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

