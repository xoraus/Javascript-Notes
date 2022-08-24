# The Complete Javascript Notes

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

# JavaScript Fundamentals Part 1

## Hello World
```js
console.log("Hello World!")
```

## A brief introduction to Javascript

_JavaScript_ was initially created to “make web pages alive”.

The programs in this language are called _scripts_. They can be written right in a web page’s HTML and run automatically as the page loads.

Scripts are provided and executed as plain text. They don’t need special preparation or compilation to run.

## Linking a JavaScript File

 ```js
let js = "amazing";
console.log(40 + 8 + 23 - 10);
```


##  Values and Variables

```js
console.log("xoraus");
console.log(23);

let firstName = "Matilda";

console.log(firstName);
console.log(firstName);
console.log(firstName);
```

## Variable name conventions

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

## Data Types

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

## Basic Operators

###### Math operators

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
###### Assignment operators

```js
let x = 10 + 5; // output: 15

x += 10; // x = x + 10 - Output: 25

x *= 4; // x = x * 4 - Output: 100

x++; // x = x + 1
x--; // x = x - 1
x--;

console.log(x);
```

###### Comparison operators

```js
console.log(ageXoraus > ageSarah); //  >, <, >=, <=
console.log(ageSarah >= 18);  // Output: true

const isFullAge = ageSarah >= 18;

console.log(now - 1991 > now - 2018);
```

## Operator Precedence

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

## Coding Challenge ##1

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

**Solution by xoraus**

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

const markHigherBMI = BMIMark > BMIJohn;

console.log(BMIMark, BMIJohn, markHigherBMI);
```

 ## Strings and Template Literals

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

## Taking Decisions: if else Statements

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

## Coding Challenge ##2

Use the BMI example from Challenge ##1, and the code you already wrote, and improve it:

1. Print a nice output to the console, saying who has the higher BMI. The message can be either "Mark's BMI is higher than John's!" or "John's BMI is higher than Mark's!"
2. Use a template literal to include the BMI values in the outputs. Example: "Mark's BMI (28.3) is higher than John's (23.9)!"

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

// console.log(`BMI of Mark is ${markBMI}`)
// console.log(`BMI of John is ${johnBMI}`)
// console.log(`Does Mark has higher BMI - ${markHigherBMI}`)

if (markBMI > johnBMI) {
  console.log(`Mark's BMI (${markBMI}) is higher than John's (${johnBMI})!`)
} else {
  console.log(`John's BMI (${johnBMI}) is higher than Marks's (${markBMI})!`)
}
```

**Another Solution**

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

## Type Conversion and Coercion
```js
// type conversion - type conversion is when we manuallyconvert from one type to another.

const inputYear = '1991';

console.log(Number(inputYear), inputYear);
console.log(Number(inputYear) + 18);

console.log(Number('xoraus')); // Outuput: NaN (Not a Number - it actually means invalid number)
console.log(typeof NaN); // output: number

console.log(String(23), 23); // String(23) is a string; 23 is a number

// type coercion - type coercion is when JavaScript automatically converts types behind the scenes for us.
// So basically, type coercion happens whenever an operator is dealing with two values that have different types.


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

## Truthy and Falsy Values

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
So in practice, the conversion to boolean is always implicit, not explicit, or in other words is always typed coercion that JavaScript does automatically behind the scenes.

But when exactly does JavaScript do type coercion to booleans? Well, it happens in two scenarios. First, when using logical operators, and Second in logical context, like for example, in the condition of an if else statement.

## Equality Operators: == vs. ===

```js
const age = '18';
if (age === 18) console.log('You just became an adult :D (strict)'); // output: true (strict equality doesn't perform type coercion)
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
So as a general rule for clean code, avoid the loose equality operator as much as you can. So when comparing values, always use strict equality with the three equal signs,

## Logical Operators

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

## Coding Challenge ##3

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

## The switch Statement
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

## Statements and Expressions
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

## The Conditional (Ternary) Operator
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
  
## Coding Challenge ##4

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

