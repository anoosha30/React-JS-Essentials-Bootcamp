# React-JS-Essentials-Bootcamp
Assignment - React JS Essentials Bootcamp

import React, { useState } from 'react';
import ReactDOM from 'react-dom';

function App() {
  const [backgroundColor, setBackgroundColor] = useState('white');

  const toggleBackgroundColor = () => {
    setBackgroundColor(prevColor => prevColor === 'white' ? 'lightblue' : 'white');
  };

  return (
    <div style={{ backgroundColor, height: '100vh' }}>
      <button onClick={toggleBackgroundColor}>Toggle Background Color</button>
    </div>
  );
}

ReactDOM.render(<App />, document.getElementById('root'));
