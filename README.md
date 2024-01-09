# The Complete Javascript Notes

**Course Outcome** - By the end of the course, you will have the knowledge and confidence that you need in order to ace your job interviews and become a professional developer.

### What you'll learn

- Become an advanced, confident, and modern JavaScript developer from scratch
- Build 6 beautiful real-world projects for your portfolio (not boring toy apps)
- Become job-ready by understanding how JavaScript really works behind the scenes
- How to think and work like a developer: problem-solving, researching, workflows
- JavaScript fundamentals: variables, if/else, operators, boolean logic, functions, arrays, objects, loops, strings, etc.
- Modern ES6+ from the beginning: arrow functions, destructuring, spread operator, optional chaining (ES2020), etc.
- Modern OOP: Classes, constructors, prototypal inheritance, encapsulation, etc.
- Complex concepts like the 'this' keyword, higher-order functions, closures, etc.
- Asynchronous JavaScript: Event loop, promises, async/await, AJAX calls and APIs
- How to architect your code using flowcharts and common patterns
- Modern tools for 2022 and beyond: NPM, Parcel, Babel and ES6 modules
- Practice your skills with 50+ challenges and assignments (solutions included)
- Get fast and friendly support in the Q&A area
- Course pathways: design your unique learning path according to your goals!

#### Topics Covered

1. JavaScript Fundamentals Part 1
2. JavaScript Fundamentals Part 2
3. How to Navigate This Course
4. Developer Skills & Editor Setup
5. [OPTIONAL] HTML & CSS Crash Course
6. JavaScript in the Browser: DOM and Events Fundamentals
7. How JavaScript Works Behind the Scenes
8. Data Structures, Modern Operators and Strings
9. A Closer Look at Functions
10. Working With Arrays
11. Numbers, Dates, Intl and Timers
12. Advanced DOM and Events
13. Object-Oriented Programming (O0P) With JavaScript
14. Mapty App: OOP, Geolocation, External Libraries, and More!
15. Asynchronous JavaScript: Promises, Async/Await, and AJAX
16. Modern JavaScript Development: Modules, Tooling, and Functional
17. Forkify App: Building a Modern Application
18. Setting Up Git and Deployment


## 1. JavaScript Fundamentals Part 1

### 1.  Hello World
```js
console.log("Hello World!")
```

### 2. A brief introduction to Javascript

_JavaScript_ was initially created to “make web pages alive”.

The programs in this language are called _scripts_. They can be written right in a web page’s HTML and run automatically as the page loads.

Scripts are provided and executed as plain text. They don’t need special preparation or compilation to run.

### 3. Linking a JavaScript File

 ```js
let js = "amazing";
console.log(40 + 8 + 23 - 10);
```


###  4. Values and Variables

```js
console.log("xoraus");
console.log(23);

let firstName = "Matilda";

console.log(firstName);
console.log(firstName);
console.log(firstName);
```

5. ### Variable name conventions

```js
let xoraus_matilda = "JM";
let $function = 27;

let person = "xoraus";
let PI = 3.1415;

let myFirstJob = "Coder";
let myCurrentJob = "Teacher";

let job1 = "programmer";
let job2 = "teacher";

console.log(myFirstJob);
```

### 6. Data Types

```js
let javascriptIsFun = true;
console.log(javascriptIsFun);

console.log(typeof true);
console.log(typeof javascriptIsFun);
console.log(typeof 23);
console.log(typeof 'xoraus');

javascriptIsFun = 'YES!';
console.log(typeof javascriptIsFun);

let year;

console.log(year);
console.log(typeof year);

year = 1991;

console.log(typeof year);
console.log(typeof null);  

let, const and var // us let when you're sure that the vaule will change in future

// let is block scoped
// VAR is function-scoped

let age = 30;
age = 31; // here let (age) is mutable

const birthYear = 1991; // it is immutable
birthYear = 1990;

const job; // this will throw an error;  
var job = 'programmer'; // used in legacy codebases

job = 'teacher'


lastName = 'Ahmed';
console.log(lastName);
```

### 7. Basic Operators

######### Math operators

```js
const now = 2037;
const ageXoraus = now - 1991;
const ageSarah = now - 2018;

console.log(ageXoraus, ageSarah);
console.log(ageXoraus * 2, ageXoraus 10, 2 ** 3);

// 2 ** 3 means 2 to the power of 3 = 2 * 2 * 2

const firstName = 'xoraus';
const lastName = 'Ahmed';

console.log(firstName + ' ' + lastName);
```
######### Assignment operators

```js
let x = 10 + 5; // output: 15

x += 10; // x = x + 10 - Output: 25

x *= 4; // x = x * 4 - Output: 100

x++; // x = x + 1
x--; // x = x - 1
x--;

console.log(x);
```

######### Comparison operators

```js
console.log(ageXoraus > ageSarah); //  >, <, >=, <=
console.log(ageSarah >= 18);  // Output: true

const isFullAge = ageSarah >= 18;

console.log(now - 1991 > now - 2018);
```

### 8. Operator Precedence

```js
const now = 2037;
const ageXoraus = now - 1991;
const ageSarah = now - 2018;

console.log(now - 1991 > now - 2018);

let x, y;

x = y = 25 - 10 - 5; // Output: x = y = 10, x = 10 - Assignment works from right to left

console.log(x, y);

const averageAge = (ageXoraus + ageSarah) 2;

console.log(ageXoraus, ageSarah, averageAge);
```

### 9. Coding Challenge ###1

Mark and John are trying to compare their BMI (Body Mass Index), which is calculated using the formula: BMI = mass / height ** 2 = mass / (height * height). (mass in kg and height in meter).

1. Store Mark's and John's mass and height in variables
2. Calculate both their BMIs using the formula (you can even implement both versions)
3. Create a boolean variable 'markHigherBMI' containing information about whether Mark has a higher BMI than John.

- TEST DATA 1: Marks weights 78 kg and is 1.69 m tall. John weights 92 kg and is 1.95 m tall.
- TEST DATA 2: Marks weights 95 kg and is 1.88 m tall. John weights 85 kg and is 1.76 m tall.

**My Solution**
```js
const markMass = 78;
const markHeight = 1.69;

const johnMass = 92;
const johnHeight = 1.95;

function calculateBMI(mass, height) {
	let BMI;
	BMI = mass / height ** 2;
	return BMI
}

const markBMI = calculateBMI(markMass,markHeight);
const johnBMI = calculateBMI(johnMass, johnHeight);
const markHigherBMI =  markBMI > johnBMI
console.log(markBMI)
console.log(johnBMI)
console.log(markHigherBMI)
```


 ### 10. Strings and Template Literals

```js
const firstName = 'xoraus';
const job = 'teacher';

const birthYear = 1991;
const year = 2037;

const xoraus = "I'm " + firstName + ', a ' + (year - birthYear) + ' year old ' + job + '!'; // concept of type coercion

console.log(xoraus);

const xorausNew = `I'm ${firstName}, a ${year - birthYear} year old ${job}!`; // one of most used ES6 Feature :)

console.log(xorausNew);

console.log(`Just a regular string...`);
  
console.log('String with \n\
multiple \n\
lines');

console.log(`String
multiple
lines`);
```

### 11. Taking Decisions: if else Statements

```js
const age = 15;
if (age >= 18) {
  console.log('Sarah can start driving license 🚗');
} else {
  const yearsLeft = 18 - age;
  console.log(`Sarah is too young. Wait another ${yearsLeft} years :)`);
}

const birthYear = 2012;

let century;
if (birthYear <= 2000) {
  century = 20;
} else {
  century = 21;
}
console.log(century);
```

### 12. Coding Challenge ###2

Use the BMI example from Challenge ###1, and the code you already wrote, and improve it:

1. Print a nice output to the console, saying who has the higher BMI. The message can be either "Mark's BMI is higher than John's!" or "John's BMI is higher than Mark's!"
2. Use a template literal to include the BMI values in the outputs. Example: "Mark's BMI (28.3) is higher than John's (23.9)!"

**Solution**

```js
const massMark = 78;
const heightMark = 1.69;

const massJohn = 92;
const heightJohn = 1.95;


const massMark = 95;
const heightMark = 1.88;

const massJohn = 85;
const heightJohn = 1.76;

const BMIMark = massMark heightMark ** 2;
const BMIJohn = massJohn (heightJohn * heightJohn);

console.log(BMIMark, BMIJohn);

if (BMIMark > BMIJohn) {
	console.log(`Mark's BMI (${BMIMark}) is higher than John's (${BMIJohn})!`)
} else {
	console.log(`John's BMI (${BMIJohn}) is higher than Marks's (${BMIMark})!`)
}
```

###  13. Type Conversion and Coercion
- type conversion - type conversion is when we manually convert from one type to another.
- type coercion - type coercion is when JavaScript automatically converts types behind the scenes for us.
- So basically, type coercion happens whenever an operator is dealing with two values that have different types.
```js
const inputYear = '1991';

console.log(Number(inputYear), inputYear);
console.log(Number(inputYear) + 18);

console.log(Number('xoraus')); // Outuput: NaN (Not a Number - it actually means invalid number)
console.log(typeof NaN); // output: number

console.log(String(23), 23); // String(23) is a string; 23 is a number

console.log('I am ' + 23 + ' years old'); // output: I am 23 years old. Since Javascript has type coercion, the number will be automatically be converted into string.
console.log('23' - '10' - 3); // output: Here the strings are converted to numbers because of (- minus) operator.
console.log('23' * '2'); // strings are converted to numbers
console.log('23' / '2'); // strings are converted to numbers

let n = '1' + 1; // String - '11'
n = n - 1; // String 11 will be converted to number 11 then 11 - 1 = 10

console.log(n); // 10

console.log(2+3+4+'5') // output: 95 as string ; 9 + '5' → 95
console.log('10'-'4'-'3'-2 +'5') // output: 15 as string ;  1 + '5' → 15

```

### 14. Truthy and Falsy Values

```js
// In javascript there are 5 falsy values: 0, '', undefined, null, NaN
console.log(Boolean(0)); // output: false
console.log(Boolean(undefined)); // output: false
console.log(Boolean('Jonas')); // output: true
console.log(Boolean({})); // output: true
console.log(Boolean('')); // output:  false

const money = 100;
if (money) {
  console.log("Don't spend it all ;)");
} else {
  console.log('You should get a job!');
}

