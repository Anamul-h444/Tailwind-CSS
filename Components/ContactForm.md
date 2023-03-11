# ContactForm
<img src='././images/contactForm2.jpg'/>
```js
import React from "react";
import { MdCall, MdLocationOn } from "react-icons/md";
import { GrMail } from "react-icons/gr";
import { BsFacebook, BsTwitter } from "react-icons/bs";
import { FaInstagramSquare } from "react-icons/fa";
import { AiFillLinkedin } from "react-icons/ai";

const ContactForm = () => {
  const contactForm = () => (
    <div className="antialiased bg-gray-100">
      <div className="w-full min-h-screen flex justify-center items-center">
        {/*.........Card.......... */}
        <div className=" flex flex-col space-y-6 md:flex-row  md:space-x-6 md:space-y-0  bg-cyan-700 w-full max-w-4xl p-8 rounded-xl text-white shadow-lg overflow-hidden ">
          {/*.........Contact information.......... */}
          <div className="flex flex-col space-y-8 justify-between">
            <div>
              <h1 className="font-bold text-4xl tracking-wide">Contact Us</h1>
              <p className="text-sm text-cyan-100 pt-2">
                lorem To create a production build, use npm run build. To create
                a production build, use npm run build.{" "}
              </p>
            </div>
            <div className="flex flex-col space-y-6">
              <div className="inline-flex space-x-2 items-center">
                <p className="text-teal-400 text-xl">
                  <MdCall />
                </p>
                <span>+8801735547549</span>
              </div>
              <div className="inline-flex space-x-2 items-center">
                <p className="text-teal-400 text-xl">
                  <GrMail />
                </p>
                <span>anamul@gmail.com</span>
              </div>
              <div className="inline-flex space-x-2 items-center">
                <p className="text-teal-400 text-xl">
                  <MdLocationOn />
                </p>
                <span>122, Savar Road, Ashulia</span>
              </div>
            </div>
            <div className="inline-flex space-x-2">
              <p>
                <BsFacebook />
              </p>
              <p>
                <BsTwitter />
              </p>
              <p>
                <FaInstagramSquare />
              </p>
              <p>
                <AiFillLinkedin />
              </p>
            </div>
          </div>

          {/*.........Contact Form.......... */}
          <div className="relative">
            {/*.........Create round.......... */}
            <div className=" w-40 h-40 rounded-full bg-teal-400 absolute -right-28 -top-28 z-0 "></div>
            <div className=" w-40 h-40 rounded-full bg-teal-400 absolute -left-28 -bottom-28 z-0 "></div>
            <div className=" bg-white p-8 rounded-xl shadow-lg text-gray-400 relative z-10   ">
              <div className="relative z-10">
                <form className="flex flex-col space-y-4 md:w-64">
                  <div>
                    <label className="text-sm">Your Name</label>
                    <input
                      type="text"
                      className="ring-1 ring-gray-300 w-full rounded-md px-2 py-2 outline-none focus:ring-2 focus:ring-teal-200"
                      placeholder="Your Name"
                    />
                  </div>
                  <div>
                    <label className="text-sm">Email Address</label>
                    <input
                      type="email"
                      className="ring-1 ring-gray-300 w-full rounded-md px-2 py-2 outline-none focus:ring-2 focus:ring-teal-200"
                      placeholder="Email Address"
                    />
                  </div>
                  <div>
                    <label className="text-sm">Message</label>
                    <textarea
                      className="ring-1 ring-gray-300 w-full rounded-md px-2 py-2 outline-none focus:ring-2 focus:ring-teal-200"
                      rows="4"
                      placeholder="Message"
                    />
                  </div>
                  <button className="bg-cyan-700 rounded-lg text-white text-bold text-sm px-6 py-2 uppercase self-end">
                    Send Message
                  </button>
                </form>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  );
  return <div>{contactForm()}</div>;
};

export default ContactForm;

```