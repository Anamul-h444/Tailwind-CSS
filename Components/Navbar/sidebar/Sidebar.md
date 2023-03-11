# Sidebar
- Main div divided by sidebar + Homepage
- By state when sidebar open set width and when sidebar close set width. Other width is for Homepage.
- By flex main div create two dive side to side.

```js
import React, { useState } from "react";
import controlImg  from './assets/images/control.png'
import logo  from './assets/images/logo.png'
import calender  from './assets/images/Calendar.png'
import chart_fill  from './assets/images/Chart_fill.png'
import chart  from './assets/images/Chart.png'
import chat  from './assets/images/Chat.png'
import folder  from './assets/images/Folder.png'
import search  from './assets/images/Search.png'
import setting  from './assets/images/Setting.png'
import user  from './assets/images/User.png'

export const Home = () => {
  const Menus = [
    { title: "Dashboard", src:[chart_fill] },
    { title: "Inbox", src: [chat] },
    { title: "Accounts", src: [user], gap: true },
    { title: "Schedule ", src: [calender] },
    { title: "Search", src:[search] },
    { title: "Analytics", src: [chart] },
    { title: "Files ", src:[folder], gap: true },
    { title: "Setting", src: [setting] },
  ];

  const [open, setOpen] = useState(true)
  const sidebar = () => (
    <div className="flex">
      {/* ..............................Sidebar........................ */}
      <div className={`${open ? 'w-72' : 'w-20'} h-screen bg-dark-purple relative transition-all duration-500 ease-in pt-8 p-5 `}>
        <img 
        src={[controlImg]} 
        alt=''
        className={`absolute -right-3 top-9 w-7 border-2 border-dark-purple rounded-full ${!open && 'rotate-180'}`}
        onClick={()=> setOpen(!open)}
        />
      <div className={`flex gap-x-4 items-center origin-left `}>
        <img
        src={[logo]}
        className={` cursor-pointer ${open && "rotate-[360deg]"} duration-200`} // এ্যারোর রোটেটিং নির্ধারণ করা হয়েছে।
        alt=''
        />
        <h1 className={`text-white font-semibold text-xl ${!open && 'scale-0'} duration-500`}>Designer</h1> // যখন ‍বার ক্লোজ হবে তখন টাইটেল লেখাগুলো হাইড হবে।
      </div>
      <ul className="pt-6">
        {
          Menus.map((menu, index)=>(
           <li key={index} className={`flex items-center gap-x-4 p-2 hover:bg-light-white rounded-md ${menu.gap ? 'mt-9' : 'mt-2'}`}> // গ্যাপ তৈরী করা হয়েছে।
            <img src={menu.src} alt='' className="cursor-pointer " />
            <span className={`text-gray-300 text-sm cursor-pointer ${!open && 'scale-0' } duration-500   `}>{menu.title}</span> // যখন ‍বার ক্লোজ হবে তখন টাইটেল লেখাগুলো হাইড হবে।
           </li>
          ))
        }
      </ul>

      </div>

      {/* ..............................Homepage........................ */}
      <div className="p-7 text-2xl font-semibold flex-1 h-screen">Homepage</div>
    </div>
  );
  return <div>{sidebar()}</div>;
};
export default Home;
```