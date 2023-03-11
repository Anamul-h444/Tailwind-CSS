- npm init --y
- npm install -D tailwindcss
- npx tailwindcss init

## tailwind.config.js

```js
module.exports = {
  content: ["./src/**/*.{html,js}"], //src এর মধ্যে থাকা এইচটিএমএল এবং জেএস ফাইলকে রিড কর
  theme: {
    extend: {},
  },
  plugins: [],
};
```

## src/input.css

```js
@tailwind base;
@tailwind components;
@tailwind utilities;
```

## package.json

- src/input.css file transfer as output in dist/output.css

```
"scripts": {
    "build": "npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch"
  }
```

- npm run build (Then create /dist/output.css)

## src/index.html

```js
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="../dist/output.css" /> //Link output file
  </head>
  <body>
    <h1 class="text-3xl font-bold underline bg-slate-600">Hello world!</h1>
  </body>
</html>
```
