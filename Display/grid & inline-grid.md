# Display- grid & inline-grid
## display-grid
```js
<div className="space-y-2 ">
      <div class="grid grid-cols-2 gap-2 bg-purple-200">
        <span className="bg-red-100 w-24 h-24">01</span>
        <span className="bg-red-200 w-24 h-24">02</span>
        <span className="bg-red-300 w-24 h-24">03</span>
        <span className="bg-red-400 w-24 h-24">04</span>
      </div>
      <div class="grid grid-cols-2 gap-2 bg-yellow-200">
        <span className="bg-blue-100 w-24 h-24">01</span>
        <span className="bg-blue-200 w-24 h-24">02</span>
        <span className="bg-blue-300 w-24 h-24">03</span>
        <span className="bg-blue-400 w-24 h-24">04</span>
      </div>
    </div>
```
### Result:
- grid ব্লক হিসেবে কাজ করে। 
- ডিভের মধ্যে grid ও grid-cols-2 নির্ধারণ করার কারণে চারটি এলিমেন্ট পুরো ওয়াইডথটিকে দুটি কলামে ভাগ করে সমস্ত জায়গা দখল করে নিয়েছে।
- grid ব্লক হিসেবে কাজ করে বিধায় দুইটি ডিভ পরস্পর নিচে ব্লক হিসেবে অবস্থান করছে। 
<img src='./images/block.jpg' />

## First div inline:
```js
<div className="space-y-2 ">
      <div class="inline-grid grid-cols-2 gap-2 bg-purple-200">
        <span className="bg-red-100 w-24 h-24">01</span>
        <span className="bg-red-200 w-24 h-24">02</span>
        <span className="bg-red-300 w-24 h-24">03</span>
        <span className="bg-red-400 w-24 h-24">04</span>
      </div>
      <div class="grid grid-cols-2 gap-2 bg-yellow-200">
        <span className="bg-blue-100 w-24 h-24">01</span>
        <span className="bg-blue-200 w-24 h-24">02</span>
        <span className="bg-blue-300 w-24 h-24">03</span>
        <span className="bg-blue-400 w-24 h-24">04</span>
      </div>
    </div>
```
### Result:
- প্রথম ডিভকে inline-grid grid-cols-2 নির্ধারণ করার কারণে ডিভটি ব্লক হওয়া সত্বেও ইনলাইনের আচরণ করল। ফলে তার অভ্যন্তরীন এলিমেন্টগুলো পাশাপাশি চলে আসল এবং ডানে জায়গা ছেড়ে দিল। 
- ২য় ডিভটি ব্লক হওয়ার কারণে সে নিচে রয়ে গেল। 
<img src='./images/inline1.jpg'/>

## Both div inline:
```js
<div className="space-y-2 ">
      <div class="inline-grid grid-cols-2 gap-2 bg-purple-200">
        <span className="bg-red-100 w-24 h-24">01</span>
        <span className="bg-red-200 w-24 h-24">02</span>
        <span className="bg-red-300 w-24 h-24">03</span>
        <span className="bg-red-400 w-24 h-24">04</span>
      </div>
      <div class="inline-grid grid-cols-2 gap-2 bg-yellow-200">
        <span className="bg-blue-100 w-24 h-24">01</span>
        <span className="bg-blue-200 w-24 h-24">02</span>
        <span className="bg-blue-300 w-24 h-24">03</span>
        <span className="bg-blue-400 w-24 h-24">04</span>
      </div>
    </div>
```
### Result:
- ২য় ডিভকে inline-grid grid-cols-2 নির্ধারণ করার কারণে ডিভটি ব্লক হওয়া সত্বেও ইনলাইনের আচরণ করল। ফলে তার অভ্যন্তরীন এলিমেন্টগুলো পাশাপাশি চলে আসল এবং ১ম ডিভের ডানের ছেড়ে দেওয়া জায়গা দখল করল।

<img src='./images/inline2.jpg'/>