let height = 0; 
if (height) { 
  console.log('YAY! Height is defined');
} else {
  console.log('Height is UNDEFINED'); // this will be the ouput because 0 is a falsy value. But this is a bug because we have defined height as 0. We can fix this using logical operators.
}
```
- So in practice, the conversion to boolean is always implicit, not explicit, or in other words is always typed coercion that JavaScript does automatically behind the scenes.
- But when exactly does JavaScript do type coercion to booleans? Well, it happens in two scenarios. First, when using logical operators, and Second in logical context, like for example, in the condition of an if else statement.

### 15. Equality Operators: == vs. ===

```js
const age = '18';
if (age === 18) console.log('You just became an adult :D (strict)'); // output: false (strict equality doesn't perform type coercion)
if (age == 18) console.log('You just became an adult :D (loose)'); // Lose equality does the type coercion therefore output: true (the string '18' will be converted to number before checking) 

const favourite = Number(prompt("What's your favourite number?"));
console.log(favourite);
console.log(typeof favourite);

if (favourite === 23) { // 22 === 23 -> FALSE
  console.log('Cool! 23 is an amzaing number!')
} else if (favourite === 7) {
  console.log('7 is also a cool number')
} else if (favourite === 9) {
  console.log('9 is also a cool number')
} else {
  console.log('Number is not 23 or 7 or 9')
}

if (favourite !== 23) console.log('Why not 23?');
```
- In case of lose equality that is `(==)` operands of different types are converted to numbers by the equality operator. An empty string, just like false, becomes a zero.
- A strict equality operator `(===)`checks the equality without type conversion.
-  So as a general rule for clean code, avoid the loose equality operator as much as you can. So when comparing values, always use strict equality with the three equal signs,

### 16. Logical Operators

```js
const hasDriversLicense = true; // A
const hasGoodVision = true; // B

console.log(hasDriversLicense && hasGoodVision); // output: true
console.log(hasDriversLicense || hasGoodVision); // output: true
console.log(!hasDriversLicense); // output: false

// if (hasDriversLicense && hasGoodVision) {
//   console.log('Sarah is able to drive!');
// } else {
//   console.log('Someone else should drive...');
// }

const isTired = false; // C
console.log(hasDriversLicense && hasGoodVision && isTired); output: false

if (hasDriversLicense && hasGoodVision && !isTired) {
  console.log('Sarah is able to drive!'); 
} else {
  console.log('Someone else should drive...');
}
// output: Sarah is able to drive! 
```

The NOT operator actually has proceedings over the OR and AND operators.

### 17. Coding Challenge ###3

There are two gymnastics teams, Dolphins and Koalas. They compete against each other 3 times. The winner with the highest average score wins the a trophy!
1. Calculate the average score for each team, using the test data below
2. Compare the team's average scores to determine the winner of the competition, and print it to the console. Don't forget that there can be a draw, so test for that as well (draw means they have the same average score).
3. BONUS 1: Include a requirement for a minimum score of 100. With this rule, a team only wins if it has a higher score than the other team, and the same time a score of at least 100 points. HINT: Use a logical operator to test for minimum score, as well as multiple else-if blocks 😉
4. BONUS 2: Minimum score also applies to a draw! So a draw only happens when both teams have the same score and both have a score greater or equal 100 points. Otherwise, no team wins the trophy.

TEST DATA: Dolphins score 96, 108 and 89. Koalas score 88, 91 and 110
TEST DATA BONUS 1: Dolphins score 97, 112 and 101. Koalas score 109, 95 and 123
TEST DATA BONUS 2: Dolphins score 97, 112 and 101. Koalas score 109, 95 and 106

**My Solution**

```js
const scoreDolphins = (96 + 108 + 89) / 3;
const scoreKoalas = (88 + 91 + 110) / 3;

console.log(scoreDolphins, scoreKoalas);

if (scoreDolphins > scoreKoalas) {
	console.log('Dolphins win the trophy 🏆');
} else if (scoreKoalas > scoreDolphins) {
	console.log('Koalas win the trophy 🏆');
} else if (scoreDolphins === scoreKoalas) {
	console.log('Both win the trophy!');
}
```

BONUS 1

```js
const scoreDolphins = (97 + 112 + 80) 3;
const scoreKoalas = (109 + 95 + 50) 3;

console.log(scoreDolphins, scoreKoalas);

if (scoreDolphins > scoreKoalas && scoreDolphins >= 100) {
	console.log('Dolphins win the trophy 🏆');
} else if (scoreKoalas > scoreDolphins && scoreKoalas >= 100) {
	console.log('Koalas win the trophy 🏆');
} else if (scoreDolphins === scoreKoalas && scoreDolphins >= 100 && scoreKoalas >= 100) {
console.log('Both win the trophy!');
} else {
console.log('No one wins the trophy 😭');
}
```

### 18. The switch Statement
```js
const day = 'friday';

switch (day) {
  case 'monday': // day === 'monday'
    console.log('Plan course structure');
    console.log('Go to coding meetup');
    break;
  case 'tuesday':
    console.log('Prepare theory videos');
    break;
  case 'wednesday':
  case 'thursday':
    console.log('Write code examples');
    break;
  case 'friday':
    console.log('Record videos');
    break;
  case 'saturday':
  case 'sunday':
    console.log('Enjoy the weekend :D');
    break;
  default:
    console.log('Not a valid day!');
}

if (day === 'monday') {
  console.log('Plan course structure');
  console.log('Go to coding meetup');
} else if (day === 'tuesday') {
  console.log('Prepare theory videos');
} else if (day === 'wednesday' || day === 'thursday') {
  console.log('Write code examples');
} else if (day === 'friday') {
  console.log('Record videos');
} else if (day === 'saturday' || day === 'sunday') {
  console.log('Enjoy the weekend :D');
} else {
  console.log('Not a valid day!');
}
```  

### 19. Statements and Expressions
```js
3 + 4 // output: 7 - an expression
1991
true && false && !false

// Following is a Statement
if (50 > 10) {
  const str = '50 is bigger';
}

const me = 'Xoraus';
console.log(`I'm ${2050 - 1997} years old ${me}`); // In javascript literals we can use expressions but not statements.
```  
- an expression is a piece of code that produces a value.
- statements are like full sentences that translate our actions.

### 20. The Conditional (Ternary) Operator
```js
const age = 23;
// age >= 18 ? console.log('I like to drink wine 🍷') : console.log('I like to drink water 💧');

const drink = age >= 18 ? 'Sharbat-e-Jaam 🍷' : 'water 💧';
console.log(drink);

let drink2;
if (age >= 18) {
  drink2 = 'Sharbat-e-Jaam 🍷';
} else {
  drink2 = 'water 💧';
}
console.log(drink2);

console.log(`I like to drink ${age >= 18 ? 'Sharbat-e-Jaam 🍷' : 'water 💧'}`);
```
  
### 21. Coding Challenge ###4

Steven wants to build a very simple tip calculator for whenever he goes eating in a restaurant. In his country, it's usual to tip 15% if the bill value is between 50 and 300. If the value is different, the tip is 20%.
1. Your task is to calculate the tip, depending on the bill value. Create a variable called 'tip' for this. It's not allowed to use an if else statement 😅 (If it's easier for you, you can start with an if else statement, and then try to convert it to a ternary operator!)
2. Print a string to the console containing the bill value, the tip, and the final value (bill + tip). Example: 'The bill was 275, the tip was 41.25, and the total value 316.25'

TEST DATA: Test for bill values 275, 40 and 430  

HINT: To calculate 20% of a value, simply multiply it by 20/100 = 0.2
HINT: Value X is between 50 and 300, if it's >= 50 && <= 300 😉

```js
const bill = 275;
const tip = (bill >= 50 && bill <= 300) ? 0.15 * bill : 0.20 * bill;

const totalValue = bill + tip;

console.log(`The bill was ${bill}, the tip was ${tip}, and the total value ${bill + tip}`);
```

## 2. JavaScript Fundamentals Part 2

### 32. Activating Strict Mode
```js
'use strict'; // to activate strict mode to 
```
- Always put strict mode in the beginning of the file
- It makes it easier for developer to avoid accidental errors.

First, strict mode forbids us to do certain things and second, it will actually create visible errors for us in certain situations in which without strict mode JavaScript will simply fail silently without letting us know that we did a mistake.
```js
'use strict';

let hasDriversLicense = false;
const passTest = true;

if (passTest) hasDriversLicense = true; // if in  hasDriver(s)License s is missing the code will behave  unexpectedly
if (hasDriversLicense) console.log('I can drive :D');

// const interface = 'Audio'; // Uncaught SyntaxError: Missing initializer in const declaration
// const private = 534; // Uncaught SyntaxError: Missing initializer in const declaration
```

### 33. Functions
```js
function logger() {
  console.log('My name is xoraus');
}

// calling / running / invoking function
logger(); // output: My name is xoraus
logger(); // output: My name is xoraus
logger(); // output: My name is xoraus

function fruitProcessor(apples, oranges) {
  const juice = `Juice with ${apples} apples and ${oranges} oranges.`;
  return juice;
}

const appleJuice = fruitProcessor(10, 5);
console.log(appleJuice);

const appleOrangeJuice = fruitProcessor(4, 8);
console.log(appleOrangeJuice);

const num = Number('6833');
```

Clean Code - **DRY Principle** that is _Don't Repeat Yourself_ 

### 34. Function Declarations vs. Expressions

```js
// Function declaration
function calcAge1(birthYeah) {
  return 2047 - birthYeah;
}
const age1 = calcAge1(1997);
// Function expression
const calcAge2 = function (birthYeah) { // Anonymous Functions - this function is an expression. Expressions produce value.
  return 2047 - birthYeah;
}
const age2 = calcAge2(1997);

console.log(age1, age2);
```
- The parameter is a kind of placeholder in the function and the argument is then the actual value that we use to fill in that placeholder that is the parameter.
- In Javascript functions are just values

#### Function Declaration
- A function declaration must have a function name.
- Function declaration does not require a variable assignment.
- These are executed before any other code.
- The function in function declaration can be accessed before and after the function
definition.
- Function declarations are hoisted
- Syntax: function foo(paramA,
paramB) { // Set of statements }

#### Function Expression
- A function Expression is similar to a function declaration without the function name.
- Function expressions can be stored in a variable assignment.
- Function expressions load and execute only when the program interpreter reaches the line of code.
- The function in function declaration can be accessed only after the function definition.
- Function expressions are not hoisted
- Syntax: const foo = function(paramA, paramB) { // Set of statements }
### 35. Arrow Functions
```js
const calcAge3 = birthYeah => 2047 - birthYeah;
const age3 = calcAge3(1997);
console.log(age3);

const yearsUntilRetirement = (birthYeah, firstName) => {
  const age = 2047 - birthYeah;
  const retirement = 65 - age;
  // return retirement;
  return `${firstName} retires in ${retirement} years`;
}

