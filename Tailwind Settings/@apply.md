# @apply
- এর মাধ্যমে index.css এ base, utility, components এর ক্লাস তৈরী করে এলিমেন্টে ব্যবহার করা যায়। 
- এর মাধ্যমে তৈরীকৃত কম্পোনেন্টে এলিমেন্টে টেইলউইন্ড এর utility ক্লাস ব্যবহার করলে তা কাজ করবেনা। কাজ করাতে হলে @layer ব্যবহার করতে হবে।  

## Example:
### index.css:
```js
@tailwind base;
@tailwind components;
@tailwind utilities;
  .btn {
    @apply inline-block px-5 py-3 rounded-lg outline-none focus:ring focus:ring-offset-2 uppercase tracking-wider font-semibold text-sm sm:text-base
  }
  .btn-primary {
    @apply bg-indigo-500 hover:bg-indigo-400 focus:ring-2 focus:ring-opacity-5 active:bg-indigo-600 hover:translate-y-2
  }

```
### App.js
```js
import React from "react";

function App() {
  return (
    <div className=" m-96">
      <button className="btn btn-primary">Submit</button>
    </div>
  );
}

export default App;
```