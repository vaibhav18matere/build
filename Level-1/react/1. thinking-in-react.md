### classwork Increase Font size, Increase counter and change background color

[codesandbox solution](https://codesandbox.io/s/thinking-in-react-l6y20x?file=/src/App.js)

### ex1: character counter (Twitter)

- See the Twitter post component. It gives you an indicator of the character count. Replicate that behavior.

[codesandbox solution](https://codesandbox.io/s/reverent-glitter-n4w6x1?file=/src/TwitterCounter.jsx)

### ex2: password match

- Any signup form, password reset form has this functionality. Take two passwords from user. Show error only if both passwords don't match.

[codesandbox solution](https://codesandbox.io/s/reverent-glitter-n4w6x1?file=/src/PasswordMatch.jsx)

### ex3: alphanumeric password

- Password should contain a number. Show error if user misses character.

[codesandbox solution](https://codesandbox.io/s/reverent-glitter-n4w6x1?file=/src/AlphaNumPassCheck.jsx)

### ex4: disable submit

- Add a submit button to password change field. Disable submit button if passwords don't match
  Clicking on submit should console the password field.

[codesandbox solution](https://codesandbox.io/s/reverent-glitter-n4w6x1?file=/src/DisablePass.jsx)

### ex5: show/hide password

- Create a password reset form
  Put a button show password near the input element.
  Clicking should show password to the user.
  Text on show password should change to hide password when password is shown.
  Click on hide password and password goes back to hidden again.

  [codesandbox solution](https://codesandbox.io/s/reverent-glitter-n4w6x1?file=/src/ShowHidePass.jsx)

### ex6: designer tool (mini figma)

Let user finalise the size of text she would like on the screen. Two buttons + and - both will increase/decrease size by 8px. Show the size on the screen.
[similar to classwork](https://codesandbox.io/s/thinking-in-react-l6y20x?file=/src/App.js)

##### IDEA You can make a small app around this which quickly selects you between fonts.

- Have prefixed sizes. Multiples of 8px.
- Have some selected best fonts.
- Tell which fonts are good for heading. which are good for text.
- Suggest pair of fonts which go together.
- Give user an option to copy the CSS. (Bonus feature)

### ex7: add to cart

- Show a list of items with add to cart button
  Clicking on the button should add that item to cart.

- Show the cart below with items added.
  Clicking on the same item twice should add more items in cart.

- CHALLENGE : increase the count of the item in cart without adding it to list.

### ex8: switch tabs

- Make three components: Home, About, Profile.
- Put some text in the components
- Now, create three buttons with same name
- Clicking on the button should show that component

##### UNDERSTANDING : this is kind of your own router, unless we get into router implementation.

### ex9: toast

- Create a Toast Component
- Component should have two things

1. Text
2. Hide Button

- Create a button show toast
- Clicking on this button should show Toast
- Clicking on hide button on toast should hide the toast

##### UNDERSTAND : how callbacks can be passed to control state from parent component.

CHALLENGE :

- Create different type of toasts: Error, Success, Warning etc.
- Differentiate your toast by just a prop and the design should change.

### ex10: todo/strikethrough

- Write a TODO app
- Add TODOs from input
- Clicking on a TODO should complete it using strikethrough
- Clicking again should remove the strikethrough.

### ex11: dark mode

- Create a toggle dark mode button
- Clicking on the button should change background and text color and toggle between dark and light mode.

### ex12: like in a list

- Render a list
- Every item in the list should have a like button.

### ex13: out of stock (grey)

- Render a list of items from an array of objects. In that object, have a field outOfStock: true
  and depending on true/false grey out the out of stock object.
- Your component card should have this design built in as an additional class.