console.log(yearsUntilRetirement(1997, 'xoraus')); console.log(yearsUntilRetirement(2005, 'ahmed'));
```

### 36. Functions Calling Other Functions
```js
function cutFruitPieces(fruit) {
  return fruit * 4;
}

function fruitProcessor(apples, oranges) {
  const applePieces = cutFruitPieces(apples);
  const orangePieces = cutFruitPieces(oranges);

  const juice = `Juice with ${applePieces} piece of apple and ${orangePieces} pieces of orange.`;
  return juice;
}
console.log(fruitProcessor(2, 3));
```

- Arrow functions do not get the **this Keyword**

### 37. Reviewing Functions
```js
const calcAge = function (birthYeah) {
  return 2047 - birthYeah;
}

const yearsUntilRetirement = function (birthYeah, firstName) {
  const age = calcAge(birthYeah);
  const retirement = 65 - age;

  if (retirement > 0) {
    console.log(`${firstName} retires in ${retirement} years`);
    return retirement;
  } else {
    console.log(`${firstName} has already retired 🎉`);
    return -1;
  }
}

console.log(yearsUntilRetirement(1997, 'xoraus'));
console.log(yearsUntilRetirement(1980, 'Jordan'));
```
![[2. JavaScript Fundamentals Part 2-20220824162950.png]]

### 38. Coding Challenge 1
Back to the two gymnastics teams, the Dolphins and the Koalas! There is a new gymnastics discipline, which works differently. Each team competes 3 times, and then the average of the 3 scores is calculated (so one average score per team). A team ONLY wins if it has at least DOUBLE the average score of the other team. Otherwise, no team wins!

1. Create an arrow function 'calcAverage' to calculate the average of 3 scores
2. Use the function to calculate the average for both teams
3. Create a function 'checkWinner' that takes the average score of each team as parameters ('avgDolhins' and 'avgKoalas'), and then logs the winner to the console, together with the victory points, according to the rule above. Example: "Koalas win (30 vs. 13)".
4. Use the 'checkWinner' function to determine the winner for both DATA 1 and DATA 2.
5. Ignore draws this time.

TEST DATA 1: Dolphins score 44, 23 and 71. Koalas score 65, 54 and 49
TEST DATA 2: Dolphins score 85, 54 and 41. Koalas score 23, 34 and 27

HINT: To calculate average of 3 values, add them all together and divide by 3
HINT: To check if number A is at least double number B, check for A >= 2 * B. Apply this to the team's average scores 😉

```js
calcAverage = (scoreA, scoreB, scoreC) => (scoreA, scoreB, scoreC) / 3

const teamDolphinAvg = Math.floor(calcAverage(85,54,41));
const teamKoalaAvg = Math.floor(calcAverage(23,34,27));

console.log(teamDolphinAvg,teamKoalaAvg)

function checkWinner(teamDolphinAvg,teamKoalaAvg) {
 if (teamDolphinAvg >= 2 * teamKoalaAvg) {
	 console.log(`Dolphins win 🏆 ${teamDolphinAvg} vs ${teamKoalaAvg}`)
 } else if (teamKoalaAvg >= 2 * teamDolphinAvg) {
	 console.log(`Koalas win 🏆 ${teamKoalaAvg} vs. ${teamDolphinAvg}`)
 } else {
	 console.log(`No body won :(`)
 }
}

checkWinner(800,351)

// Test 2
scoreDolphins = calcAverage(85, 54, 41);
scoreKoalas = calcAverage(23, 34, 27);
console.log(scoreDolphins, scoreKoalas);
checkWinner(scoreDolphins, scoreKoalas);

```


### 39. Introduction to Arrays
```js
const friend1 = 'Al-Farabi';
const friend2 = 'Al-Ghazali';
const friend3 = 'Al- Razi';

const friends = ['Al-Farabi', 'Al-Ghazali', 'Al- Razi'];
console.log(friends);

const y = new Array(1991, 1984, 2008, 2020);

console.log(friends[0]); // output: Al-Farabi
console.log(friends[2]); // output: Al- Razi

console.log(friends.length); // outpt: 3
console.log(friends[friends.length - 1]); // output: Peter

friends[3] = 'Al-Qalbi';
console.log(friends); // output: Al-Farabi, Al-Ghazali, Al- Razi
// friends = ['Bob', 'Alice']

const firstName = 'Jordan';
const xoraus = [firstName, 'Ahmed', 2047 - 1997, 'teacher', friends];
console.log(xoraus);
console.log(xoraus.length);

// Exercise
const calcAge = function (birthYeah) {
  return 2047 - birthYeah;
}
const years = [1990, 1967, 2002, 2010, 2018];

const age1 = calcAge(years[0]);
const age2 = calcAge(years[1]);
const age3 = calcAge(years[years.length - 1]);
console.log(age1, age2, age3);

const ages = [calcAge(years[0]), calcAge(years[1]), calcAge(years[years.length - 1])];
console.log(ages);
```

### 40. Basic Array Operations (Methods)
```js
const friends = ['Al-Farabi', 'Al-Ghazali', 'Al- Razi'];
// const friends = ['Michael', 'Steven', 'Peter'];

// Add elements
const newLength = friends.push('xoraus');
console.log(friends);
console.log(newLength);

friends.unshift('Jordan');
console.log(friends);

// Remove elements
friends.pop(); // Last
const popped = friends.pop();
console.log(popped);
console.log(friends);

friends.shift(); // First
console.log(friends);

console.log(friends.indexOf('Al-Farabi'));
console.log(friends.indexOf('Al-Ghazali'));

friends.push(25);
console.log(friends.includes('Al- Razi'));
console.log(friends.includes('Ahmed'));
console.log(friends.includes(25));

if (friends.includes('Al-Ghazali')) {
  console.log('You have a friend called Al-Ghazali');
}
```

### 41. Coding Challenge ###2
Ahmed is still building his tip calculator, using the same rules as before: Tip 15% of the bill if the bill value is between 50 and 300, and if the value is different, the tip is 20%.

1. Write a function 'calcTip' that takes any bill value as an input and returns the corresponding tip, calculated based on the rules above (you can check out the code from first tip calculator challenge if you need to). Use the function type you like the most. Test the function using a bill value of 100.
2. And now let's use arrays! So create an array 'bills' containing the test data below.
3. Create an array 'tips' containing the tip value for each bill, calculated from the function you created before.
4. BONUS: Create an array 'total' containing the total values, so the bill + tip.

TEST DATA: 125, 555 and 44

HINT: Remember that an array needs a value in each position, and that value can actually be the returned value of a function! So you can just call a function as array values (so don't store the tip values in separate variables first, but right in the new array) 

```js
const calcTip = function (bill) {
  return bill >= 50 && bill <= 300 ? bill * 0.15 : bill * 0.2;
}
// const calcTip = bill => bill >= 50 && bill <= 300 ? bill * 0.15 : bill * 0.2;

const bills = [125, 555, 44];
const tips = [calcTip(bills[0]), calcTip(bills[1]), calcTip(bills[2])];
const totals = [bills[0] + tips[0], bills[1] + tips[1], bills[2] + tips[2]];

console.log(bills, tips, totals);
```

### 42. Introduction to Objects
```js
const xorausArray = [
  'Jordan',
  'Ahmed',
  2027 - 1997,
  'teacher',
  ['Ali', 'Khan', 'Sal']
];

const xoraus = {
  firstName: 'Jordan',
  lastName: 'Ahmed',
  age: 2027 - 1997,
  job: 'teacher',
  friends: ['Ali', 'K', 'Sal']
};
```

### 43. Dot vs. Bracket Notation
```js
const xoraus = {
  firstName: 'Jordan',
  lastName: 'Ahmed',
  age: 2027 - 1997,
  job: 'teacher',
  friends: ['Plato', 'Aristotle', 'Socrates']
};
console.log(xoraus); 

console.log(xoraus.lastName); // output: Ahmed
console.log(xoraus['lastName']); // output: Ahmed

const nameKey = 'Name';
console.log(xoraus['first' + nameKey]); // output: Jordan
console.log(xoraus['last' + nameKey]); // output: Ahmed

// console.log(xoraus.'last' + nameKey) // this will not work

const interestedIn = prompt('What do you want to know about Jordan? Choose between firstName, lastName, age, job, and friends');

if (xoraus[interestedIn]) {
  console.log(xoraus[interestedIn]);
} else {
  console.log('Wrong request! Choose between firstName, lastName, age, job, and friends');
}

xoraus.location = 'India';
xoraus['twitter'] = '@xoraus';
console.log(xoraus);

// Challenge
// "Jonas has 3 friends, and his best friend is called Aristotle"
console.log(`${xoraus.firstName} has ${xoraus.friends.length} friends, and his best friend is called ${xoraus.friends[1]}`);

```

- when we need to first compute the property name,  then we have to use the bracket notation otherwise use dot notation.
- we get **undefined ** when when we try to access a property on an object that does not exist.

### 44. Object Methods
```js
const xoraus = {
  firstName: 'Jordan',
  lastName: 'Ahmed',
  birthYeah: 1997,
  job: 'Programmer',
  friends: ['Socrates', 'Plato', 'Aristotle'],
  hasDriversLicense: true,

  // calcAge: function (birthYeah) {
  //   return 2037 - birthYeah;
  // }

  // calcAge: function () {
  //   // console.log(this);
  //   return 2027 - this.birthYeah;
  // }

  calcAge: function () {
    this.age = 2027 - this.birthYeah;
    return this.age;
  },

  getSummary: function () {
    return `${this.firstName} is a ${this.calcAge()}-year old ${xoraus.job}, and he has ${this.hasDriversLicense ? 'a' : 'no'} driver's license.`
  }
};

console.log(xoraus.calcAge());

console.log(xoraus.age);
console.log(xoraus.age);
console.log(xoraus.age);

// Challenge
// "Jonas is a 30-year old programmer, and he has a driver's license"
console.log(xoraus.getSummary());
```
- Any function that is attached to an object is called a method.

### 45. Coding Challenge ###3
Let's go back to Mark and John comparing their BMIs! This time, let's use objects to implement the calculations! Remember: BMI = mass / height ** 2 = mass / (height * height). (mass in kg and height in meter)

1. For each of them, create an object with properties for their full name, mass, and height (Mark Miller and John Smith)
2. Create a 'calcBMI' method on each object to calculate the BMI (the same method on both objects). Store the BMI value to a property, and also return it from the method.
3. Log to the console who has the higher BMI, together with the full name and the respective BMI. Example: "John Smith's BMI (28.3) is higher than Mark Miller's (23.9)!"

TEST DATA: Marks weights 78 kg and is 1.69 m tall. John weights 92 kg and is 1.95 m tall.

```js
const mark = {
  fullName: 'Mark Miller',
  mass: 78,
  height: 1.69,
  calcBMI: function () {
    this.bmi = this.mass / this.height ** 2;
    return this.bmi;
  }
};

