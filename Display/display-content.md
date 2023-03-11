# Display-contents
- কোন এলিমেন্ট এ  ব্যবহার করলে Display-content সে তার প্যারেন্টস ডিভের সমস্ত ক্লাস ব্যবহার করে।
- এক্ষেত্রে তার মধ্যে থাকা কোন ক্লাসগুলো কাজ করবেনা
## Without content
```js
<div className="flex ">
      <div class="flex gap-2 bg-purple-200">
        <div className="bg-red-100 w-24 h-24">01</div>
        <div className="bg-red-200 w-24 h-24">02</div>
        <div className="bg-red-300 w-24 h-24">03</div>
        <div className="bg-red-400 w-24 h-24">04</div>
      </div>
      <div class="gap-2 bg-yellow-200">
        <div className="bg-blue-100 w-24 h-24">01</div>
        <div className="bg-blue-200 w-24 h-24">02</div>
        <div className="bg-blue-300 w-24 h-24">03</div>
        <div className="bg-blue-400 w-24 h-24">04</div>
      </div>
    </div>
```
## Result:
- প্যারেন্টস ডিভকে flex করার কারণে চিলড্রেন ডিভগুলো রো বরাবর এসেছে।
- চিলড্রেন ২য় ডিভটি flex না হওয়ায় তার কনটেন্টগুলো ১ম ডিভের পাশে এসে নিচে নিচে এসেছে।
<img src= './images/contents1.jpg'/>

## Use Content:
```js
<div className="flex ">
      <div class="flex gap-2 bg-purple-200">
        <div className="bg-red-100 w-24 h-24">01</div>
        <div className="bg-red-200 w-24 h-24">02</div>
        <div className="bg-red-300 w-24 h-24">03</div>
        <div className="bg-red-400 w-24 h-24">04</div>
      </div>
      <div class=" constents gap-2 bg-yellow-200">
        <div className="bg-blue-100 w-24 h-24">01</div>
        <div className="bg-blue-200 w-24 h-24">02</div>
        <div className="bg-blue-300 w-24 h-24">03</div>
        <div className="bg-blue-400 w-24 h-24">04</div>
      </div>
    </div>
```
## Result:
- প্যারেন্টস ডিভকে flex করার কারণে চিলড্রেন ডিভগুলো রো বরাবর এসেছে।
- চিলড্রেন ২য় ডিভটি flex না হওয়া সত্ত্বেও flex হয়েছে। কারণ সে প্যারেন্টস ডিভের সমস্ত ক্লাস ইনহেরিট করেছে।
- তবে এক্ষেত্রে তার মধ্যে থাকা বাকি ক্লাসগুলো কাজ করবেনা। যেমন:gap-2 bg-yellow-200 কাজ করছেনা। 
<img src= './images/contents2.jpg'/>