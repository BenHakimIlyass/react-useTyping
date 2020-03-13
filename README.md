# react-useTyping
Created with CodeSandbox
Demo : https://codesandbox.io/s/funny-bouman-bejjb
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
