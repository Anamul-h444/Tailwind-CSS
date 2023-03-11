# Display block, inline and inline-block

## Block element list:
```html
- <address> -   Contact information.
- <article> -   Article content.
- <aside> -     Aside content.
- <blockquote> -  Long ("block") quotation.
- <details> -    Disclosure widget.
- <dialog> -     Dialog box.
- <dd> -     Describes a term in a description list.
- <div> -    Document division.
- <dl> -     Description list.
- <dt> -     Description list term.
- <fieldset> -   Field set label.
- <figcaption> -   Figure caption.
- <figure> -    Groups media content with a caption 
- <footer> -    Section or page footer.
- <form> -     Input form.
- <h1>, <h2>, <h3>, <h4>, <h5>, <h6> -    Heading levels 1-6.
- <header> -    Section or page header.
- <hgroup> -    Groups header information.
- <hr> -     Horizontal rule (dividing line).
- <li> -    List item.
- <main> -    Contains the central content unique to this document.
- <nav> -     Contains navigation links.
- <ol> -     Ordered list.
- <p> -     Paragraph.
- <pre> -     Preformatted text.
- <section> -    Section of a web page.
- <table> -     Table.
- <ul> -     Unordered list.
```
## inline element list:
```html

    <a>
    <abbr>
    <acronym>
    <audio> (if it has visible controls)
    <b>
    <bdi>
    <bdo>
    <big>
    <br>
    <button>
    <canvas>
    <cite>
    <code>
    <data>
    <datalist>
    <del>
    <dfn>
    <em>
    <embed>
    <i>
    <iframe>
    <img>
    <input>
    <ins>
    <kbd>
    <label>
    <map>
    <mark>
    <meter>
    <noscript>
    <object>
    <output>
    <picture>
    <progress>
    <q>
    <ruby>
    <s>
    <samp>
    <script>
    <select>
    <slot>
    <small>
    <span>
    <strong>
    <sub>
    <sup>
    <svg>
    <template>
    <textarea>
    <time>
    <u>
    <tt>
    <var>
    <video>
    <wbr>
```
# inline-block
- কোন inline এলিমেন্টে inline-block ব্যবহার করলে উক্ত এলিমেন্ট সরাসরি block এলিমেন্ট হবেনা inline ই থাকবে কিন্ত তার মধ্যে block এর মত সব সিএসএস ব্যবহার করা যাবে। 
- কোন block এলিমেন্টে inline-block ব্যবহার করলে উক্ত এলিমেন্ট সরাসরি inline হবে শুধু আচরণ inline এলিমেন্ট এর মত হবে  কিন্ত তার মধ্যে block এর মত সব সিএসএস ব্যবহার করা যাবে। 
 # inline Vs inline-block
 ```js
 <div className="bg-blue-700 w-48 h-48 m-6">
        <span className="bg-blue-200 m-4 p-4 w-36 h-36 ">
          I am inline element
        </span>
      </div>

      <div className="bg-purple-700 w-48 h-48 m-6">
        <span className="inline-block bg-green-300 m-4 p-4 w-36 h-36">
          I am inline-block element
        </span>
      </div>
 ```
 ## Result:
 - inline এলিমেন্টে top margin, top padding, width, height কাজ করবেনা। এখানে মার্জিং এবং প্যাডিং কাজ করেছে কিন্তু টপে কাজ করেনি। প্যাডিং যদিও দেখা যাচ্ছে কিন্তু েকনটেন্ট তার নিজ স্থানেই রয়েছে। 
 - নিচে span ট্যাগ inline হওয়া সত্ত্বেও তাহাকে inline-block হিসেবে ব্যবহার কারণে তার মধ্যে সবই কাজ করেছে। 
 
 <img src='./images/inlineVs.jpg' />

 # inline-block vs block
 
 ```js
  <div className="flex text-white">
      <div className="bg-blue-700 w-48 h-48 m-6">
        <p>
          I am <span>inline</span> element
        </p>
      </div>

      <div className="bg-purple-700 w-60 h-48 m-6">
        <p>
          I am <span className="inline-block bg-red-400 w-32 p-5 mt-2">inline-block</span> element
        </p>
      </div>

      <div className="bg-green-700 w-48 h-48 m-6">
        <p>
        I am <span className="block bg-slate-400 w-32 p-5 mt-2">block</span> element
        </p>
      </div>
    </div>
 ```
 ## Result:
 - span ট্যাগ inline এলিমেন্ট তাহাকে inline-block করে তার মধ্যে ব্লক এর মত সমস্ত সিএএস এপ্লাই করা হয়েছে এবং কাজ করেছে কিন্তু সে inline ই রয়েছে কারণ সে তার লাইন ছাড়েনি। 
 -  span ট্যাগ inline এলিমেন্ট তাহাকে block করে তার মধ্যে ব্লক এর মত সমস্ত সিএএস এপ্লাই করা হয়েছে এবং কাজ করেছে কিন্তু সে সম্পূর্ণভাবে block এলিমেন্ট হয়ে গিয়েছে। কারণ সে লাইন ছেড়ে নিজে সম্পূর্ণ একটি ব্লক দখল করেছে।
 <img src='./images/blockVs.jpg' />