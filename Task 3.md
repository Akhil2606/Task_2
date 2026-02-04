##### &nbsp;					**Part 1 – Logical \& Ternary Operato**r





1\. Check whether a number is between 10 and 50 using logical AND.

Input: let num = 25

Output: "Valid Number" or "Invalid Number"



-->



let num = 25

if(num >=10 \&\& num<= 50){

&nbsp;	console.log("Valid Number");

} else {

&nbsp;	console.log("Invalid Number");

}



Explanation : Logical AND Operator checks all the conditions to be true. Since the given input, 25 lies between 10 and 50, it prints Valid Number.



--------------------------------------------------------------------------------------------------------------------------------------------------------------



2\. Check if a user is eligible to log in.

Condition:

username must be "admin"

password must be "1234"

Use logical AND.



-->



let username = prompt("Enter your username");

let pswd = prompt("Enter your password");



if(username === "admin" \&\& pswd === "1234"){

&nbsp;   console.log("Eligible to Login");    

} else {

&nbsp;   console.log("Unable to Login");    

}



Explanation : In the above code both username and password matches with the given input. Hence, the user is able to Login



--------------------------------------------------------------------------------------------------------------------------------------------------------------



3\. Using ternary operator:

Check if a number is even or odd.



-->



let num = 26;

let result = (num % 2 == 0) ? "Even" : "Odd";

console.log(result);



Explanation : If num%2 == 0 then, it prints as Even or else it prints Odd.



---------------------------------------------------------------------------------------------------------------------------------------------------------------



4\. What is the output?

console.log((10 === "10") || (5 > 2) \&\& !(3 < 1));

Explain step by step.



-->



Output : true

Explanation : It executes from left to right.

The 1st condition (10 === "10")has strictly equal to operator --> false

The 2nd condition (5 > 2) is absolutely correct --> true

The 3rd condition !(3 < 1) 3 is not less than 1 which is false but, ! operator reverse the output --> true

1st condition || 2nd condition \&\& 3rd condition

--> false || true \&\& false

--> true || false

--> true



---------------------------------------------------------------------------------------------------------------------------------------------------------------

---------------------------------------------------------------------------------------------------------------------------------------------------------------



##### &nbsp;					**Part 2 – Type Conversion**





5\. Find the output and explain:

console.log("5" + 2);

console.log("5" - 2);

console.log("5" \* 2);

console.log("5" / 2);



-->



Output : 52

&nbsp;	 3

&nbsp;	 10

&nbsp;	 2.5

Explanation :

("5" + 2) --> string concatenation results in string.

("5" - 2), ("5" \* 2), ("5" / 2) --> Since -, \* and / works only with numbers, JS automatically converts string into number.



--------------------------------------------------------------------------------------------------------------------------------------------------------------



6\. Convert the following using explicit conversion:

let value = "100";

\- Convert to Number

\- Convert to Boolean



-->



let value = "100";

let numvalue = Number(value);

console.log(numvalue);

console.log(typeof numvalue);



let boolvalue = Boolean(value);

console.log(boolvalue);

console.log(typeof boolvalue);



--------------------------------------------------------------------------------------------------------------------------------------------------------------



7\. What will be the output?

console.log(Boolean(""));

console.log(Boolean(" "));

console.log(Boolean(0));

console.log(Boolean(\[]));

Explain why.



-->



Output : false

&nbsp;	 true

&nbsp;	 false

&nbsp;	 true



Explanation :

Empty string → false

pace is still a value → true

0 → false

Empty array is an object → true



--------------------------------------------------------------------------------------------------------------------------------------------------------------

--------------------------------------------------------------------------------------------------------------------------------------------------------------



##### &nbsp;					**Part 3 – Conditional Statements**





8\. Write a program:

If marks >= 90 → Grade A

If marks >= 75 → Grade B

If marks >= 50 → Grade C

Else → Fail

Use if else if.



--> 



let marks = prompt("Enter your marks");

if(marks >= 90){

&nbsp;   console.log("Grade A");    

}else if(marks >= 75){

&nbsp;   console.log("Grade B");

}else if(marks >= 50){

&nbsp;   console.log("Grade C");

}else {

&nbsp;   console.log("Fail");

}



--------------------------------------------------------------------------------------------------------------------------------------------------------------



9\. Traffic Signal Program using switch case:

"red" → Stop

"yellow" → Ready

"green" → Go

Default → Invalid Signal



-->



let signal = "red";

switch(signal){

&nbsp;   case "red" :

&nbsp;       console.log("Stop"); break;

&nbsp;   case "yellow" :

&nbsp;       console.log("Ready"); break;

&nbsp;   case "green" :

&nbsp;       console.log("Go"); break;

&nbsp;   default :

&nbsp;       console.log("Invalid Signal");

}



--------------------------------------------------------------------------------------------------------------------------------------------------------------



10\. (Nested If): Check eligibility:

Age >= 18

Height >= 160

Weight >= 50

If all true → "Selected"

Else → show which condition failed.



-->



