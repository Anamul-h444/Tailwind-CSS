# font-family

## use font in element

```js
<p class="font-sans ...">The quick brown fox ...</p>
<p class="font-serif ...">The quick brown fox ...</p>
<p class="font-mono ...">The quick brown fox ...</p>
```

## Use custom font-famil

### index.css:

```js
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600&display=swap');
@tailwind base;
@tailwind components;
@tailwind utilities;
```

### Config.js:

```js
extend: {
      fontFamily: {
        poppins: ["Poppins", "sans-serif"],
      },
    }
```

### Arbitrary values:

```js
<p class="font-['Poppins']">
  <!-- ... -->
</p>
```

- custom font এর যে weight গুলো import করা হয়েছে তা নির্ধারণ করতে হবে tailwind এর font-weight প্রপার্টির মাধ্যমে।
- custom font এর যে weight গুলো import করা হয়নি tailwind এর font-weight সে প্রপার্টি ব্যবহার করলে কাজ করবেনা।

```js
className="max-h-[200px] bg-red-600 text-black font-poppins font-thin
```
