### 1. create a component named "Person" that takes two props "name" and "age".The compnent should display the person's name and age in a paragraph element.

```javascript
import React from 'react';

const Person = ({ name, age }) => {
  return (
    <div>
      <p>Name: {name}</p>
      <p>Age: {age}</p>
    </div>
  );
};

export default Person;

```

### 2. create a component named "Button" that takes two props- "text and "click". The compnent should display a button element with given text and call the onClick function when Clicked.
```javascript
import React from 'react';
import Button from './Button'; // Assuming the component file is in the same directory

const App = () => {
  const handleButtonClick = () => {
    console.log('Button clicked!');
    // You can add your custom logic here to execute when the button is clicked.
  };

  return (
    <div>
      <h1>Button Component Example</h1>
      <Button text="Click Me" click={handleButtonClick} />
    </div>
  );
};

export default App;
```
### 3.create a component named "Header" that takes one prop-  "title". The compnent should display a header element with given title.
```javascript
import React from 'react';

const Header = ({ title }) => {
  return (
    <header>
      <h1>{title}</h1>
    </header>
  );
};

export default Header;
```
### 3.create a component named "List" that takes one prop-  "items". The compnent should display an unordered list element with given list items.
```javascript
import React from 'react';

const List = ({ items }) => {
  return (
    <ul>
      {items.map((item, index) => (
        <li key={index}>{item}</li>
      ))}
    </ul>
  );
};

export default List;
```