const john = {
  fullName: 'John Smith',
  mass: 92,
  height: 1.95,
  calcBMI: function () {
    this.bmi = this.mass / this.height ** 2;
    return this.bmi;
  }
};

mark.calcBMI();
john.calcBMI();

console.log(mark.bmi, john.bmi);

// "John Smith's BMI (28.3) is higher than Mark Miller's (23.9)!"

if (mark.bmi > john.bmi) {
  console.log(`${mark.fullName}'s BMI (${mark.bmi}) is higher than ${john.fullName}'s BMI (${john.bmi})`)
} else if (john.bmi > mark.bmi) {
  console.log(`${john.fullName}'s BMI (${john.bmi}) is higher than ${mark.fullName}'s BMI (${mark.bmi})`)
}

```

### 46. Iteration: The for Loop
```js
// console.log('Lifting weights repetition 1 🏋️‍♀️');
// console.log('Lifting weights repetition 2 🏋️‍♀️');
// console.log('Lifting weights repetition 3 🏋️‍♀️');
// console.log('Lifting weights repetition 4 🏋️‍♀️');
// console.log('Lifting weights repetition 5 🏋️‍♀️');
// console.log('Lifting weights repetition 6 🏋️‍♀️');
// console.log('Lifting weights repetition 7 🏋️‍♀️');
// console.log('Lifting weights repetition 8 🏋️‍♀️');
// console.log('Lifting weights repetition 9 🏋️‍♀️');
// console.log('Lifting weights repetition 10 🏋️‍♀️');

// for loop keeps running while condition is TRUE
for (let rep = 1; rep <= 30; rep++) {
  console.log(`Lifting weights repetition ${rep} 🏋️‍♀️`);
}
```

### 47. Looping Arrays, Breaking and Continuing
```js
const jonas = [
  'Jonas',
  'Schmedtmann',
  2037 - 1991,
  'teacher',
  ['Michael', 'Peter', 'Steven'],
  true
];
const types = [];

// console.log(jonas[0])
// console.log(jonas[1])
// ...
// console.log(jonas[4])
// jonas[5] does NOT exist

for (let i = 0; i < jonas.length; i++) {
  // Reading from jonas array
  console.log(jonas[i], typeof jonas[i]);

  // Filling types array
  // types[i] = typeof jonas[i];
  types.push(typeof jonas[i]);
}

console.log(types);

const years = [1991, 2007, 1969, 2020];
const ages = [];

for (let i = 0; i < years.length; i++) {
  ages.push(2037 - years[i]);
}
console.log(ages);

// continue and break
console.log('--- ONLY STRINGS ---')
for (let i = 0; i < jonas.length; i++) {
  if (typeof jonas[i] !== 'string') continue;

  console.log(jonas[i], typeof jonas[i]);
}

console.log('--- BREAK WITH NUMBER ---')
for (let i = 0; i < jonas.length; i++) {
  if (typeof jonas[i] === 'number') break;

  console.log(jonas[i], typeof jonas[i]);
}

```

### 48. Looping Backwards and Loops in Loops
```js
const jonas = [
  'Jonas',
  'Schmedtmann',
  2037 - 1991,
  'teacher',
  ['Michael', 'Peter', 'Steven'],
  true
];

// 0, 1, ..., 4
// 4, 3, ..., 0

for (let i = jonas.length - 1; i >= 0; i--) {
  console.log(i, jonas[i]);
}

for (let exercise = 1; exercise < 4; exercise++) {
  console.log(`-------- Starting exercise ${exercise}`);

  for (let rep = 1; rep < 6; rep++) {
    console.log(`Exercise ${exercise}: Lifting weight repetition ${rep} 🏋️‍♀️`);
  }
}
```

### 49. The while Loop
```js
for (let rep = 1; rep <= 10; rep++) {
  console.log(`Lifting weights repetition ${rep} 🏋️‍♀️`);
}

let rep = 1;
while (rep <= 10) {
  // console.log(`WHILE: Lifting weights repetition ${rep} 🏋️‍♀️`);
  rep++;
}

let dice = Math.trunc(Math.random() * 6) + 1;

while (dice !== 6) {
  console.log(`You rolled a ${dice}`);
  dice = Math.trunc(Math.random() * 6) + 1;
  if (dice === 6) console.log('Loop is about to end...');
}
```

### 50. Coding Challenge ###4

Let's improve Steven's tip calculator even more, this time using loops!
1. Create an array 'bills' containing all 10 test bill values
2. Create empty arrays for the tips and the totals ('tips' and 'totals')
3. Use the 'calcTip' function we wrote before (no need to repeat) to calculate tips and total values (bill + tip) for every bill value in the bills array. Use a for loop to perform the 10 calculations!

TEST DATA: 22, 295, 176, 440, 37, 105, 10, 1100, 86 and 52

HINT: Call calcTip in the loop and use the push method to add values to the tips and totals arrays 😉

1. BONUS: Write a function 'calcAverage' which takes an array called 'arr' as an argument. This function calculates the average of all numbers in the given array. This is a DIFFICULT challenge (we haven't done this before)! Here is how to solve it:
  4.1. First, you will need to add up all values in the array. To do the addition, start by creating a variable 'sum' that starts at 0. Then loop over the array using a for loop. In each iteration, add the current value to the 'sum' variable. This way, by the end of the loop, you have all values added together
  4.2. To calculate the average, divide the sum you calculated before by the length of the array (because that's the number of elements)
  4.3. Call the function with the 'totals' array

```js
const calcTip = function (bill) {
  return bill >= 50 && bill <= 300 ? bill * 0.15 : bill * 0.2;
}
const bills = [22, 295, 176, 440, 37, 105, 10, 1100, 86, 52];
const tips = [];
const totals = [];

for (let i = 0; i < bills.length; i++) {
  const tip = calcTip(bills[i]);
  tips.push(tip);
  totals.push(tip + bills[i]);
}
console.log(bills, tips, totals);

const calcAverage = function (arr) {
  let sum = 0;
  for (let i = 0; i < arr.length; i++) {
    // sum = sum + arr[i];
    sum += arr[i];
  }
  return sum / arr.length;
}
console.log(calcAverage([2, 3, 7]));
console.log(calcAverage(totals));
console.log(calcAverage(tips));
```
## 4. Developer Skills & Editor Setup

### How to fail at learning to Code

A person named "_Noob Programmer_"

- He didn't have a clear goal at the beginning of his journey
- He started by watching courses and reading tutorials, but he would just copy the code without caring how it works. Sometimes he would just copy and paste code!
- He didn't reinforce what he was learning by doing small challenges or taking notes He didn't practice coding, and didn't come up with his own project ideas
- He quickly became frustrated when his code was not perfectly clean or efficient He lost motivation because he thought he could never know everything
- He was learning in isolation
- After finishing a couple of a courses, he thought he now was a web developer and could start applying to jobs. But he couldn't even build an app on his own!

### How to succeed at learning to Code

- He didn’t have a clear goal at the beginning of his journey
	- **FIX**
		- Set a specific, measurable, realistic and time-based goal 
		- Know exactly why you are learning to code: Switching careers? Finding a better job?
		- Imagine a big project you want to be able to build!
		- Research technologies you need and then learn them
- He would just copy the code without caring how it works. Sometimes he would just copy and paste code!
	- **FIX**
		- Understand the code that you're studying and typing 
		- Always type the code, don't copy-paste!
- He didn't reinforce what he was learning by doing small challenges or taking notes
	- **FIX**
		- After you learn a new a feature or concept, use it immediately 
		- Take notes
		-  Challenge yourself and practice with small coding exercises and challenges
		- Don't be in a hurry to complete the course fast!
- He didn't practice coding, and didn't come up with his own project ideas
	- **FIX**
		- Practicing on your own is the most important thing to do
		- This is NOT optional! Without practice outside of courses, you won't go anywhere!
		- Come up with your own project ideas or copy popular sites or applications, or just parts of them in the beginning Don't be stuck in "tutorial hell"
- He quickly became frustrated when his code was not perfectly clean or efficient
	- **FIX**
		- Don't get stuck trying to write the perfect code!
		- Just write tons of code, no matter the quality!
		- Clean and efficient code will come with time
		- You can always refactor code later
- He lost motivation because he thought he could never know everything
	- **FIX**
		- Embrace the fact that you will never you know everything
		- Just focus on what you need to achieve your goal!
- He was learning in isolation 
	- **FIX**
		- Explain new concepts to other people. If you can explain it, you truly understand it!
		- Share your goals to make yourself accountable
		- Share your learning progress with the web dev community ( ###100DaysOfCode, ###CodeNewbie, ###webdev, etc.)
- After finishing a couple of courses, he thought he now was a web developer and could start applying to jobs 
	- **FIX**
		- The biggest misconception that people have!
		- Courses are an amazing starting point, but are only the beginning of your journey!

### Learning how to code is hard, but you can do it!

![[4. Developer Skills & Editor Setup-1661521832385.jpeg]]

### How to fail at solving problems

WHENEVER JOHN ENCOUNTERS A PROBLEM:
* He jumps at the problem without much thinking 
*  He implements his solution in an unstructured way 
*  He gets stressed out when things don't work
* He is too proud to research solutions
- **FIX**
	- Stay calm and slow down, don't just jump at a problem without a plan
	-  Take a very logical and rational approach (programming is just logic, in the end...) 
	- Use my 4-step framework to solve any problem 
- Make sure you 100% understand the problem. Ask the right questions to get a clear picture of the problem
- Divide and conquer: Break a big problem into smaller sub-problems.
- Don't be afraid to do as much research as you have to
- For bigger problems, write pseudo-code before writing the actual code

### What is a software bug?

- Software bug: Defect or problem in a computer program. Basically, any unexpected or unintended behavior of a computer program is a software bug.
- Bugs are completely normal in software development!
- Debugging: Process of finding, fixing and preventing bugs.
- _Note_ - A real bug which was causing an error in Harvard's computer in the 1940s

### The Debugging Process

![[4. Developer Skills & Editor Setup-1661522068743.jpeg]]

## 5. HTML & CSS Crash Course

### Basic HTML Structure and Elements and Attributes, Classes and IDs
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />

    <link href="style.css" rel="stylesheet" />

    <title>Learning HTML & CSS</title>
  </head>
  <body>
    <h1>JavaScript is fun, but so is HTML & CSS!</h1>
    <p class="first">
      You can learn JavaScript without HTML and CSS, but for DOM manipulation
      it's useful to have some basic ideas of HTML & CSS. You can learn more
      about it
      <a href="https://www.udemy.com/user/jonasschmedtmann/">on Udemy</a>.
    </p>

    <h2>Another heading</h2>
    <p class="second">
      Just another paragraph
    </p>

    <img
      id="course-image"
      src="https://img-a.udemycdn.com/course/480x270/437398_46c3_9.jpg"
    />

    <form id="your-name">
      <h2>Your name here</h2>
      <p class="first">Please fill in this form :)</p>

      <input type="text" placeholder="Your name" />
      <button>OK!</button>
    </form>
  </body>
</html>
```

