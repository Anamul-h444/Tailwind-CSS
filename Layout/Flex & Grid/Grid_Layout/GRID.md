# Grid Layout
# Specifying the column in a grid
 grid-cols-{n} এর মাধ্যমে একটি কন্টেইনারের কন্টেন্টগুলোকে সমান সাইজের কলামে ভাগ করা যায়।  
 - প্রত্যেকটি কন্টেন্টকে বাম থেকে ডানে নিয়ে প্রথম রোতে নির্ধারিত কলাম তৈরী করবে, পরে যদি কন্টেন্ট বেশি হয় তাহলে আবার নিচের রো থেকে কলাম তৈরী করবে।
 <img src="./images/grid1.jpg"/>
 # Spanning columns
col-span-{n} এর মাধ্যমে কলামকে বৃদ্ধি করা যায়।  
 <img src="./images/grid2.jpg"/>
 # Starting and ending columns
 col-start-{n} and col-end-{n} এর মাধ্যমে কলাম এর শুরু এবং শেষ নির্ধারণ করা যায়। কলামের হিসাব শুরু হবে ১ থেকে এবং শেষ হবে শেষ নাম্বারের আগের নাম্বারে।    
 -  নিচে ১ নং কলামটি ২ নং কলাম থেকে শুরু হয়ে ২নং এ শেষ হয়েছে ফলে শুধু একটি কলামই নিয়েছে এবং ১ নং কলামটি গ্যাপ রয়ে গিয়েছে।
 - ২ নং কলামটি ঐ রো এর ১ নং কলাম থেকে শুরু হয়ে ৩ নং কলাম পর্যন্ত নিয়েছে ফলে সে দুইটি কলাম দখল করছে। 
 - ৪ নং কলামটির শেষ হবে ৪ নং কলামে, যেহেতু শুরু বলা হয়নি তাই সে শুরুর  কলামগুলো খালি রেখে ৩ নং কলামে সরে গিয়েছে।
 - ৫নং কলামটি ১ থেকে ৩ পর্যন্ত পুরো কলামটি দখল করেছে। 
  <img src="./images/grid3.jpg"/>

  # Specifying the rows in a grid
 grid-rows-{n} এর মাধ্যমে একটি কন্টেইনারের কন্টেন্টগুলোকে সমান সাইজের রোতে ভাগ করা যায়।  
 - প্রত্যেকটি কন্টেন্টকে উপর থেকে নিচে নিয়ে প্রথম কলামে নির্ধারিত রো তৈরী করবে, পরে যদি কন্টেন্ট বেশি হয় তাহলে আবার ডানের কলাম থেকে রো তৈরী করবে। অর্থাৎ সে প্রথম কলাম থেকে শুরু করবে যখন ওভারফ্লো হবে তখন ২য় কলাম থেকে শুরু হবে। যেমনঃ ৪ টি রো নির্ধারণ করার কারণে প্রথমে কলামে ৪ টি রো তৈরী হওয়ার পর ২য় কলামে ৫ থেকে রো তৈরী করছে। 

 <img src="./images/grid4.jpg"/>

 # Spanning rows
 row-span-{n} এর মাধ্যমে rows বৃদ্ধি করা যায়।    
 <img src="./images/grid5.jpg"/>

 # Starting and ending rows
 row-start-{n} and row-end-{n} এর মাধ্যমে row এর শুরু এবং শেষ নির্ধারণ করা যায়।  
 <img src="./images/grid6.jpg"/>

 # Setting the gap between elements
 ## Syntax: gap-{size}

 <img src="./images/grid7.jpg"/>


# What is item in grid layout
<img src="./images/item2.jpg"/>

 # Justify Items
 সে নির্ধারণ করে আইটেমগুলো মেইন এক্সিস তথা রো বরাবর কি কিভাবে এ্যালাইন হবে।
## justify-items-start
<img src="./images/start.jpg"/>

## justify-items-end
<img src="./images/end.jpg"/>

## justify-items-center	
<img src="./images/center.jpg"/>

## justify-items-stretch
<img src="./images/stretch.jpg"/>


# Justify Self
সে নির্ধারণ করে আইটেমগুলোর থেকে যেকোন আইটেম ব্যক্তিগতভাবে মেইন এক্সিস তথা রো বরাবর কিভাবে এ্যালাইন হবে।

## justify-self-start
<img src="./images/start1.jpg"/>

## justify-self-end
<img src="./images/end1.jpg"/>	

## justify-self-center	
<img src="./images/center1.jpg"/>

## justify-self-stretch
<img src="./images/stretch1.jpg"/>

# What is align content?
<img src="./images/content.jpg"/>

# Align Content
সে নির্ধারণ করে আইটেমগুলো ক্রস এক্সিস/কলাম বরাবর তথা উপর থেকে নিচের দিকে কিভাবে এ্যালাইন হবে। 
- কন্টেইনারের যে হাইট রয়েছে সে হাইট অনুযায়ী Statr, End, Center, Between and Evenly নির্ধারিত হয়। সুতরাং হাইট নির্ধারণ না করলে এ প্রপার্টি কাজ  করবেনা।  

## content-center
<img src="./images/2.jpg"/>

## content-start
<img src="./images/1.jpg"/>

## content-end
<img src="./images/3.jpg"/>

## content-between
<img src="./images/4.jpg"/>

## content-around
<img src="./images/5.jpg"/>

## content-evenly
<img src="./images/6.jpg"/>

# Place Content
ইহা Content কে একসাথে রো এবং কলাম বরাবর justify এবং align করে।  
## place-content-center
<img src="./images/8.jpg"/>

## place-content-start
<img src="./images/9.jpg"/>

## place-content-end
<img src="./images/10.jpg"/>

## place-content-between
<img src="./images/11.jpg"/>

## place-content-around
<img src="./images/12.jpg"/>

## place-content-evenly	
<img src="./images/13.jpg"/>

## place-content-stretch 
<img src="./images/14.jpg"/>

# Place items
ইহা items কে একসাথে রো এবং কলাম বরাবর justify এবং align করে। 
## place-items-start
<img src="./images/start3.jpg"/>

## place-items-end
<img src="./images/end3.jpg"/>

## place-items-center
<img src="./images/center3.jpg"/>

## place-items-stretch
<img src="./images/stretch3.jpg"/>

# place-self-items
ইহা item কে ব্যক্তিগতবাবে রো এবং কলাম বরাবর justify এবং align করে। 

## place-self-start	
<img src="./images/100.jpg"/>

## place-self-end
<img src="./images/102.jpg"/>

## place-self-center
<img src="./images/101.jpg"/>

## place-self-stretch
<img src="./images/103.jpg"/>
