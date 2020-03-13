# react-useTyping
Created with CodeSandbox
# Api
 
 ```javascript
import React from "react";
import useTyping from "./useTyping";

const MyComponent=()=> {
  const [typing, data, setData] = useTyping();
  return (
    <div>
      <h1>{data && data}</h1>
      <h2>{typing === true && "Typing..."}</h2>
      <input onChange={e => setData(e.target.value)} />
    </div>
  );
}
export default MyComponent;