### Basic Styling with CSS &  Introduction to the CSS Box Model

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background-color: rgb(255, 247, 201);
  font-family: Arial;
  font-size: 20px;
  padding: 50px;
}

h1 {
  font-size: 35px;
  margin-bottom: 25px;
}

h2 {
  margin-bottom: 20px;
  text-align: center;
}

p {
  margin-bottom: 20px;
}

.first {
  color: red;
}

###your-name {
  background-color: rgb(255, 220, 105);
  border: 5px solid ###444;
  width: 400px;
  padding: 25px;
  margin-top: 30px;
}

input,
button {
  padding: 10px;
  font-size: 16px;
}

a {
  background-color: yellowgreen;
}

###course-image {
  width: 300px;
}

###your-name h2 {
  color: olivedrab;
}
```

## 6. JavaScript in the Browser - DOM and Events Fundamentals


###  PROJECT ### 1: Guess My Number!

```js
'use strict';

document.querySelector('.message');
console.log(document.querySelector('.message').textContent);
```

- (.) notation for classes
- (#) for selecting ids
- .textContent to select the text.

###  What's the DOM and DOM Manipulation

**DOM** - Document Object Model: Structured Representation of Html Documents. Allows Javascript to Access Html Elements and Styles to Manipulate Them. Dom Changes text, HTML attributes, and even CSS styles.

###  The DOM Tree Structure

![[6. JavaScript in the Browser - DOM and Events Fundamentals-1661525143222.jpeg]]


###  DOM !== Javascript

![[6. JavaScript in the Browser - DOM and Events Fundamentals-1661525192615.jpeg]]

###  Selecting and Manipulating Elements
```js
console.log(document.querySelector('.message').textContent);
document.querySelector('.message').textContent = '🎉 Correct Number!';

document.querySelector('.number').textContent = 13;
document.querySelector('.score').textContent = 10;

document.querySelector('.guess').value = 23; // we use ".value" to read from the input field.
console.log(document.querySelector('.guess').value);
```

###  Handling Click Events

- **Event Listener** - Now, an event is something that happens on the page. For example, a mouse click, or a mouse moving, or a key press,
- And if a function is just is value, then we can also pass it into another function as an argument.

```js
document.querySelector('.message');
console.log(document.querySelector('.message').textContent);

document.querySelector('.check').addEventListener('click', function () {
  const guess = console.log(document.querySelector('.guess').value);
  console.log(guess, typeof guess);

  if (!guess) {
    document.querySelector('.message').textContent = '🚫 No Number!';
  }
});

```

- whenever we get the user value it's in string format
- So we selected this button here using querySelector.
- And then we use the addEventListener method on that element to attach an event handler.
- And that event handler is this function here.

###  Implementing the Game Logic
```js
const secretNumber = Math.trunc(Math.random() * 20) + 1;
let score = 20;

document.querySelector('.message');
console.log(document.querySelector('.message').textContent);

document.querySelector('.check').addEventListener('click', function () {
  const guess = Number(document.querySelector('.guess').value);
  console.log(guess, typeof guess);

// When there is no input
  if (!guess) {
    document.querySelector('.message').textContent = '🚫 No Number!';
  } else if (guess === secretNumber) { // When player wins
    document.querySelector('.message').textContent = '🎉 Correct Number!';
  } else if (guess > secretNumber) { // When guess is too high
    if (score > 1) {
      document.querySelector('.message').textContent = '📈 Too high!';
      score--;
      document.querySelector('.score').textContent = score;
    } else {
      document.querySelector('.message').textContent = '💥 You lost the game!';
      document.querySelector('.score').textContent = 0;
    }
    // When guess is too low
  } else if (guess < secretNumber) {
    if (score > 1) {
      document.querySelector('.message').textContent = '📉 Too low!';
      score--;
      document.querySelector('.score').textContent = score;
    } else {
      document.querySelector('.message').textContent = '💥 You lost the game!';
      document.querySelector('.score').textContent = 0;
    }
  }
});
```
- And so it's always good to keep a variable which actually holds the data in our code and not just rely on the DOM to hold our data. And the variable can also be called a state variable Because this score is part of the so-called application state which is basically all the data that is relevant to the application.
###  Manipulating CSS Styles
```js

```

###  Coding Challenge 1
```js
'use strict';

let secretNumber = Math.trunc(Math.random() * 20) + 1;
let score = 20;
let highScore = 0;
console.log(secretNumber);
document.querySelector('.message');
console.log(document.querySelector('.message').textContent);

document.querySelector('.check').addEventListener('click', function () {
  const guess = Number(document.querySelector('.guess').value);
  console.log(guess, typeof guess);

  // When there is no input
  if (!guess) {
    document.querySelector('.message').textContent = '🚫 No Number!';
  } else if (guess === secretNumber) {
    // When player wins
    document.querySelector('.message').textContent = '🎉 Correct Number!';
    document.querySelector('.number').textContent = secretNumber;
    document.querySelector('body').style.backgroundColor = '### 60b347';
    document.querySelector('.number').style.width = '30rem';
    if (score > highScore) {
      highScore = score;
    }
  } else if (guess > secretNumber) {
    // When guess is too high
    if (score > 1) {
      document.querySelector('.message').textContent = '📈 Too high!';
      score--;
      document.querySelector('.score').textContent = score;
    } else {
      document.querySelector('.message').textContent = '💥 You lost the game!';
      document.querySelector('.score').textContent = 0;
    }
    // When guess is too low
  } else if (guess < secretNumber) {
    if (score > 1) {
      document.querySelector('.message').textContent = '📉 Too low!';
      score--;
      document.querySelector('.score').textContent = score;
    } else {
      document.querySelector('.message').textContent = '💥 You lost the game!';
      document.querySelector('.score').textContent = 0;
    }
  }
});

document.querySelector('.again').addEventListener('click', function () {
  document.querySelector('.message').textContent = 'Start Guessing';
  document.querySelector('body').style.backgroundColor = '### 222';
  document.querySelector('.number').style.width = '15rem';
  secretNumber = Math.trunc(Math.random() * 20) + 1;
  score = 20;
  document.querySelector('.score').textContent = score;
  document.querySelector('.number').textContent = '?';
  document.querySelector('.guess').value = '';
  document.querySelector('.highscore').textContent = highScore;
});

```

###  Implementing High scores

```js
if (score > highScore) {
      highScore = score;
    }
    
document.querySelector('.highscore').textContent = highScore;
```

###  Refactoring Our Code: The DRY Principle
```js
'use strict';
let secretNumber = Math.trunc(Math.random() * 20) + 1;
let score = 20;
let highscore = 0;

const displayMessage = function (message) {
  document.querySelector('.message').textContent = message;
};

document.querySelector('.check').addEventListener('click', function () {
  const guess = Number(document.querySelector('.guess').value);
  console.log(guess, typeof guess);

  // When there is no input
  if (!guess) {
    // document.querySelector('.message').textContent = '⛔️ No number!';
    displayMessage('⛔️ No number!');

    // When player wins
  } else if (guess === secretNumber) {
    // document.querySelector('.message').textContent = '🎉 Correct Number!';
    displayMessage('🎉 Correct Number!');
    document.querySelector('.number').textContent = secretNumber;

    document.querySelector('body').style.backgroundColor = '### 60b347';
    document.querySelector('.number').style.width = '30rem';

    if (score > highscore) {
      highscore = score;
      document.querySelector('.highscore').textContent = highscore;
    }

    // When guess is wrong
  } else if (guess !== secretNumber) {
    if (score > 1) {
      // document.querySelector('.message').textContent =
      // guess > secretNumber ? '📈 Too high!' : '📉 Too low!';
      displayMessage(guess > secretNumber ? '📈 Too high!' : '📉 Too low!');
      score--;
      document.querySelector('.score').textContent = score;
    } else {
      // document.querySelector('.message').textContent = '💥 You lost the game!';
      displayMessage('💥 You lost the game!');
      document.querySelector('.score').textContent = 0;
    }
  }
});

document.querySelector('.again').addEventListener('click', function () {
  score = 20;
  secretNumber = Math.trunc(Math.random() * 20) + 1;

  // document.querySelector('.message').textContent = 'Start guessing...';
  displayMessage('Start guessing...');
  document.querySelector('.score').textContent = score;
  document.querySelector('.number').textContent = '?';
  document.querySelector('.guess').value = '';

  document.querySelector('body').style.backgroundColor = '### 222';
  document.querySelector('.number').style.width = '15rem';
});
```

### ###  Guess the Number - HTML
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <link rel="stylesheet" href="style.css" />
    <title>Guess My Number!</title>
  </head>
  <body>
    <header>
      <h1>Guess My Number!</h1>
      <p class="between">(Between 1 and 20)</p>
      <button class="btn again">Again!</button>
      <div class="number">?</div>
    </header>
    <main>
      <section class="left">
        <input type="number" class="guess" />
        <button class="btn check">Check!</button>
      </section>
      <section class="right">
        <p class="message">Start guessing...</p>
        <p class="label-score">💯 Score: <span class="score">20</span></p>
        <p class="label-highscore">
          🥇 Highscore: <span class="highscore">0</span>
        </p>
      </section>
    </main>
    <script src="script.js"></script>
  </body>
</html>

```
### ###  Guess the Number - CSS
```css
@import url('https://fonts.googleapis.com/css?family=Press+Start+2P&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: inherit;
}

html {
  font-size: 62.5%;
  box-sizing: border-box;
}

body {
  font-family: 'Press Start 2P', sans-serif;
  color: ### eee;
  background-color: ### 222;
  /* background-color: ### 60b347; */
}

/* LAYOUT */
header {
  position: relative;
  height: 35vh;
  border-bottom: 7px solid ### eee;
}

main {
  height: 65vh;
  color: ### eee;
  display: flex;
  align-items: center;
  justify-content: space-around;
}

.left {
  width: 52rem;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.right {
  width: 52rem;
  font-size: 2rem;
}

/* ELEMENTS STYLE */
h1 {
  font-size: 4rem;
  text-align: center;
  position: absolute;
  width: 100%;
  top: 52%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.number {
  background: ### eee;
  color: ### 333;
  font-size: 6rem;
  width: 15rem;
  padding: 3rem 0rem;
  text-align: center;
  position: absolute;
  bottom: 0;
  left: 50%;
  transform: translate(-50%, 50%);
}

.between {
  font-size: 1.4rem;
  position: absolute;
  top: 2rem;
  right: 2rem;
}

.again {
  position: absolute;
  top: 2rem;
  left: 2rem;
}

.guess {
  background: none;
  border: 4px solid ### eee;
  font-family: inherit;
  color: inherit;
  font-size: 5rem;
  padding: 2.5rem;
  width: 25rem;
  text-align: center;
  display: block;
  margin-bottom: 3rem;
}

.btn {
  border: none;
  background-color: ### eee;
  color: ### 222;
  font-size: 2rem;
  font-family: inherit;
  padding: 2rem 3rem;
  cursor: pointer;
}

.btn:hover {
  background-color: ### ccc;
}

.message {
  margin-bottom: 8rem;
  height: 3rem;
}

.label-score {
  margin-bottom: 2rem;
}
```

