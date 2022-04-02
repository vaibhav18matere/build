### Class Work 1: Increment button counter

- Create a button and increment a counter every time that button is clicked. log the counter on console after every render.
[Solution](https://codesandbox.io/s/useeffect-odno00?file=/src/Counter.jsx)

### Class Work 2: predict the output and order

- What will be the console for the initial render?
- What will be the console after user clicks increment button?

```
export default function App() {
  const [counter, setCounter] = useState(0)

  useEffect(() => {
    console.log('from useEffect...', counter)
  })

  function incrementClickHandler() {
    setCounter((counter) => {
      console.log('from click handler...', counter)
      return counter + 1
    })
  }

  console.log('before render...', counter)
  return (
    <div className='App'>
      <h1>{counter} </h1>
      <button onClick={incrementClickHandler}>Increment </button>
    </div>
  )
}
```

[solution](https://codesandbox.io/s/objective-dawn-93tbf8)

### Class Work 3: Save items to localStorage

- [Documentation](https://developer.mozilla.org/en-US/docs/Web/API/Window/localStorage) to refer: 
  - Open your console.
  - localStorage.setItem('myKey', 'myValue')
  - Go to Applications and you'll see this value updated.
  - Now, let's refresh the browser
  - You see that it's still there. Local Storage values are preserved across sessions.
  - Let's read this value in console using localStorage.getItem('myKey')
  - Now, let's try to store an array into localStorage, you'll see that it loses the value
  - How do we solve this? JSON.stringify() to the rescue.

- Use [this](https://codesandbox.io/s/wishlist-exercise-oydf9) codesanbox for the exercise.
- There's a working wishlist in this. However, the wishlist is not saved after it is updated. 
- Use useEffect() and localStorage API to save this data to localStorage.
- Add a console log as well to print data updated every time this effect is run.
- [Solution](https://codesandbox.io/s/useeffect-odno00?file=/src/Wishlist.jsx)

### Class Work 4: save wishlist to server

- Wishlist udpates should saved to the server using API calls.
- And then read from those APIs when WishList is loaded. [check - practice react repo]()

### excercise 1 : make your counter print console only once

- Use the useEffect dependency array to control how many times it is logged. Log it only once and say,
  "Hey! This is the initial value of Counter: { counter }".
- Make sure that it doesn't run on every render. [add empty array - to the end of useEffect]()

### excercise 02: fix saving to wishlist

- Remember how saving to wishlist was happening even when the text was getting updated in the input box. Fix that now using the dependency array to run only when the list is updated and not the text. [add state variable - which needs to change]()

- Fix the dependency array for the network call being made in previous homework where you are saving the wishlist to server.

### excercise 3: Can you fix the problem?

[Question](https://codesandbox.io/s/fix-localstorage-success-saved-sggj0)

[Answer](https://codesandbox.io/s/fix-localstorage-success-saved-fixed-kkc3d)

### Practice more

[Check axios syntax](https://github.com/axios/axios)

### ex04: GET data

- [challenge](https://codesandbox.io/s/load-data-exercise-xm4qo?file=/README.md)

- [My Solution](https://codesandbox.io/s/useeffect-server-calls-1lwhtj?file=/src/App.js)

- [solution](https://codesandbox.io/s/load-data-exercise-forked-cy4vbg)

### ex05: Load Data on page render

- [challenge](https://codesandbox.io/s/load-products-tzdb8?file=/README.md)
- [solution](https://codesandbox.io/s/useeffect-load-products-9lscwp)

### ex06: POST data

- [challenge](https://codesandbox.io/s/post-request-exercise-exo0j)

### ex07

- This is your address management for eCommerce website.
- Overtime, turn it into a full-fledged app with all the bells and whistles of address management

1. input validation
2. multiple fields
3. remove address
4. edit address

- See Flipkart or Amazon's address management for inspiration.
