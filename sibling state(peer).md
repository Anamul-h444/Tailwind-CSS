# Styling based on sibling state (peer-{modifier})

- যখন কোন এলিমেন্টকে sibling এর সাপেক্ষে স্টাইল করার প্রয়োজন হয় তখন sibling এর মধ্যে peer ক্লাসটি লিখতে হবে এবং টার্গেট এলিমেন্ট এর মধ্যে সিউডো ক্লাস ব্যবহার করতে হবে। (যেমনঃ peer-invalid)
- এখানে input ইলিমেন্ট এর সাপেক্ষে p ট্যাগটি প্রদর্শিত হবে।
- যদি invalid হয় তাহলে প্রদর্শিত হবে Please provide valid email!
- মনে রাখতে হবে যার সাপেক্ষে স্টাইল করার প্রয়োজন তাহাকে সবসময় উপরে রাখতে হবে অন্যথায় কাজ করবেনা।

```css
<div>
    <span class="block">Email</span>

    <input
        type="email"
        class="peer w-56 h-10 px-6 py-2 border-2 border-gray-400 rounded-md outline-none focus:border-purple-600 text-lg text-gray-400 focus:text-purple-700 border-opacity-50"
    />
    
    <p class="mt-2 invisible peer-invalid:visible">Please provide valid email!</p>
      </div>
```