###  PROJECT ### 2: Modal Window
```js
'use strict';

const modal = document.querySelector('.modal');
const overlay = document.querySelector('.overlay');
const btnCloseModal = document.querySelector('.close-modal');
const btnsOpenModal = document.querySelectorAll('.show-modal');
```

###  Working With Classes
```js
const openmodal = function () {
  console.log('Button clicked');
  modal.classList.remove('hidden');
  overlay.classList.remove('hidden');
};

for (let i = 0; i < btnsOpenModal.length; i++)
  btnsOpenModal[i].addEventListener('click', openmodal);

const CloseModal = function () {
  modal.classList.add('hidden');
  overlay.classList.add('hidden');
};

btnCloseModal.addEventListener('click', CloseModal);

overlay.addEventListener('click', CloseModal);
```
- in order to change the appearance of elements on our page. 
-  classes allow us to basically aggregate multiple CSS properties in just one, like a container.s o each class functions a bit like a container with a lot of properties in it.
- And then here, by adding and removing them, we basically can activate and deactivate certain styles, all at the same time.

###  Handling an "Esc" Keypress Event
Now, keyboard events are so-called global events because they do not happen on one specific element. And for global events like keyboard events we usually list and on the whole document.
```js
document.addEventListener('keydown', function (e) {
  //   console.log(e);
  if (e.key === 'Escape' && !modal.classList.contains('hideen')) {
    CloseModal();
  }
});
```
###  PROJECT ### 3: Pig Game
```js
'use strict';

// Selecting elements
const score0El = document.querySelector('### score--0');
const score1El = document.getElementById('score--0');
const diceEl = document.querySelector('.dice');

score0El.textContent = 0;
score1El.textContent = 0;
diceEl.classList.add('hidden');

```

###  Rolling the Dice
```js
'use strict';

// Selecting elements
const score0El = document.querySelector('### score--0');
const score1El = document.getElementById('score--1');

const current0El = document.getElementById('current--0');
const current1El = document.getElementById('current--1');

const diceEl = document.querySelector('.dice');
const btnNew = document.querySelector('.btn--new');
const btnRoll = document.querySelector('.btn--roll');
const btnHold = document.querySelector('.btn--hold');

// Starting Conditions
score0El.textContent = 0;
score1El.textContent = 0;
diceEl.classList.add('hidden');

const scores = [0, 0];
let currScore = 0;
let activePlayer = 0; // 0 - Player 1 & 1 -Player 1

btnRoll.addEventListener('click', function () {
  //1. Generate a random dice roll
  const dice = Math.trunc(Math.random() * 6) + 1;
  console.log(dice);
  //2. Diplay dice
  diceEl.classList.remove('hidden');
  diceEl.src = `dice-${dice}.png`;
  console.log(diceEl.src);

  //3.check for rolled 1
  if (dice !== 1) {
    currScore += dice;
    document.getElementById(`current--${activePlayer}`).textContent = currScore;
  } else {
    // switch to next player
     }
});

```

###  Switching the Active Player
```js
const player0El = document.querySelector('.player--0');
const player1El = document.querySelector('.player--1');

btnRoll.addEventListener('click', function () {
  //1. Generate a random dice roll
  const dice = Math.trunc(Math.random() * 6) + 1;
  //2. Diplay dice
  diceEl.classList.remove('hidden');
  diceEl.src = `dice-${dice}.png`;

  //3.check for rolled 1
  if (dice !== 1) {
    currScore += dice;
    document.getElementById(`current--${activePlayer}`).textContent = currScore;
  } else {
    // switch to next player
    document.getElementById(`current--${activePlayer}`).textContent = 0;
    currScore = 0;
    activePlayer = activePlayer === 0 ? 1 : 0;
    player0El.classList.toggle('player--active'); // Toggle will act as on off switch
    player1El.classList.toggle('player--active');
  }
});
```

###  Holding Current Score
```js
'use strict';

// Selecting elements

const player0El = document.querySelector('.player--0');
const player1El = document.querySelector('.player--1');

const score0El = document.querySelector('### score--0');
const score1El = document.getElementById('score--1');

const current0El = document.getElementById('current--0');
const current1El = document.getElementById('current--1');

const diceEl = document.querySelector('.dice');
const btnNew = document.querySelector('.btn--new');
const btnRoll = document.querySelector('.btn--roll');
const btnHold = document.querySelector('.btn--hold');

// Starting Conditions
score0El.textContent = 0;
score1El.textContent = 0;
diceEl.classList.add('hidden');

let scores = [0, 0];
let currScore = 0;
let activePlayer = 0; // 0 - Player 1 & 1 -Player 1
let playing = true;

const switchPlayer = function () {
  document.getElementById(`current--${activePlayer}`).textContent = 0;
  currScore = 0;
  activePlayer = activePlayer === 0 ? 1 : 0;
  player0El.classList.toggle('player--active');
  player1El.classList.toggle('player--active');
};

btnRoll.addEventListener('click', function () {
  if (playing) {
    //1. Generate a random dice roll
    const dice = Math.trunc(Math.random() * 6) + 1;
    //2. Diplay dice
    diceEl.classList.remove('hidden');
    diceEl.src = `dice-${dice}.png`;

    //3.check for rolled 1
    if (dice !== 1) {
      currScore += dice;
      document.getElementById(`current--${activePlayer}`).textContent =
        currScore;
    } else {
      // switch to next player
      switchPlayer();
    }
  }
});

btnHold.addEventListener('click', function () {
  if (playing) {
    scores[activePlayer] += currScore;
    document.getElementById(`score--${activePlayer}`).textContent =
      scores[activePlayer];
    // Switching Player
    if (scores[activePlayer] >= 10) {
      playing = false;
      diceEl.classList.add('hidden');
      document
        .querySelector(`.player--${activePlayer}`)
        .classList.add('player--winner');
      document
        .querySelector(`.player--${activePlayer}`)
        .classList.add('player--active');
    } else {
      switchPlayer();
    }
  }
});

```

###  Resetting the Game
```js
const init = function () {
  scores = [0, 0];
  currentScore = 0;
  activePlayer = 0;
  playing = true;

  score0El.textContent = 0;
  score1El.textContent = 0;
  current0El.textContent = 0;
  current1El.textContent = 0;

  diceEl.classList.add('hidden');
  player0El.classList.remove('player--winner');
  player1El.classList.remove('player--winner');
  player0El.classList.add('player--active');
  player1El.classList.remove('player--active');
};

btnNew.addEventListener('click', init);
```

###  Complete Code

 ### ###  HTML
```js
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <link rel="stylesheet" href="style.css" />
    <title>Pig Game</title>
  </head>
  <body>
    <main>
      <section class="player player--0 player--active">
        <h2 class="name" id="name--0">Player 1</h2>
        <p class="score" id="score--0">43</p>
        <div class="current">
          <p class="current-label">Current</p>
          <p class="current-score" id="current--0">0</p>
        </div>
      </section>
      <section class="player player--1">
        <h2 class="name" id="name--1">Player 2</h2>
        <p class="score" id="score--1">24</p>
        <div class="current">
          <p class="current-label">Current</p>
          <p class="current-score" id="current--1">0</p>
        </div>
      </section>

      <img src="dice-5.png" alt="Playing dice" class="dice" />
      <button class="btn btn--new">🔄 New game</button>
      <button class="btn btn--roll">🎲 Roll dice</button>
      <button class="btn btn--hold">📥 Hold</button>
    </main>
    <script src="script.js"></script>
  </body>
</html>

```

