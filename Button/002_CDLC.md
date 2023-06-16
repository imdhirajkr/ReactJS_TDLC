### Question : Displays "Hello, how are you?" in a popup when the button is clicked: 

```js
import React from 'react';

function App() {
  const handleClick = () => {
    alert('Hello, how are you?');
  };

  return (
    <div>
      <h1>Simple Button</h1>
      <button onClick={handleClick}>Click Me</button>
    </div>
  );
}

export default App;

```