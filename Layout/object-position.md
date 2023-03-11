# object-position
- ইহা শুধুমাত্র  object-cover এর ক্ষেত্রে ব্যবহার করা হয় নির্ধারিত অংশ প্রদর্শনের জন্য। 

<img src='./images/objectPosn.jpg'>

```js
<div className="flex items-center justify-center h-screen w-full space-x-1" >
      <div className="w-[500px] h-[500px] bg-slate-300 ">
        <h1 className="text-2xl font-semibold text-center">without object</h1>
        <div className="  flex items-center justify-center rounded-md">
          <img src={[photo]} alt='' className="w-96 h-96 rounded-md" />
        </div>
      </div>
      <div className="w-[500px] h-[500px] bg-slate-300 ">
        <h1 className="text-2xl font-semibold text-center">object-left</h1>
        <div className="  flex items-center justify-center rounded-md">
          <img src={[photo]} alt='' className="w-96 h-96 rounded-md object-cover object-left " />
        </div>
      </div>
      <div className="w-[500px] h-[500px] bg-slate-300 ">
        <h1 className="text-2xl font-semibold text-center">object-right</h1>
        <div className="  flex items-center justify-center rounded-md">
          <img src={[photo]} alt='' className="w-96 h-96 rounded-md object-cover object-right " />
        </div>
      </div>
      <div className="w-[500px] h-[500px] bg-slate-300 ">
        <h1 className="text-2xl font-semibold text-center">object-center</h1>
        <div className="  flex items-center justify-center rounded-md">
          <img src={[photo]} alt='' className="w-96 h-96 rounded-md object-cover object-center " />
        </div>
      </div>
    </div>
```