### ###  CSS
```JS
@import url('https://fonts.googleapis.com/css2?family=Nunito&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: inherit;
}

html {
  font-size: 62.5%;
  box-sizing: border-box;
}

body {
  font-family: 'Nunito', sans-serif;
  font-weight: 400;
  height: 100vh;
  color: ### 333;
  background-image: linear-gradient(to top left, ### 753682 0%, ### bf2e34 100%);
  display: flex;
  align-items: center;
  justify-content: center;
}

/* LAYOUT */
main {
  position: relative;
  width: 100rem;
  height: 60rem;
  background-color: rgba(255, 255, 255, 0.35);
  backdrop-filter: blur(200px);
  filter: blur();
  box-shadow: 0 3rem 5rem rgba(0, 0, 0, 0.25);
  border-radius: 9px;
  overflow: hidden;
  display: flex;
}

.player {
  flex: 50%;
  padding: 9rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  transition: all 0.75s;
}

/* ELEMENTS */
.name {
  position: relative;
  font-size: 4rem;
  text-transform: uppercase;
  letter-spacing: 1px;
  word-spacing: 2px;
  font-weight: 300;
  margin-bottom: 1rem;
}

.score {
  font-size: 8rem;
  font-weight: 300;
  color: ### c7365f;
  margin-bottom: auto;
}

.player--active {
  background-color: rgba(255, 255, 255, 0.4);
}
.player--active .name {
  font-weight: 700;
}
.player--active .score {
  font-weight: 400;
}

.player--active .current {
  opacity: 1;
}

.current {
  background-color: ### c7365f;
  opacity: 0.8;
  border-radius: 9px;
  color: ### fff;
  width: 65%;
  padding: 2rem;
  text-align: center;
  transition: all 0.75s;
}

.current-label {
  text-transform: uppercase;
  margin-bottom: 1rem;
  font-size: 1.7rem;
  color: ### ddd;
}

.current-score {
  font-size: 3.5rem;
}

/* ABSOLUTE POSITIONED ELEMENTS */
.btn {
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  color: ### 444;
  background: none;
  border: none;
  font-family: inherit;
  font-size: 1.8rem;
  text-transform: uppercase;
  cursor: pointer;
  font-weight: 400;
  transition: all 0.2s;

  background-color: white;
  background-color: rgba(255, 255, 255, 0.6);
  backdrop-filter: blur(10px);

  padding: 0.7rem 2.5rem;
  border-radius: 50rem;
  box-shadow: 0 1.75rem 3.5rem rgba(0, 0, 0, 0.1);
}

.btn::first-letter {
  font-size: 2.4rem;
  display: inline-block;
  margin-right: 0.7rem;
}

.btn--new {
  top: 4rem;
}
.btn--roll {
  top: 39.3rem;
}
.btn--hold {
  top: 46.1rem;
}

.btn:active {
  transform: translate(-50%, 3px);
  box-shadow: 0 1rem 2rem rgba(0, 0, 0, 0.15);
}

.btn:focus {
  outline: none;
}

.dice {
  position: absolute;
  left: 50%;
  top: 16.5rem;
  transform: translateX(-50%);
  height: 10rem;
  box-shadow: 0 2rem 5rem rgba(0, 0, 0, 0.2);
}

.player--winner {
  background-color: ### 2f2f2f;
}

.player--winner .name {
  font-weight: 700;
  color: ### c7365f;
}

.hidden {
  display: none;
}

```

### ###  Javascript
```js
'use strict';

// Selecting elements
const player0El = document.querySelector('.player--0');
const player1El = document.querySelector('.player--1');
const score0El = document.querySelector('### score--0');
const score1El = document.getElementById('score--1');
const current0El = document.getElementById('current--0');
const current1El = document.getElementById('current--1');

const diceEl = document.querySelector('.dice');
const btnNew = document.querySelector('.btn--new');
const btnRoll = document.querySelector('.btn--roll');
const btnHold = document.querySelector('.btn--hold');

let scores, currentScore, activePlayer, playing;

// Starting conditions
const init = function () {
  scores = [0, 0];
  currentScore = 0;
  activePlayer = 0;
  playing = true;

  score0El.textContent = 0;
  score1El.textContent = 0;
  current0El.textContent = 0;
  current1El.textContent = 0;

  diceEl.classList.add('hidden');
  player0El.classList.remove('player--winner');
  player1El.classList.remove('player--winner');
  player0El.classList.add('player--active');
  player1El.classList.remove('player--active');
};
init();

const switchPlayer = function () {
  document.getElementById(`current--${activePlayer}`).textContent = 0;
  currentScore = 0;
  activePlayer = activePlayer === 0 ? 1 : 0;
  player0El.classList.toggle('player--active');
  player1El.classList.toggle('player--active');
};

// Rolling dice functionality
btnRoll.addEventListener('click', function () {
  if (playing) {
    // 1. Generating a random dice roll
    const dice = Math.trunc(Math.random() * 6) + 1;

    // 2. Display dice
    diceEl.classList.remove('hidden');
    diceEl.src = `dice-${dice}.png`;

    // 3. Check for rolled 1
    if (dice !== 1) {
      // Add dice to current score
      currentScore += dice;
      document.getElementById(`current--${activePlayer}`).textContent =
        currentScore;
    } else {
      // Switch to next player
      switchPlayer();
    }
  }
});

btnHold.addEventListener('click', function () {
  if (playing) {
    // 1. Add current score to active player's score
    scores[activePlayer] += currentScore;
    // scores[1] = scores[1] + currentScore

    document.getElementById(`score--${activePlayer}`).textContent =
      scores[activePlayer];

    // 2. Check if player's score is >= 100
    if (scores[activePlayer] >= 100) {
      // Finish the game
      playing = false;
      diceEl.classList.add('hidden');

      document
        .querySelector(`.player--${activePlayer}`)
        .classList.add('player--winner');
      document
        .querySelector(`.player--${activePlayer}`)
        .classList.remove('player--active');
    } else {
      // Switch to the next player
      switchPlayer();
    }
  }
});

btnNew.addEventListener('click', init);
```

## 7. How JavaScript Works Behind the Scenes

### An High-Level Overview of JavaScript

###### What is Javascript?
- Javascript Is a High-Level, Object-Oriented, Multi-Paradigm Programming Language.
- Javascript Is a **High-Level** _Prototype-Based_ **Object-Oriented** Multi-Paradigm Interpreted or Just-in-Time Compiled Dynamic| Single-Threaded Garbage-Collected Programming Language With First-Class Functions and a Non-Blocking Event Loop Concurrency Model

#######  High-level
![[7. How JavaScript Works Behind the Scenes-1661664454597.jpeg]]
####### Garbage-collected
![[7. How JavaScript Works Behind the Scenes-1661664479453.jpeg]]
####### Interpreted or just-in-time compiled 
![[7. How JavaScript Works Behind the Scenes-1661664501052.jpeg]]
####### Multi-paradigm
![[7. How JavaScript Works Behind the Scenes-1661664573105.jpeg]]
####### Prototype-based object-oriented 
![[7. How JavaScript Works Behind the Scenes-1661664597254.jpeg]]
####### First-class functions
![[7. How JavaScript Works Behind the Scenes-1661664636245.jpeg]]

####### Dynamic
![[7. How JavaScript Works Behind the Scenes-1661664652377.jpeg]]

####### Single-threaded & Non-blocking event loop
![[7. How JavaScript Works Behind the Scenes-1661664673207.jpeg]]

### The JavaScript Engine and Runtime

###### What is Javascript Engine
![[7. How JavaScript Works Behind the Scenes-1661670799106.jpeg]]
- So a JavaScript engine is simply a computer program that executes JavaScript code.
- Now every browser has its own JavaScript engine but probably the most well known engine is Google's V-Eight.
- So any JavaScript engine always contains a call stack and a heap. The call stack is where our code is actually executed using something called execution contexts. Then the heap is an unstructured memory pool which stores all the objects that our application needs.
###### Compilation vs Interpretation

![[7. How JavaScript Works Behind the Scenes-1661670833417.jpeg]]


###### Just in Time Compilation of Javascript
![[7. How JavaScript Works Behind the Scenes-1661670875764.jpeg]]

###### Runtime in Browser
![[7. How JavaScript Works Behind the Scenes-1661670745908.jpeg]]

###### Runtime in NodeJs

![[7. How JavaScript Works Behind the Scenes-1661670767221.jpeg]]

### Execution Contexts and The Call Stack 
###### What is an Execution Context?
![[7. How JavaScript Works Behind the Scenes-1661673934102.jpeg]]

But now what exactly is an execution context?
Well, an execution context is an abstract concept.
But I define it basically as an environment in which a piece of JavaScript is executed. a It's like a box that stores all the necessary information for some code to be executed.
Such as local variables or arguments passed into a function.
So, JavaScript code always runs inside an execution context.

Now, in any JavaScript project, no matter how large it is, there is only ever one global execution context. It's always there as the default context, and it's where top-level code will execute.

###### Execution Context in Detail
![[7. How JavaScript Works Behind the Scenes-1661673969086.jpeg]]

Because remember each function gets its own execution context
as soon as the function is called. So basically all the variables that are somehow declared inside a function, will end up in its variable environment. However, a function can also access variables outside of the function and this works because of something called the scope chain. 

Scope chain basically consists of references to variables that are located outside of the current function. And to keep track of the scope chain, it is stored in each execution context.

Execution contexts belonging to arrow functions, do not get their own arguments keyword, nor do they get the this keyword, okay? So, basically arrow functions don't have the arguments object and the this keyword. Instead, they can use the arguments object, and the this keyword from their closest regular function parent.

###### The Call Stack
![[7. How JavaScript Works Behind the Scenes-1661674004333.jpeg]]

JavaScript has only one thread of execution. And so it can only do one thing at a time.

So like to use the analogy of the call stack being like a map for the JavaScript engine.
Because the call stack ensures that the order of execution never gets lost.
### Scope and The Scope Chain
###### Scope Concepts
- **Scoping**: How our program's variables are organized and accessed. "Where do variables live?" or "Where can we access a certain variable, and where not?",
- **Lexical scoping**: Scoping is controlled by placement of functions and blocks in the code; 
- **Scope**: Space or environment in which a certain variable is declared (variable environment in case of functions). There is global scope, function scope, and block scope; 
- **Scope of a variable**: Region of our code where a certain variable can be accessed.

###### The 3 types of Scopes
![[7. How JavaScript Works Behind the Scenes-1661745363013.jpeg]]

###### Scope Chain vs. The Call Stack
![[7. How JavaScript Works Behind the Scenes-1661745401792.jpeg]]

###### Summary
- Scoping asks the question "Where do variables live?" or "Where can we access a certain variable, and where not?";
- There are 3 types of scope in JavaScript: the global scope, scopes defined by functions, and scopes defined by blocks;
- Only let and const variables are block-scoped. Variables declared with var end up in the closest function scope;
- In JavaScript, we have lexical scoping, so the rules of where we can access variables are based on exactly where in the code functions and blocks are written;
- Every scope always has access to all the variables from all its outer scopes. This is the scope chain!
- When a variable is not in the current scope, the engine looks up in the scope chain until it finds the variable it's looking for. This is called variable lookup;
- The scope chain is a one-way street: a scope will never, ever have access to the variables of an inner scope;
- The scope chain in a certain scope is equal to adding together all the variable environments of the all parent scopes;
- The scope chain has nothing to do with the order in which functions were called. It does not affect the scope chain at all!

### Scoping in Practice
```js
function calcAge(birthYear) {
  const age = 2037 - birthYear;

  function printAge() {
    let output = `${firstName}, you are ${age}, born in ${birthYear}`;
    console.log(output); // output: firstName = Jonas → coming from global scope.

	// Block Scope
    if (birthYear >= 1981 && birthYear <= 1996) {
      var millenial = true;
      // Creating NEW variable with same name as outer scope's variable
      const firstName = 'Steven'; // firstName already declared in Global Scope

      // Reasssigning outer scope's variable
      output = 'NEW OUTPUT!'; 

      const str = `Oh, and you're a millenial, ${firstName}`; // output: Steven - This happens because Javascript tries to look the variable name in the current scope.
      console.log(str); // output: Oh, and you're a millenial, xoraus

      function add(a, b) { 
        return a + b; // The scope of this add function is only where it is defined
      }
    }
    console.log(str); // output: // str is not defined
    console.log(millenial); //output: true
    console.log(add(2, 3)); // output: add is not defined. (in strict mode)
    console.log(output); //output: NEW OUTPUT
  }
  printAge();

  return age;
}

