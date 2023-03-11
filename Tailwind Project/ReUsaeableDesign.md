## Create a button
- যদি কোন কম্পোনেন্টকে ইমপোর্ট করে  <> </> এভাবে ব্যবহার করা হয় তাহলে তার ইমপোর্টকৃত কম্পোনেন্টে প্রপসের children এ  <> </> তার মাঝের অংশ পাস হয়।
```js
import React from "react";

export const Button = (props) => {
  console.log(props);
  return (
    <div>
      <button className="bg-purple-700 text-white px-6 py-2 rounded-md m-5">
        {props.children}
      </button>
    </div>
  );
};
```
## Use This button
```js
import React from "react";
import { Button } from "./Button";

function Home() {
  return (
    <>
      <Button>Get Started</Button>
      <Button>More</Button>
      <Button>Submit</Button>
    </>
  );
}

export default Home;
```