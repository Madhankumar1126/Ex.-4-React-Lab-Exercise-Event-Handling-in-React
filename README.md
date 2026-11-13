# Ex.-4-React-Lab-Exercise-Event-Handling-in-React
## Name: Madhan Kumar J
## Roll no: 2305001016
## Department: CSE

## AIM
### To understand and implement event handling in React using events such as onClick, onChange, and onSubmit. 

## PROGRAM
### App.jsx  
### i) onClick Event function
```py
App() {   function handleClick() {     alert("Button was clicked!"); 
  }   return ( 
    <div> 
      <h1>React Event Handling</h1> 
      <button onClick={handleClick}> 
        Click Me 
      </button> 
    </div> 
  ); 
} export default App;
```
 
### ii) onClick with State
```py
import { useState } from "react"; function App() {   const [count, setCount] = useState(0);   function handleClick() {     setCount(count + 1); 
  }   return ( 
    <div> 
      <h1>Click Counter</h1> 
      <h2>Button clicked: {count} times</h2> 
      <button onClick={handleClick}> 
        Click Me 
      </button> 
    </div> 
  ); 
} export default App; 
 ```
### iii) onChange Event 
```py
import { useState } from "react"; function App() {   const [name, setName] = useState("");   function handleChange(event) {     setName(event.target.value); 
  }   return ( 
    <div> 
      <h1>Student Name</h1> 
      <input 
        type="text" 
        placeholder="Enter your name"         onChange={handleChange} 
      /> 
      <h2>Hello, {name}</h2> 
    </div> 
  ); 
} export default App; 
```
## OUTPUT
<img width="816" height="291" alt="image" src="https://github.com/user-attachments/assets/aaece1bc-6a74-4060-bef7-2542d68f1572" />
<img width="818" height="296" alt="image" src="https://github.com/user-attachments/assets/eaba908d-7076-4fea-8f69-4e14ed3a73f9" />
<img width="820" height="302" alt="image" src="https://github.com/user-attachments/assets/05c59eb5-d8f5-4d4b-80e2-0ebc6e81b4a1" />




## RESULT
### Thus, React event handling was successfully implemented using the onClick and onChange events. The application responded to button clicks, maintained a click counter using useState, and displayed the student's name dynamically based on user input. 
