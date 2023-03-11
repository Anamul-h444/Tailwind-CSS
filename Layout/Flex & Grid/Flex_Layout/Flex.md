# Flex Layout
## Flex Property: 
There are two kind of flex property:  
### Flex Container Property:
•	flex-direction  
•	flex-wrap  
•	flex-flow  
•	justify-content  
•	align-items  
•	align-content  
### Flex Items Property:
•	order  
•	flex-grow  
•	flex-shrink  
•	flex-basis  
•	flex  
•	align-self  

## Flexbox Axis:
1. Main-axis -> এই এক্সিস বরাবর আইটেম সমূহ মোভ করে যখন flex ঘেষণা করা হয়। বাই ডিফল্ট ইহা বাম থেকে ডানে কাজ করে।
2. Cross-axis -> এই এক্সিস বরাবর আইটেম সমূহ এ্যালাইন হয়। বাই ডিফল্ট ইহা উপর থেকে নিচের দিকে কাজ করে। 

# Flex-Direction
## flex-row	
<img src="./images/1.jpg" />

## flex-row-reverse	
<img src="./images/2.jpg" />

## flex-col	
<img src="./images/3.jpg" />

## flex-col-reverse
<img src="./images/4.jpg" />

# Flex-wrap
## flex-nowrap
<img src="./images/5.jpg" />

## flex-wrap
<img src="./images/6.jpg" />

## flex-wrap-reverse
<img src="./images/7.jpg" />

# What is content?
<img src="./images/content.jpg" />

# What is Items?
<img src="./images/items.jpg" />

# Justify content
## justify-start
<img src="./images/8.jpg" />

## justify-end	
<img src="./images/9.jpg" />

## justify-center
<img src="./images/10.jpg" />

## justify-between
<img src="./images/11.jpg" />

## justify-around
- Start point to items gap + End point to items gap == items to items gap.
<img src="./images/12.jpg" />

## justify-evenly
- Start point to items gap == End point to items gap == items to items gap.
<img src="./images/13.jpg" />

# Align Item
ইহা ক্রস এক্সিস বরাবর কাজ করে। তাই কন্টেইনারের হাইট নির্ধারণ না করলে ইহা কাজ করবেনা। কন্টেইনারের হাইটকে প্রত্যেকটি আইটেম সমান ভাবে ভাগ করে যার যার এরিয়া তৈরী করে।   
## items-start
<img src="./images/14.jpg" />	

## items-end
<img src="./images/15.jpg" />

## items-center	
<img src="./images/16.jpg" />

## items-baseline
<img src="./images/17.jpg" />

## items-stretch
<img src="./images/18.jpg" />

# Align Content
## content-center
<img src="./images/19.jpg" />

## content-start
<img src="./images/20.jpg" />

## content-end	
<img src="./images/21.jpg" />

## content-between
<img src="./images/22.jpg" />

## content-around 
- Start point to items gap + End point to items gap == items to items gap.
<img src="./images/23.jpg" />

## content-evenly 
- Start point to items gap == End point to items gap == items to items gap.
<img src="./images/24.jpg" />

# Align Self
## self-start
<img src="./images/25.jpg" />

## self-end	
<img src="./images/27.jpg" />

## self-center
<img src="./images/26.jpg" />

## self-stretch	
<img src="./images/28.jpg" />

# Grow
Grow মানে হল বৃদ্ধি হওয়া। বাই ডিফল্ট তার মান ০; অর্থাৎ সে বৃদ্ধি হবেনা। আইটেমস এর যে যে আইটেমের মধ্যে grow ব্যবহার করা হবে সে আইটেমগুলো বৃদ্ধি হয়ে  মেইন এক্সিস বরাবর কন্টেইনারের বাকি জায়গাটুকু দখল করবে।   
grow       -> 	flex-grow: 1;  
grow-0     -> 	flex-grow: 0;  

## Example
<img src="./images/29.jpg" />
<img src="./images/30.jpg" />

# Shrink
Shrink মানে হল সংকুচিত হওয়া। বাই ডিফল্ট তার মান ১; অর্থাৎ সে সংকুচিত হবে।  আইটেমস এর যে যে আইটেমের মধ্যে Shrink:০ ব্যবহার করা হবে সে আইটেমগুলো সংকুচিত হবেনা।  
shrink       ->	flex-shrink: 1;  
shrink-0    ->	flex-shrink: 0;  
## Shrink
<img src="./images/31.jpg" />

## Don't Shrink
<img src="./images/32.jpg" />

# basis
এর মাধ্যমে আইটেমের প্রাথমিক সাইজ নির্ধারণ করা হয়।
<img src="./images/33.jpg" />

# Order
এর মাধ্যমে আইটেম যে অবস্থানে থাকুক সে অবস্থান অন্যত্র তার অবস্থান নির্ণয় করা যায।
<img src="./images/34.jpg" />
