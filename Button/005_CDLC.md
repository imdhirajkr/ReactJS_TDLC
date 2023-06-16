### Task_5 : Play the music when button is clicked

```js
import React, { useState, useRef } from 'react';

function App() {
  const [message, setMessage] = useState('Hello World');
  const [backgroundColor, setBackgroundColor] = useState('');

  const audioRef = useRef(null);

  const handleClick = () => {
    setMessage('Hello India');
    setBackgroundColor('yellow');
    audioRef.current.play();
  };

  return (
    <div style={{ backgroundColor }}>
      <h1>{message}</h1>
      <button onClick={handleClick}>Click Me</button>
      <audio ref={audioRef}>
        <source src="audio/airtel.mp3" type="audio/mpeg" />
      </audio>
    </div>
  );
}

export default App;



```
