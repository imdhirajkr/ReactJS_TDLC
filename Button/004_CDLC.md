### Task_4 : Change the background color to "Hello India"

```js
import React, { useState } from 'react';

function App() {
  const [message, setMessage] = useState('Hello World');
  const [backgroundColor, setBackgroundColor] = useState('');

  const handleClick = () => {
    setMessage('Hello India');
    setBackgroundColor('yellow');
  };

  return (
    <div style={{ backgroundColor }}>
      <h1>{message}</h1>
      <button onClick={handleClick}>Click Me</button>
    </div>
  );
}

export default App;



```