let age = prompt("Enter your age");

let height = prompt("Enter your height");

let weight = prompt("Enter your weight");



if(age >= 18){

&nbsp;   if( height >= 160){

&nbsp;       if(weight >= 50){

&nbsp;           console.log("Selected");

&nbsp;       }else{

&nbsp;           console.log("Weight is less");

&nbsp;       }

&nbsp;   }else{

&nbsp;       console.log("Height is less");        

&nbsp;   }

}else{

&nbsp;   console.log("Age is less");

}



---------------------------------------------------------------------------------------------------------------------------------------------------------------

---------------------------------------------------------------------------------------------------------------------------------------------------------------

##### &nbsp;					**Part 4 – Loops**







11\. Print numbers from 1 to 20 using for loop.



-->



for (let i = 1; i <= 20; i++){

&nbsp;   console.log(i);

}



---------------------------------------------------------------------------------------------------------------------------------------------------------------



12\. Print only odd numbers from 1 to 20.



-->



for (let i = 1; i <= 20; i++){

&nbsp;   if(i %2==1){

&nbsp;       console.log(i);

&nbsp;   }

}



---------------------------------------------------------------------------------------------------------------------------------------------------------------



13\. Using while loop:

Print numbers from 10 to 1.



-->



let i = 10;



while (i >= 1) {

&nbsp;   console.log(i);

&nbsp;   i--;

}



---------------------------------------------------------------------------------------------------------------------------------------------------------------



14\. Using do-while loop:

Print numbers from 1 to 5.



-->



let i = 1;



do {

&nbsp;   console.log(i);

&nbsp;   i++;

} while (i <= 5);



----------------------------------------------------------------------------------------------------------------------------------------------------------------



15\. Using for-of loop:

Print each character from:

let word = "STACKLY"



-->



let word = "STACKLY";



for (let char of word){

&nbsp;   console.log(char);

}



-----------------------------------------------------------------------------------------------------------------------------------------------------------------



16\. Using for-in loop:

Print both key and value from:

let student = {

name: "Arun",

course: "MERN",

duration: "6 months"



-->



let student = {

&nbsp; name: "Arun",

&nbsp; course: "MERN",

&nbsp; duration: "6 months"

};



for (let key in student) {

&nbsp; console.log(key + " : " + student\[key]);

}



------------------------------------------------------------------------------------------------------------------------------------------------------------------

------------------------------------------------------------------------------------------------------------------------------------------------------------------



##### &nbsp;					**Real-Time Questions**



RT 1. Login System

If username = "admin" AND password = "1234" → "Login Success"

Else → "Invalid Credentials"

Use logical operator + ternary.



-->



let username = prompt("Enter your username");

let password = prompt("Enter your password");



console.log(username === "admin" \&\& password === "1234" ? "Login Success" : "Invalid Credentials");



-----------------------------------------------------------------------------------------------------------------------------------------------------------------

&nbsp;

RT 2. Salary Bonus System

If employee salary > 50000 AND experience > 3 years

→ Eligible for bonus

Else → Not eligible



-->



let salary = prompt("Enter your salary");

let exp = prompt("Enter your experience");



if(salary > 50000 \&\& exp > 3){

&nbsp;       console.log("Eligible for bonus");

}else{

&nbsp;   console.log("Not Eligible");

}



-----------------------------------------------------------------------------------------------------------------------------------------------------------------



RT 3. Shopping Discount

If cart amount:

>= 5000 → 20% discount

>= 2000 → 10% discount

< 2000 → No discount

Use if-else if.



-->



let amount = prompt("Enter the cart amount");

if(amount >= 5000){

&nbsp;   console.log("20% discount");    

}else if(amount >= 2000){

&nbsp;   console.log("10% discount");

}else{

&nbsp;   console.log("No discount");

}



-----------------------------------------------------------------------------------------------------------------------------------------------------------------



RT 4. Even/Odd Counter

Count how many even numbers between 1 to 50.



-->



let count = 0;

for(let i =1; i <= 50; i++){

&nbsp;   if(i %2 === 0){

&nbsp;       count++;

&nbsp;   }

}

console.log("Even numbers :", count);



-----------------------------------------------------------------------------------------------------------------------------------------------------------------



RT 5. Dynamic Greeting System

If hour between:

1–6 → Good Morning

7–12 → Morning

13–16 → Good Afternoon

17–19 → Good Evening

Else → Good Night



-->



let hour = prompt("Enter time in hours");

if(hour >= 1 \&\& hour <= 6){

&nbsp;   console.log("Good Morning..!!");    

}else if(hour >= 7 \&\& hour <= 12){

&nbsp;   console.log("Morning");

}else if(hour >= 13 \&\& hour <= 16){

&nbsp;   console.log("Good Afternoon");    

}else if(hour >= 17 \&\& hour <= 19){

&nbsp;   console.log("Good Evening");

}else{

&nbsp;   console.log("Good Night");

}



-----------------------------------------------------------------------------------------------------------------------------------------------------------------































&nbsp;















