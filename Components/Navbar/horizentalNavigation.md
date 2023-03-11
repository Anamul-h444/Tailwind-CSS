## মিডিয়াম স্ক্রিন
- মেনুগুলো ফ্লেক্স রো বরাবর থাকবে, মেনুবারের নাম ও মেনুগুলো জাস্টিফাই বিটোইন থাকবে।

## স্মল স্ক্রিন
- মেনুগলো li এর মাধ্যমে নিচে নিচে থাকবে।
- দুইটি আইকেন থাকবে একটি মেনু আরেকটি ক্রস।
- যখন ওপেন থাকবে তখন ক্রস প্রদর্শিত হবে অন্যসময় মেনু প্রদর্শিত হবে। 
- মেনুতে ক্লিক করলে মেনুবার আসবে এবং ক্রস এ ক্লিক করলে মেনুবার চলে যাবে। 



```js
import React, { useState } from "react";
import { BiAnalyse } from "react-icons/bi";
import { AiOutlineMenu, AiOutlineClose } from "react-icons/ai";

const Timeline = () => {
  const [isOpen, setIsOpen] = useState(false);
  let Link = [
    { name: "Home", link: "/" },
    { name: "Contact", link: "/" },
    { name: "About Us", link: "/" },
    { name: "Menu", link: "/" },
  ];
  const timeline = () => (
/* ...........body............*/
    <div className="bg-indigo-600 w-full h-screen"> 

/* ...........Menubar............*/
      <div className="shadow-lg w-full fixed bg-white py-4 md:flex md:items-center md:justify-between">    //This is menubar

/* ...........menubar name and icon............*/
        <div className="flex items-center font-bold text-2xl space-x-2 md:px-10 px-7">   
          <span className="text-indigo-600 text-3xl">
            <BiAnalyse />
          </span>
          <span>Designer</span>
        </div>
/* ...........open and show icon............*/
        <div
          onClick={() => setIsOpen(!isOpen)}
          className="absolute right-4 top-4 text-2xl md:hidden"
        >
          {isOpen ? <AiOutlineClose /> : <AiOutlineMenu />}
        </div>

/* ...........open and show ul/li items............*/
        <ul
          className={`md:flex md:items-center px-7 md:pb-0 pb-7 transition-all duration-500 ease-in ${
            isOpen ? "top-[65px] " : "top-[-490px] "
          } md:opacity-100 absolute bg-white w-full md:w-auto md:static md:z-auto z-[-1] `}
        >
          {Link.map((link) => (
            <li className="md:ml-8 text-xl md:my-0 my-7">
              <a
                className="text-gray-800 hover:text-gray-400 duration-500"
                href={link.link}
              >
                {link.name}
              </a>
            </li>
          ))}
          <button className="text-white bg-indigo-600 px-2 py-2 rounded-md hover:bg-indigo-400 md:ml-8 md:mr-8 duration-500">
            Get Started
          </button>
        </ul>
      </div>
    </div>
  );

  return <div>{timeline()}</div>;
};

export default Timeline;


```