const firstName = 'xoraus';
calcAge(1997);  // output: xoraus you are 50, born in 1997
console.log(age); // output: age is not defined 
printAge(); // output: printAge is not defined
```

- const and let variables are block scoped.
- so variables declared with the var keyword are function scoped. So they simply ignore the block, because they are not block scoped at all. They're just function scoped.
- that the scope of a variable is the entire region of the code in which the variable is accessible.
- Functions are block scoped in **Strict Mode**
- So the scope chain isn't necessary at all, if the variable that we're looking for is already in the current scope.

### Variable Environment: Hoisting and The TDZ
![[7. How JavaScript Works Behind the Scenes-1661750446465.jpeg]]
- So we learned that an execution context always contains three parts. A variable environment, the scope chain in the in current context, and the this keyword.
- So in JavaScript we have a mechanism called hoisting. And hoisting basically make some types of variables accessible, or let's say usable in the code before they are actually declared in the code. Now, many people simply define hoisting by saying that variables are magically lifted off moved to the top of their scope for example, to the top of a function. And that is actually what hoisting looks like on the surface.
- Instead, behind the scenes the code is basically scanned for variable declarations before it is executed. So this happens during the so-called creation phase of the execution context that we talked about before. Then for each variable that is found is in the code, a new property is created in a variable environment object. And that's how hoisting really works. Now, hoisting does not work the same for all variable types.
- This means that a function expression or arrow function created with var is hoisted to _undefined_. But if created with **let** or **const**, it's not usable before it's declared in a code because of the Temporal Dead Zone so again, just like normal variables. And is this is actually the reason  that we cannot use function expressions before we write them in the code, unlike function declarations.

![[7. How JavaScript Works Behind the Scenes-1661751743808.jpeg]]

- So to recap, basically each and every let and const variable get their own Temporal Dead Zone that starts at the beginning of the scope until the line where it is defined.
And the variable is only safe to use after the TDZ, so the Temporal Dead Zone.
- Alright, now what is actually the need for JavaScript to have a Temporal Dead Zone? Well, the main reason that the TDZ was introduced in ES6 is that the behavior I described before makes it way easier to avoid and catch errors. Because using a variable that is set to undefined before it's actually declared can cause serious bugs which might be hard to find.
- So accessing variables before declaration is bad practice and should be avoided. And the best way to avoid it iS by simply getting an error.
- A second and smaller reason why the TDZ exists is to make const variables actually work the way they are supposed to. So as you know, we can't reassign const variables. it So it will not be possible to set them to undefined first and then assign their real value later.
- Now, if hoisting creates so many problems, why does it exist in the first place? I get this question all the time. And so let's quickly talk about that here. So the creator of JavaScript basically implemented hoisting so that we can use function declarations before we use them. Because this is essential for some programming techniques, such as mutual recursion. Some people also think that it makes code a lot more readable. Now, the fact that it also works for var declarations is because that was the only way hoisting could be implemented at the time. So the hoisting of var variables is basically just a byproduct of hoisting functions.
###### Hoisting Example
```js
// Take a look at this code

test();
 
function test() {
  console.log("Hello");
}

// We can call the test() function before it was declared in code. That's the hoisting in practice.

// Why it's possible?

// JavaScript engine scans the code before executing it and creates a property for each variable or function in the code. For normal variables, it assigns an undefined value, and for functions it assigns a reference to that function in memory. That's why we can call a function, but if we try to access a variable, we will get undefined.

function scope() {
  console.log(var1); // undefined
  console.log(va1); // undefined
 
  var var1 = "Hello";
  var var2 = "Hi";
}
```
### Hoisting and TDZ in Practice
```js
// # Hoisting with Variables
console.log(me); // output: Undefined (because of Var)
// console.log(job); // output: Cannot access 'job' before initialization, the origin of this error is that the jobn variable is still in temporal dead zone
// console.log(year); // output: Cannot access 'year' before initialization

var me = 'Jonas';
let job = 'teacher';
const year = 1991;

// Functions
console.log(addDecl(2, 3)); //output: 5 
// console.log(addExpr(2, 3)); // output: Cannot access 'addExpr' before initialization
	console.log(addArrow); // output: Undefined
// console.log(addArrow(2, 3));

function addDecl(a, b) {
  return a + b;
}

const addExpr = function (a, b) {
  return a + b;
};

var addArrow = (a, b) => a + b;

// Example
console.log(undefined);
	if (!numProducts) deleteShoppingCart(); // output: All products deleted because at this moment the numProducts is 'Undefined' because it is declared with 'var' and that's because how the var works with hosting

var numProducts = 10;

function deleteShoppingCart() {
  console.log('All products deleted!');
}

var x = 1; // we get a property of x = 1. we cannot find y or z here in this object and that's because they were declared with let or const
let y = 2;
const z = 3;

console.log(x === window.x); // output: true
console.log(y === window.y); // output: false
console.log(z === window.z); // output: false
```

- variables declared with var, will create a property on the global window object.
And that can have some implications in some cases.

### The this Keyword
![[7. How JavaScript Works Behind the Scenes-1661754569885.jpeg]]

- Instead, if you use 'the this variable' in an arrow function, it will simply be the this keyword of the surrounding function. So of the parent function and in technical terms, this is called the 'lexical this keyword,' because it simply gets picked up from the outer lexical scope of the arrow function.
- It's also important to know what the, this keyword is not. So this will never point to the function in which we are using it. Also, the this keyword will never point to the variable environment of the function. And these are two pretty common misconceptions

### The this Keyword in Practice
```js
'use strict'
// The this Keyword in Practice
console.log(this); // output: Window Object

const calcAge = function (birthYear) {
  console.log(2037 - birthYear);
  console.log(this); // output: Undefined (in case of strict mode)
};
calcAge(1991);

const calcAgeArrow = birthYear => {
  console.log(2037 - birthYear);
  console.log(this); // output: Window (because the arrow function doesn't get the this function So instead the arrow function simply uses the lexical this keyword, which means that it uses the disc keyword of its parent function or of its parents scope.
};
calcAgeArrow(1980);

const jonas = {
  year: 1991,
  calcAge: function () {
    console.log(this); // output: jonas object - The reason that the this keyword will point to Jonas in this case is because jonas was the object calling that method
    console.log(2037 - this.year); // output: 46
  },
};
jonas.calcAge();

const matilda = {
  year: 2017,
};

matilda.calcAge = jonas.calcAge; // method borrowing 
matilda.calcAge(); // output: 20  (this will point to year: 2017) - So even though the method is written here inside of the Jonas object the this keyword will still point to Matilda. If it is Matilda, who calls the method.

const f = jonas.calcAge;
f(); // Cannot read property 'year' of undefined
```
### Regular Functions vs. Arrow Functions
```js
// Regular Functions vs. Arrow Functions
// var firstName = 'Matilda';

const jonas = {
  firstName: 'Jonas',
  year: 1991,
  calcAge: function () {
    // console.log(this);
    console.log(2037 - this.year);

    // Solution 1
    // const self = this; // self or that
    // const isMillenial = function () {
    //   console.log(self);
    //   console.log(self.year >= 1981 && self.year <= 1996);
    // };

    // Solution 2
    const isMillenial = () => {
      console.log(this);
      console.log(this.year >= 1981 && this.year <= 1996);
    };
    isMillenial(); 
  },

  greet: () => {
    console.log(this); //output: Window
    console.log(`Hey ${this.firstName}`); //output: Matilda
  },
};
jonas.greet(); // output: Hey Undefined - (using the this keyword from it's parent's this keyword)
jonas.calcAge();

// arguments keyword
const addExpr = function (a, b) {
  console.log(arguments);
  return a + b;
};
addExpr(2, 5);
addExpr(2, 5, 8, 12);

var addArrow = (a, b) => {
  console.log(arguments);
  return a + b;
};
addArrow(2, 5, 8);

```
- Now, just like the this keyword, the arguments keyword is only available in regular functions.
### Primitives vs. Objects (Primitive vs. Reference Types)
![[7. How JavaScript Works Behind the Scenes-1661760447942.jpeg]]
```js
let age = 30;
let oldAge = age;
age = 31;
console.log(age);
console.log(oldAge);

const me = {
  name: 'Jonas',
  age: 30,
};
const friend = me;
friend.age = 27;
console.log('Friend:', friend);
console.log('Me', me);
```
![[7. How JavaScript Works Behind the Scenes-1661765088951.jpeg]]

### Primitives vs. Objects in Practice
```js
// Primitive types
let lastName = 'Williams';
let oldLastName = lastName;
lastName = 'Davis';
console.log(lastName, oldLastName); // output: Davis Williams

// Reference types
const jessica = {
  firstName: 'Jessica',
  lastName: 'Williams',
  age: 27,
};
const marriedJessica = jessica;
marriedJessica.lastName = 'Davis';
console.log('Before marriage:', jessica); // output: Before marriage: { firstName: 'Jessica', lastName: 'Davis', age: 27 }
console.log('After marriage: ', marriedJessica); // output: After marriage: { firstName: 'Jessica', lastName: 'Davis', age: 27 }

// Copying objects
const jessica2 = {
  firstName: 'Jessica',
  lastName: 'Williams',
  age: 27,
  family: ['Alice', 'Bob'],
};

const jessicaCopy = Object.assign({}, jessica2);
jessicaCopy.lastName = 'Davis';

jessicaCopy.family.push('Mary');
jessicaCopy.family.push('John');

console.log('Before marriage:', jessica2); // family: [ 'Alice', 'Bob', 'Mary', 'John' ]
console.log('After marriage: ', jessicaCopy); // amily: [ 'Alice', 'Bob', 'Mary', 'John' ]
```
- And that's why we say that this object.assign only creates a shallow copy
- However, the family object is a deeply nested object. And so therefore, object.assign did not really, behind the scenes, copy it to the new object.
- Now, a deep clone is what we would need here. Usually, we do something like this  using an external library, for example, like LoDash, and this library has a ton of helpful tools and one is of them is for deep cloning.

####### Later in course
- Prototypal Inheritance Object Oriented Programming (00P) With JavaScript 
- Event Loop Asynchronous JavaScript: Promises, Async/Await and AJAX 
- How the DOM Really Works Advanced DOM and Events


