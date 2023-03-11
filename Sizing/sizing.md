# height

- By default height 0

# min-height

- মিনিমাম হাইট নির্ধারিত প্যারেন্টস এর চিলড্রেন এর হাইট যখন প্যারেন্টস এর তুলনায় কম হবে তখনই সে কাজ করবে। এছাড়া নির্ধারিত হাইটের বেশির ক্ষেত্রে ওয়াইডথ এর সাথে সমন্বয় করে রেসপনসিভ হিসেবে কাজ করবে। ।
- সর্বোচ্চ যত ইচ্চা হাইট কাজ করবে।
- প্যারেন্টস এর নির্ধারণকৃত মিনিমাম হাইট এর তুলনায় চিলড্রেন এর হাইট কম হলে চিলড্রেন দখল করার পর মিনিমাম হাইটের বাকিটুকু খালি থাকবে।

# Example:
# Original Size
<img src='./images/sz-1.jpg'>

```js
<div className="bg-blue-700 text-white w-48 min-h-[110px]">
  <p className="text-2xl">Original Size</p>
</div>
```
# Over Size/Responsive
<img src='./images/sz-2.jpg'>

```js
<div className="bg-blue-700 text-white w-48 min-h-[110px]">
  <p className="text-2xl">Over Size</p>
  <p>
    Note that the development build is not optimized. To create a production
    build, use npm run buildNote that the development build ist optimized. To
    create a production build, use npm run build
  </p>
</div>
```
# Under-size
<img src='./images/sz-3.jpg'>

```js
<div className="bg-blue-700 text-white w-48 min-h-[110px]">
  <p className="text-2xl">Under Size</p>
  <p>Note</p>
</div>
```
# max-height
- সর্বনিম্ন যেকোন হাইট দেওয়া যাবে। 
- ম্যাক্সিমাম হাইট নির্ধারিত প্যারেন্টস এর চিলড্রেন এর হাইট যখন প্যারেন্টস এর তুলনায় বেশি হবে তখনই সে কাজ করবে। । নির্ধারিত হাইটের চেয় কম হাইটের ক্ষেত্রে ওয়াইডথ এর সাথে সমন্বয়ে রেসপনসিভ হিসেবে কাজ করবে।
- প্যারেন্টস এর নির্ধারণকৃত ম্যাক্সিমাম হাইট এর তুলনায় চিলড্রেন এর হাইট বেশি হলে চিলড্রেন দখল করার পর ওভারফ্লো হবে।