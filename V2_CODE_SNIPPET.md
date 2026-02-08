
## 1. How to create a functional component?

```jsx
function MyComponent() {
  return <h1>Hello React</h1>;
}

export default MyComponent;
```

---

## 2. How to call one component inside another?

```jsx
function Child() {
  return <p>Child Component</p>;
}

function Parent() {
  return <Child />;
}
```

---

## 3. How to pass data from parent to child?

```jsx
function Child({ name }) {
  return <p>{name}</p>;
}

function Parent() {
  return <Child name="React" />;
}
```

---

## 4. How to create and update state?

```jsx
const [count, setCount] = useState(0);

<button onClick={() => setCount(count + 1)}>+</button>
```

---

## 5. How to use `useEffect` on component load?

```jsx
useEffect(() => {
  console.log("Component Mounted");
}, []);
```

---

## 6. How to fetch API data and store in state?

```jsx
const [users, setUsers] = useState([]);

useEffect(() => {
  fetch("https://jsonplaceholder.typicode.com/users")
    .then(res => res.json())
    .then(data => setUsers(data));
}, []);
```

---

## 7. How to list API data using `map()`?

```jsx
<ul>
  {users.map(user => (
    <li key={user.id}>{user.name}</li>
  ))}
</ul>
```

---

## 8. How to use `useRef`?

```jsx
const inputRef = useRef();

<button onClick={() => inputRef.current.focus()}>
  Focus
</button>

<input ref={inputRef} />
```

---

## 9. How to use `useContext`?

```jsx
const MyContext = createContext();

<MyContext.Provider value="Hello">
  <Child />
</MyContext.Provider>
```

```jsx
const value = useContext(MyContext);
```

---

## 10. How to create a custom hook?

```jsx
function useCounter() {
  const [count, setCount] = useState(0);
  return { count, setCount };
}
```

```jsx
const { count, setCount } = useCounter();
```
