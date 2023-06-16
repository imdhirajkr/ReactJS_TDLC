### Task_3 : Display "Hello India" from "Hello World" whenever button is clicked 

```js
import React, { useState } from 'react';

function App() {
  const [message, setMessage] = useState('Hello World');

  const handleClick = () => {
    setMessage('Hello India');
  };

  return (
    <div>
      <h1>{message}</h1>
      <button onClick={handleClick}>Click Me</button>
    </div>
  );
}

export default App;


```

* We use the useState hook to create a state variable called message and a function to update it called setMessage. 

* The initial value of message is set to "Hello World".
* We define a function called handleClick that will be called when the button is clicked. * Inside this function, we call setMessage to update the value of message to "Hello India".
* In the JSX, we use curly braces `{}` to display the value of message in the `<h1>` element.
* The onClick attribute of the button is set to the handleClick function, so when the button is clicked, the handleClick function will be called and the message will be updated to "Hello India", causing the `<h1>` element to display "Hello India".