# @layer
- @apply এর মাধ্যমে index.css এ base, utility, components এর ক্লাস তৈরী করে এলিমেন্টে ব্যবহার করা যায়। 
- এই base, utility, components এর ক্লাস কে @layer এ রাখলে এলিমেন্টে Tailwind এর utility ক্লাস দ্ধারা কাস্টমাইজ করা যাবে। 

## Components:
- @layer এর ভিতর Components class এর নাম দিয়ে @apply এর পর utility class লিখতে হবে। 
## utilities:
- @layer এর ভিতর utilities class এর নাম দিয়ে তার ভিতর css এর প্রপার্টি লিখে উক্ত প্রপার্টির ভেল্যু এসাইন করতে হবে।
## base:
- Tailwind by default সমস্ত প্রকার এইচটিএমএল এলিমেন্টের সাইজ, মার্জিন, প্যাডিং, লিষ্টিং, বর্ডার ইত্যাদি রিসেট করে দেয়। সুতরাং এগুলোর ভেল্যু এসাইন করা যায়।
- @layer এর ভিতর HTML Element এর নাম দিয়ে তার ভিতর Tailwind Utility class এর মাধ্যমে উক্ত Element এর ভেল্যু এসাইন করতে হবে।

## Example:
### index.css:
```js
@tailwind base;
@tailwind components;
@tailwind utilities;

@layer components {
  .btn {
    @apply inline-block px-5 py-3 rounded-lg outline-none focus:ring focus:ring-offset-2 uppercase tracking-wider font-semibold text-sm sm:text-base
  }
  .btn-primary {
    @apply bg-indigo-500 hover:bg-indigo-400 focus:ring-2 focus:ring-opacity-5 active:bg-indigo-600 hover:translate-y-2
  }
}

@layer utilities {
  .my-font-size{
    font-size: 20px;
  }
}

@layer base {
  h1 {
    @apply text-2xl;
  }
  h2 {
    @apply text-xl;
  }
  h3 {
    @apply text-lg;
  }
  a {
    @apply text-blue-600 underline;
  }
}


```
### App.js
```js
import React from "react";

function App() {
  return (
    <div className=" m-96">
      <h1>I am testing base</h1>
      <button className="btn btn-primary rounded-sm my-font-size">Submit</button>
    </div>
  );
}

export default App;
```