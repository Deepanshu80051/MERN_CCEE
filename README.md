# MERN_CCEE
## PAPER
```
🔥 Complete 40 Questions with Detailed Answers & Explanations (Hindi + English)

Q1. Which of the following tools is used to debug Node.js application?
a) JSLint
b) ESLint
c) EventEmitter
d) Node Inspector ✅
Explanation (English): Node Inspector is specifically designed for debugging Node.js applications. JSLint and ESLint are for code quality checking, EventEmitter is for handling events.
Explanation (Hindi): Node Inspector विशेष रूप से Node.js applications को debug करने के लिए बनाया गया है। JSLint और ESLint code quality check करते हैं, EventEmitter events handle करता है।

Q2. Given the following JavaScript code, what will be the output?
javascriptvar arr = [1,2,3];
var arr2 = [6,7,8];
var result = arr.concat(arr2);
console.log(result);
a) 1,2,3
b) 1,2,3,6,7,8 ✅
c) Error
d) 6,7,8
Explanation (English): concat() method merges two arrays and returns a new array with all elements combined.
Explanation (Hindi): concat() method दो arrays को merge करके एक नया array return करता है जिसमें सभी elements होते हैं।

Q3. Which jQuery function is used to prevent code from running before the document is finished loading?
a) $(document).load()
b) $(document).ready() ✅
c) $(body).load()
d) $(body).ready()
Explanation (English): $(document).ready() ensures that DOM is fully loaded before executing JavaScript code.
Explanation (Hindi): $(document).ready() यह ensure करता है कि JavaScript code execute होने से पहले DOM पूरी तरह load हो जाए।

Q4. What are the methods used to provide effects in jQuery?
a) show()
b) hide()
c) toggle()
d) All of the above ✅
Explanation (English): jQuery provides all three methods - show(), hide(), and toggle() for visual effects.
Explanation (Hindi): jQuery तीनों methods provide करता है - show(), hide(), और toggle() visual effects के लिए।

Q5. ______ is a command line tool that installs, updates or uninstalls Node.js packages in your application.
a) package-manager
b) NPM (Node Package Manager) ✅
c) REPL
d) package-installer
Explanation (English): NPM (Node Package Manager) is the official package manager for Node.js. REPL is an interactive shell.
Explanation (Hindi): NPM (Node Package Manager) Node.js का official package manager है। REPL एक interactive shell है।

Q6. What is the default ECMAScript target version used by TypeScript compiler?
a) ES3 ✅
b) ES6
c) ES2015
d) ES2016
Explanation (English): TypeScript compiler's default target is ES3 for maximum compatibility with older browsers.
Explanation (Hindi): TypeScript compiler का default target ES3 है ताकि पुराने browsers के साथ maximum compatibility मिल सके।

Q7. Where can you place the styles that are only used by a single component in Angular application?
a) In the global styles.css
b) In the app component css ✅
c) In the module
d) In the html file
Explanation (English): Component-specific styles should be placed in the component's CSS file for encapsulation.
Explanation (Hindi): Component-specific styles को component की CSS file में रखना चाहिए encapsulation के लिए।

Q8. In Angular, which decorator is used to create your own custom-defined pipe?
a) @Pipe ✅
b) @Piped
c) @PipeModule
d) @PipeClass
Explanation (English): @Pipe decorator is used to define custom pipes in Angular.
Explanation (Hindi): @Pipe decorator Angular में custom pipes बनाने के लिए use होता है।

Q9. Where can we put the JavaScript code in an HTML page?
a) In <head> section only
b) In <body> section only
c) In both <head> as well as <body> section ✅
d) None, JavaScript code can only exist in external file
Explanation (English): JavaScript can be placed in both <head> and <body> sections, or in external files.
Explanation (Hindi): JavaScript को <head> और <body> दोनों sections में रख सकते हैं, या external files में भी।

Q10. The process by which the browser decides which object to trigger event handlers is called:
a) Event Triggering
b) Event Listening
c) Event Handling
d) Event Propagation ✅
Explanation (English): Event Propagation includes bubbling and capturing phases where browser decides event flow.
Explanation (Hindi): Event Propagation में bubbling और capturing phases होते हैं जहाँ browser event flow decide करता है।

Q11. Which of the following statements is false about Node.js?
a) I/O operations are non-blocking
b) Ideal for synchronous and CPU intensive tasks ✅
c) Supports caching of modules
d) Applications can be scaled horizontally & vertically
Explanation (English): FALSE! Node.js is NOT ideal for CPU-intensive tasks. It's best for I/O operations and asynchronous tasks.
Explanation (Hindi): FALSE! Node.js CPU-intensive tasks के लिए ideal नहीं है। यह I/O operations और asynchronous tasks के लिए best है।

Q12. Which of the following is the correct code for retrieving the index of the selected option in JavaScript?
a) document.getElementsByTagName('select')
b) document.getElementById('myselect')
c) document.getElementById('myselect').selectedIndex ✅
d) document.getElementByName('myselect')
Explanation (English): You need to access the element first, then use .selectedIndex property to get the index.
Explanation (Hindi): पहले element को access करना होगा, फिर .selectedIndex property से index मिलेगा।

Q13. How many $rootScope can an Angular JS application have?
a) Zero
b) One ✅
c) Two
d) Infinite
Explanation (English): Every AngularJS application has exactly ONE $rootScope which is the parent of all scopes.
Explanation (Hindi): हर AngularJS application में सिर्फ एक ही $rootScope होता है जो सभी scopes का parent होता है।

Q14. Which of the following is a valid URL for user to get response as "Hello John"?
javascriptapp.get('/name/:name', (req,res)=>{
  res.send("Hello " + req.params.name);
});
a) localhost/john
b) localhost:4000/John
c) localhost/name=John
d) localhost:4000/name/John ✅
Explanation (English): Route is /name/:name, so URL must be localhost:4000/name/John (port + route + parameter).
Explanation (Hindi): Route /name/:name है, इसलिए URL होगा localhost:4000/name/John (port + route + parameter)।

Q15. What will be the output of the following JavaScript code?
javascriptvar num = parseInt("123abc");
a) 123 ✅
b) 123abc
c) Exception
d) NaN
Explanation (English): parseInt() parses string until it hits a non-numeric character, so it returns 123.
Explanation (Hindi): parseInt() string को parse करता है जब तक non-numeric character नहीं आता, इसलिए 123 return होगा।

Q16. Node.js is a ______ language.
a) Server Side ✅
b) Client Side
c) Immediate Side
d) Network Side
Explanation (English): Node.js is a server-side JavaScript runtime environment.
Explanation (Hindi): Node.js एक server-side JavaScript runtime environment है।

Q17. In Angular, which decorator is used to configure your module class?
a) @NgModule ✅
b) @NgConfigure
c) @NgApp
d) @NgAngular
Explanation (English): @NgModule decorator is used to define and configure Angular modules.
Explanation (Hindi): @NgModule decorator Angular modules को define और configure करने के लिए use होता है।

Q18. Which of the following can be used to convert a JSON object into a string?
a) JSON.Parse()
b) JSON.Stringify() ✅
c) JSON.NObj()
d) JSON.Objectify()
Explanation (English): JSON.stringify() converts JavaScript object to JSON string. JSON.parse() does the opposite.
Explanation (Hindi): JSON.stringify() JavaScript object को JSON string में convert करता है। JSON.parse() उल्टा काम करता है।

Q19. As the web app architecture is concerned, which type(s) of testing is/are used as integration test?
a) Component testing
b) Content testing
c) Navigation testing
d) Both B and C ✅
Explanation (English): Integration testing in web apps includes Content and Navigation testing to verify system interactions.
Explanation (Hindi): Web apps में integration testing में Content और Navigation testing शामिल होते हैं system interactions verify करने के लिए।

Q20. In Node.js the ______ class is used to create and consume custom events.
a) EventEmitter ✅
b) Events
c) NodeEvent
d) CustomEvent
Explanation (English): EventEmitter class from 'events' module is used for event-driven programming in Node.js.
Explanation (Hindi): 'events' module का EventEmitter class Node.js में event-driven programming के लिए use होता है।

Q21. What will be the return in the following JavaScript code?
javascriptfunction construct() {
  var funcs = [];
  for (var i = 0; i < 10; i++) {
    funcs.push(function() {
      return i;
    });
  }
  return funcs;
}
var funcs = construct();
funcs[5]();
a) 9
b) 0
c) 10 ✅
d) 12
Explanation (English): Closure issue! When loop ends, i=10. All functions reference the same i, so they all return 10.
Explanation (Hindi): Closure problem! जब loop end होता है, i=10 हो जाता है। सभी functions same i को reference करते हैं, इसलिए सब 10 return करेंगे।

Q22. How many callback functions can be attached to handle a request in Express?
a) Exactly One
b) Two
c) Three
d) Unlimited ✅
Explanation (English): Express allows unlimited middleware/callback functions for a single route using next().
Explanation (Hindi): Express एक route के लिए unlimited middleware/callback functions allow करता है next() use करके।

Q23. Predict the output on the console for the following JavaScript code:
javascriptlet js = "JS Program";
console.log(typeof js);
js = 5;
console.log(typeof js);
a) string number ✅
b) string string
c) null null
d) string integer
Explanation (English): First typeof returns "string", after reassignment to 5, typeof returns "number".
Explanation (Hindi): पहली बार typeof "string" return करेगा, 5 assign करने के बाद typeof "number" return करेगा।

Q24. Which of the following is a utility function in jQuery?
a) jQuery.add()
b) jQuery.parseJSON() ✅
c) jQuery.join()
d) jQuery.append()
Explanation (English): jQuery.parseJSON() is a utility function. Others are DOM manipulation methods.
Explanation (Hindi): jQuery.parseJSON() एक utility function है। बाकी DOM manipulation methods हैं।

Q25. Which HTTP method is used to update existing data?
a) GET
b) POST
c) PUT ✅
d) FETCH
Explanation (English): PUT is used to update existing resources. POST creates new, GET retrieves, PATCH does partial update.
Explanation (Hindi): PUT existing resources को update करने के लिए use होता है। POST नया बनाता है, GET retrieve करता है, PATCH partial update करता है।

Q26. What is the default Content-Type for JSON data?
a) text/json
b) application/json ✅
c) json/text
d) application/text
Explanation (English): Standard MIME type for JSON is application/json.
Explanation (Hindi): JSON के लिए standard MIME type application/json है।

Q27. Which middleware is required to access req.body in Express?
a) express.static()
b) express.json() ✅
c) express.router()
d) No middleware required
Explanation (English): express.json() middleware parses incoming JSON payloads and makes it available in req.body.
Explanation (Hindi): express.json() middleware incoming JSON payloads को parse करके req.body में available कराता है।

Q28. What does res.json() do in Express?
a) Parses JSON
b) Sends JSON response ✅
c) Reads JSON file
d) Validates JSON
Explanation (English): res.json() sends a JSON response with proper Content-Type header automatically.
Explanation (Hindi): res.json() automatically proper Content-Type header के साथ JSON response भेजता है।

Q29. Which React hook is used to manage state in function components?
a) useEffect
b) useReducer
c) useState ✅
d) useRef
Explanation (English): useState is the primary hook for managing state in React function components.
Explanation (Hindi): useState React function components में state manage करने का primary hook है।

Q30. What is JSX?
a) JavaScript XML ✅
b) Java Syntax Extension
c) JSON XML
d) JavaScript Extra
Explanation (English): JSX stands for JavaScript XML - it allows writing HTML-like syntax in JavaScript.
Explanation (Hindi): JSX का मतलब है JavaScript XML - यह JavaScript में HTML जैसा syntax लिखने की permission देता है।

Q31. Which command is used to start a React development server?
a) npm run
b) npm start ✅
c) npm serve
d) react start
Explanation (English): npm start runs the development server defined in package.json scripts.
Explanation (Hindi): npm start package.json scripts में defined development server को run करता है।

Q32. What does key prop do in React?
a) Styles elements
b) Identifies components uniquely ✅
c) Stores state
d) Binds data
Explanation (English): key prop helps React identify which items changed, added, or removed in lists.
Explanation (Hindi): key prop React को यह identify करने में help करता है कि lists में कौन से items change, add या remove हुए हैं।

Q33. Which lifecycle method is called after component is rendered (Class component)?
a) componentWillMount
b) componentDidMount ✅
c) componentWillUpdate
d) componentDidUpdate
Explanation (English): componentDidMount() is called immediately after component is mounted/rendered.
Explanation (Hindi): componentDidMount() component mount/render होने के तुरंत बाद call होता है।

Q34. What does npm init do?
a) Installs packages
b) Creates node_modules
c) Creates package.json ✅
d) Runs project
Explanation (English): npm init initializes a new Node.js project and creates package.json file.
Explanation (Hindi): npm init नया Node.js project initialize करके package.json file बनाता है।

Q35. Which of the following is NOT a valid HTTP status code?
a) 200
b) 404
c) 600 ✅
d) 500
Explanation (English): HTTP status codes range from 100-599. 600 is NOT valid.
Explanation (Hindi): HTTP status codes 100-599 की range में होते हैं। 600 valid नहीं है।

Q36. Which symbol is used to define route parameters in Express?
a) ?
b) &
c) : ✅
d) #
Explanation (English): Colon : is used for route parameters: /user/:id
Explanation (Hindi): Colon : route parameters के लिए use होता है: /user/:id

Q37. Which statement about middleware is TRUE?
a) Runs after response is sent
b) Cannot modify request
c) Has access to req, res, next ✅
d) Only one middleware allowed
Explanation (English): Middleware functions have access to request (req), response (res), and next() function.
Explanation (Hindi): Middleware functions को request (req), response (res), और next() function का access होता है।

Q38. Which hook is equivalent to lifecycle methods in React?
a) useState
b) useEffect ✅
c) useMemo
d) useCallback
Explanation (English): useEffect replaces componentDidMount, componentDidUpdate, and componentWillUnmount.
Explanation (Hindi): useEffect componentDidMount, componentDidUpdate, और componentWillUnmount को replace करता है।

Q39. Which command installs a package globally?
a) npm install
b) npm install --save
c) npm install -g ✅
d) npm global install
Explanation (English): -g flag installs packages globally: npm install -g package-name
Explanation (Hindi): -g flag packages को globally install करता है: npm install -g package-name

Q40. Which database is commonly used with MERN stack?
a) MySQL
b) PostgreSQL
c) MongoDB ✅
d) Oracle
Explanation (English): MERN = MongoDB, Express, React, Node.js
Explanation (Hindi): MERN = MongoDB, Express, React, Node.js









```
# Introduction to JavaScript
#### Key Points:

1. JavaScript ek client-side scripting language hai (browser me run hoti hai)
2. Dynamically typed language hai (variable ka type runtime pe decide hota hai)
3. Case-sensitive hai (name aur Name alag hain)
4. HTML me 3 tarike se add kar sakte hain:

* Inline: <button onclick="alert('Hi')">
* Internal: <script> tag ke andar
* External: <script src="file.js">

**MCQ Tip: JavaScript interpreted language hai, compiled nahi**

### Variables in JavaScript
https://docs.google.com/document/d/1lIqA5OEUojAbEO4AGeAFPJ46N4CEmAZxeX7xroU1hNc/edit?usp=sharing
MCQ Important:

1. var ko re-declare kar sakte ho, let aur const ko nahi
2. const me value change nahi kar sakte (but object/array ke andar change kar sakte ho)
3. Hoisting: var undefined hota hai top pe, let/const error dete hain

### Operators:
Comparison:

1. == (value check) vs === (value + type check) ⚠️ Bahut important!
2. Example: 5 == "5" → true, but 5 === "5" → false
   **MCQ Trap: == loose equality, === strict equality!**

MCQ Important:

1. var is function-scoped
2. let and const are block-scoped

### String and Method
https://docs.google.com/document/d/1lIqA5OEUojAbEO4AGeAFPJ46N4CEmAZxeX7xroU1hNc/edit?tab=t.cdplberkcm30

MCQ Trap:

1. Strings immutable hote hain (change nahi hote, naya string banta hai)
2. slice() negative index le sakta hai, substring() nahi

### Numbers & Number Methods
https://docs.google.com/document/d/1lIqA5OEUojAbEO4AGeAFPJ46N4CEmAZxeX7xroU1hNc/edit?tab=t.sxkzmsjw6kge

MCQ Important:

1. NaN == NaN → false (unique property!)
2. typeof NaN → "number"
3. Division by 0 → Infinity

### Boolean Values

Falsy Values (jo false ban jate hain):

1. false
2. 0
3. "" (empty string)
4. null
5. undefined
6. NaN
```
if(0) { }  // false
if(1) { }  // true
if("") { } // false
if("hi") { } // true
```
**MCQ Trap: Boolean("0") → true (kyunki string hai, empty nahi!)**
https://docs.google.com/document/d/1lIqA5OEUojAbEO4AGeAFPJ46N4CEmAZxeX7xroU1hNc/edit?tab=t.ncskyymerrwx

MCQ Important:

1. Month 0 se start hota hai (0=Jan, 11=Dec)
2. Day of week: 0=Sunday, 6=Saturday
   
### Array
https://docs.google.com/document/d/1lIqA5OEUojAbEO4AGeAFPJ46N4CEmAZxeX7xroU1hNc/edit?tab=t.9yghoxk703fv

MCQ Trap:

1. arr[10] = 5 karo to beech ke indices undefined ho jayenge
2. sort() by default string ki tarah sort karta hai: [1,10,2].sort() → [1,10,2]

1. for...of (arrays ke liye):
javascriptfor(let item of array) { }
2. for...in (objects ke liye):
javascriptfor(let key in object) { }

### 🔥 High-Priority MCQ Topics:
1. Type Coercion (Automatic Conversion)
```
javascript"5" + 2       // "52" (string concatenation)
"5" - 2       // 3 (number subtraction)
"5" * 2       // 10 (number multiplication)
true + 1      // 2 (true = 1, false = 0)
false + 10    // 10
"10" == 10    // true (loose equality converts)
"10" === 10   // false (strict equality)
```
**MCQ Trap: + operator string ko priority deta hai, baaki operators numbers ko!**
2. Undefined vs Null vs NaN
```
let x;           // undefined
let y = null;    // null
let z = 10/"a";  // NaN

typeof undefined  // "undefined"
typeof null       // "object" ⚠️ Important!
typeof NaN        // "number"
```
**MCQ Important: typeof null → "object" (JavaScript ki famous bug!)**

3. Hoisting (Bahut important!)
```
console.log(x);  // undefined (var hoisted with undefined)
var x = 5;

console.log(y);  // Error! (let/const in TDZ)
let y = 10;

test();  // "Hello" (function declaration hoisted)
function test() { console.log("Hello"); }
```
4. Array Tricky Questions
```
let arr = [1, 2, 3];
arr[10] = 5;
console.log(arr.length);  // 11 (not 4!)
console.log(arr[5]);      // undefined

let arr2 = [1, 10, 2, 21];
arr2.sort();  // [1, 10, 2, 21] ⚠️ String sorting!
// Correct: arr2.sort((a,b) => a-b)  // [1, 2, 10, 21]

let arr3 = [];
console.log(arr3[0]);  // undefined (not error!)
```
5. String Indexing
```
   let str = "Hello";
console.log(str[0]);     // "H"
console.log(str[10]);    // undefined (no error!)
**str[0] = "h";            // No effect! (strings immutable)⚠️**
console.log(str);        // "Hello"

"Hello"[1]               // "e"
"Hello".charAt(1)        // "e"
```
7. Truthy/Falsy Tricky Cases
```
Boolean(0)        // false
Boolean("0")      // true ⚠️ (string hai!)
Boolean("")       // false
Boolean(" ")      // true ⚠️ (space hai!)
Boolean([])       // true ⚠️ (empty array bhi!)
Boolean({})       // true ⚠️ (empty object bhi!)

if([]) { }        // Ye run hoga! (truthy)
if("") { }        // Ye nahi (falsy)
```
**MCQ Trap: Empty array/object bhi truthy hote hain!**
8. Variable Declaration Without Keyword
```
x = 10;  // Global variable ban jata hai (strict mode me error)
console.log(x);  // 10

function test() {
    y = 20;  // Ye bhi global!
}
test();
console.log(y);  // 20
```
**MCQ Important: var/let/const ke bina declare karoge to global ban jata hai!**
9. Loop me var vs let
```
// var ke saath:
for(var i=0; i<3; i++) {
    setTimeout(() => console.log(i), 100);
}
// Output: 3 3 3 ⚠️ (sab me last value)

// let ke saath:
for(let i=0; i<3; i++) {
    setTimeout(() => console.log(i), 100);
}
// Output: 0 1 2 ✅ (separate copy)
```
10. Array/String Length
```
let arr = [1, 2, 3];
arr.length = 2;
console.log(arr);  // [1, 2] ⚠️ (truncate ho gaya!)

let str = "Hello";
str.length = 2;    // No effect (immutable)
console.log(str);  // "Hello"
```
**MCQ Trap: Array ka length writeable hai, string ka nahi!**
11. Comparison Tricky Cases
```
null == undefined      // true ⚠️
null === undefined     // false

0 == false            // true
0 === false           // false

"" == false           // true
"" === false          // false

NaN == NaN            // false ⚠️
NaN === NaN           // false

[] == false           // true ⚠️
[] === false          // false
```
13. Function Declarations vs Expressions
```
// Declaration (hoisted):
test1();  // Works!
function test1() { console.log("Hi"); }

// Expression (not hoisted):
test2();  // Error!
var test2 = function() { console.log("Hi"); };
```
14. Pass by Value vs Reference
```
// Primitives (pass by value):
let a = 10;
let b = a;
b = 20;
console.log(a);  // 10 (unchanged)

// Objects/Arrays (pass by reference):
let arr1 = [1, 2];
let arr2 = arr1;
arr2.push(3);
console.log(arr1);  // [1, 2, 3] ⚠️ (changed!)
```
* ⚠️
```
  "Hello"[10]       // undefined
"Hello".charAt(10) // "" (empty string)
"Hello".slice(-2)  // "lo" (last 2)
[1,2,3].indexOf(4)  // -1 (not undefined!)
"Hello".indexOf("z") // -1
[1,2] + [3,4]  // "1,23,4" (strings!)

* console.log([] == ![]);  // true ⚠️
Step by step:
![] → false (empty array truthy hai)
[] == false
"" == false (array to string conversion)
0 == 0 → true

console.log([] == []);  // false
console.log("5" - "2");  // 3
console.log("5" * "2");  // 10
console.log(+"5" + +"3");  // 8
console.log(!!"false");  // true
console.log(Number(""));  // 0
console.log("Hello".substring(-2));  // "Hello" substring() negative values ko 0 treat karta hai!
slice() negative support karta hai, substring() nahi.

let arr = [1, 2, 3];
delete arr[1];
console.log(arr.length);  // 3 delete element remove karta hai but length same rehti hai!
let arr = [1, 2, 3];
delete arr[1];
console.log(arr[1]);  // undefined delete us position ko undefined kar deta hai!
console.log([1, 2, 3].join());  // "1,2,3" join() default separator comma (,) hai!
let arr = [1, 2, 3];
for(let i in arr) {
    console.log(typeof i);  // "string"
}
for...in indices ko string me return karta hai! ⚠️
```
🎯 Weak Areas Identified:
1. Advanced Type Coercion (Major Issue!)

* [] == ![] → true
* "5" - "2" → 3
* Number("") → 0
* !!"false" → true

Practice Needed: 30 minutes daily on type conversion

2. Array Methods Edge Cases

* delete operator behavior
* join() default separator
* slice() negative indices
* for...in returns strings


3. Hoisting (Still Confusion)

* Function inside function hoisting
* typeof function


4. Loops

* for...in vs for...of
* Nested loop counting

### 💡 Quick Revision Sheet:
```
// Addition (+) prefers strings
"5" + 2 → "52"

// Other operators prefer numbers
"5" - 2 → 3
"5" * 2 → 10
"5" / 2 → 2.5

// Special conversions
Number("") → 0
Number("hello") → NaN
Boolean("0") → true (non-empty string!)
delete arr[1]        // Creates undefined, length same
arr.join()           // Default separator: ","
arr.slice(1, -1)     // Negative = from end
for(let i in arr)    // Returns indices as STRINGS
for(let val of arr)  // Returns VALUES
```
## Objects & Object Properties
Object Creation:-
```
// 3 ways to create objects:

// 1. Object Literal
let obj1 = { name: "Raj", age: 25 };

// 2. new Object()
let obj2 = new Object();
obj2.name = "Raj";

// 3. Object.create()
let obj3 = Object.create(null);

let person = { name: "Raj", age: 25 };


```
Accessing Properties: :-
```
// Dot notation
console.log(person.name);  // "Raj"

// Bracket notation (useful for dynamic keys)
console.log(person["age"]);  // 25

let key = "name";
console.log(person[key]);  // "Raj"
```
Adding/Deleting Properties:
```
let obj = { a: 1 };

obj.b = 2;           // Add property
delete obj.a;        // Delete property
console.log(obj);    // { b: 2 }
```
Important Object Methods:

https://docs.google.com/document/d/1lIqA5OEUojAbEO4AGeAFPJ46N4CEmAZxeX7xroU1hNc/edit?tab=t.ylaxipxyb9bq

MCQ Important:

1. Dot notation me space/special characters allowed nahi
2. delete operator property remove karta hai
3. Object.keys() returns array, not object

## Object Methods & Prototypes
💡 Arrow functions me this nahi hota:
```
let obj = {
    name: "Raj",
    show: () => {
        console.log(this.name);  // undefined (no 'this' binding)
    }
};
```
```
let person = {
    name: "Raj",
    age: 25,
    greet: function() {
        console.log("Hello " + this.name);
    }
};

person.greet();  // "Hello Raj"
```
Prototype:

1. Har object ka ek prototype hota hai
2. Prototype se properties/methods inherit hoti hain
3. MCQ Important:
* __proto__ object ka prototype point karta hai
* Arrow functions me this binding nahi hoti -- undefined deta hu
* All objects inherit from Object.prototype

## D. Closures (BAHUT IMPORTANT!)
Closure: Function jo apne outer function ke variables ko remember kar sakta hai.
```
function outer() {
    let count = 0;
    
    function inner() {
        count++;
        console.log(count);
    }
    
    return inner;
}

let counter = outer();
counter();  // 1
counter();  // 2
counter();  // 3
```
MCQ Important:

1. Closure = function + lexical environment
2. Inner function outer variables ko access kar sakta hai
3. Private variables banane ke liye use hota hai

💡 new keyword kya karta hai:

1. Empty object create karta hai
2. this ko us object se bind karta hai
3. Object return karta ha

MCQ Important:

1. sort() default string sort karta hai
2. Number sorting: (a, b) => a - b
3. Bubble/Selection/Insertion: O(n²)
4. Quick/Merge: O(n log n)
5. Every object has __proto__
6. Encapsulation: Private fields #
7. Inheritance: extends, super()
### MCQ

1.let arr = [1, 2, 3];
console.log(arr.__proto__ === Array.prototype);   // true

JavaScript Revision Notes - Topic-wise Priority
```
🔴 Priority 1: THIS BINDING & CONTEXT (Sabse Important)
Q10: Arrow Function aur this
Tumhara Answer: c (Error)
Sahi Answer: b (undefined)
Concept:
javascriptlet obj = {
    name: "Raj",
    greet: () => {
        console.log(this.name);  // undefined
    }
};
obj.greet();
Yaad Rakhne Wale Points:

✅ Arrow functions apna this nahi banate
✅ Arrow function parent scope ka this use karta hai
✅ Object literal mein arrow function = global this
✅ Global scope mein this.name = undefined
❌ Regular function: obj ka this use karta

Rule: Object methods ke liye KABHI arrow function mat use karo!

Q14: Function Context Loss
Tumhara Answer: a (10)
Sahi Answer: b (undefined)
Concept:
javascriptlet obj = {
    value: 10,
    getValue: function() {
        return this.value;
    }
};
let getValue = obj.getValue;  // Function reference copy
console.log(getValue());  // undefined - context lost!
Yaad Rakhne Wale Points:

✅ Function ko variable mein assign karne se this kho jata hai
✅ obj.getValue aur getValue different hai
✅ Direct call: this = global object (strict mode mein undefined)
✅ Fix: getValue.call(obj) ya obj.getValue.bind(obj)

Rule: Function reference copy karne se context lost hota hai!

🔴 Priority 2: AUTOMATIC SEMICOLON INSERTION (ASI)
Q24: Return Statement Ka Trap
Tumhara Answer: a ({ value: 10 })
Sahi Answer: b (undefined)
Concept:
javascriptfunction test() {
    return        // ← JavaScript yahan semicolon add kar deta hai!
    {
        value: 10
    };
}
console.log(test());  // undefined
Yaad Rakhne Wale Points:

✅ return ke baad new line = automatic semicolon
✅ JavaScript reads: return; (undefined)
✅ Object baad mein unreachable code ban jata hai
✅ Fix: return { same line pe likho

Sahi Tarika:
javascriptfunction test() {
    return {  // Same line pe start karo!
        value: 10
    };
}
Rule: Return statement aur opening brace { same line pe!

🟡 Priority 3: CONSTRUCTOR FUNCTIONS
Q26: Constructor Without new
Tumhara Answer: d (Person object)
Sahi Answer: b (undefined)
Concept:
javascriptfunction Person(name) {
    this.name = name;
}
let p1 = Person("Raj");  // `new` bhool gaye!
console.log(p1);  // undefined
Yaad Rakhne Wale Points:

✅ new ke bina: function normally execute hota hai
✅ Return statement nahi = undefined return
✅ this global object ko point karta (window.name = "Raj")
✅ Object nahi banta

What happens:

Without new: this = global, returns undefined
With new: this = new object, returns that object

Rule: Constructor function HAMESHA new ke saath call karo!

🟡 Priority 4: PRIVATE FIELDS & PROTOTYPES
Q31: Prototype Method Sharing
Tumhara Answer: b (false)
Sahi Answer: a (true)
Concept:
javascriptfunction Person(name) {
    this.name = name;
}
Person.prototype.greet = function() {
    console.log("Hello " + this.name);
};
let p1 = new Person("Raj");
let p2 = new Person("Priya");
console.log(p1.greet === p2.greet);  // true!
Yaad Rakhne Wale Points:

✅ Prototype method SAME reference hota hai
✅ Dono instances same function share karte hain
✅ Memory efficient - ek hi function copy
✅ Method prototype pe store hota, instance pe nahi

Rule: Prototype methods = shared across all instances!

Q32: Private Class Fields
Tumhara Answer: b (undefined)
Sahi Answer: c (Error)
Concept:
javascriptclass BankAccount {
    #balance = 1000;  // Private field (#)
    
    getBalance() {
        return this.#balance;  // OK - inside class
    }
}
let acc = new BankAccount();
console.log(acc.#balance);  // Error! Can't access outside
Yaad Rakhne Wale Points:

✅ # = Private field (ES2022)
✅ Class ke bahar access = SyntaxError
✅ Undefined nahi, direct ERROR throw hota hai
✅ Only class methods can access private fields

Rule: Private fields (#) class ke bahar accessible nahi!

🟢 Priority 5: ARRAY SORTING
Q33: Default Sort Behavior
Tumhara Answer: c ([10, 5, 20, 15])
Sahi Answer: b ([10, 15, 20, 5])
Concept:
javascriptlet arr = [10, 5, 20, 15];
arr.sort();  // NO comparator!
console.log(arr);  // [10, 15, 20, 5]
Yaad Rakhne Wale Points:

✅ Default sort = LEXICOGRAPHIC (string sorting)
✅ Numbers ko strings mein convert karta hai
✅ "10" < "15" < "20" < "5" (string comparison)
✅ Numeric sort ke liye comparator chahiye

Sahi Tarika:
javascriptarr.sort((a, b) => a - b);  // Numeric sort
Rule: Numbers sort karne ke liye HAMESHA comparator do!

Q36: String Sorting
Tumhara Answer: a ("banana")
Sahi Answer: b ("apple")
Concept:
javascriptlet arr = ["banana", "apple", "cherry"];
arr.sort();
console.log(arr[0]);  // "apple"
// Sorted: ["apple", "banana", "cherry"]
Yaad Rakhne Wale Points:

✅ Strings alphabetically sort hote hain
✅ Case-sensitive: uppercase < lowercase
✅ "apple" alphabetically pehle aata hai


Q37: Bubble Sort Complexity
Tumhara Answer: a (O(n))
Sahi Answer: c (O(n²))
Yaad Rakhne Wale Points:

✅ Bubble Sort worst case = O(n²)
✅ Nested loops = n × n
✅ Best case (sorted): O(n)
✅ Average case: O(n²)


Q39: Sort with Zero Comparator
Tumhara Answer: a ([3, 1, 4, 1, 5])
Sahi Answer: c (Order may vary)
Concept:
javascriptlet arr = [3, 1, 4, 1, 5];
arr.sort((a, b) => {
    return 0;  // All elements equal!
});
console.log(arr);  // Implementation dependent
Yaad Rakhne Wale Points:

✅ Return 0 = elements equal
✅ JavaScript sort is NOT STABLE in all browsers
✅ Order implementation-dependent
✅ Original order maintain nahi hota guaranteed

Rule: Sort stability pe depend mat karo!

📊 Quick Revision Checklist
THIS Binding (Most Important!)

 Regular function: dynamic this
 Arrow function: lexical this (parent scope)
 Method call: obj.method() → this = obj
 Function copy: context lost
 call/apply/bind: manual this binding

Common Traps

 Return + newline = ASI (auto semicolon)
 Constructor without new = undefined
 Private fields (#) = Error outside class
 Default sort = lexicographic (string sort)
 Prototype methods = shared reference

Memory Tips
🎯 Arrow Function: "Arrow kabhi apna THIS nahi banata"
🎯 Return Statement: "Return aur { ek hi line pe"
🎯 Constructor: "NEW bhool gaye toh UNDEFINED milega"
🎯 Sort: "Numbers ko comparator chahiye"
🎯 Private Field: "Hash (#) class ke bahar ERROR"
```

## DOM
Exam Confusion Points:

1. ✅ getElementById → NO 's' in element
2. ✅ getElementsByClassName → HAS 's' in elements
3. ✅ HTMLCollection = LIVE (auto updates)
4. ✅ NodeList (querySelectorAll) = STATIC
5. ✅ querySelector returns FIRST match only
```
Q: What's the difference?
let p = document.createElement('p');
p.textContent = '<b>Hi</b>';  // → Shows: <b>Hi</b> (text)
p.innerHTML = '<b>Hi</b>';    // → Shows: Hi (bold)
```
6. Event Bubbling vs Capturing:
```
// Bubbling (default) - Child → Parent
element.addEventListener('click', handler, false);

// Capturing - Parent → Child
element.addEventListener('click', handler, true);

```
7. Form
```
Q: Which is correct for form validation?
a) form.onsubmit = validate()     // Wrong - executes immediately
b) form.onsubmit = validate       // Correct
c) form.onsubmit = validate;      // Correct (same as b)
d) form.onsubmit = "validate()"   // Wrong
```

* + = 1 or more, * = 0 or more, ? = optional..
^ = start, $ = end
8. 3. Error Types (Exam Me Puchte Hain!)
```
// ReferenceError - undefined variable
console.log(x);  // ReferenceError: x is not defined

// TypeError - wrong type operation
null.toString();  // TypeError: Cannot read property

// SyntaxError - wrong syntax
eval('var x = ;');  // SyntaxError

// RangeError - number out of range
let arr = new Array(-1);  // RangeError
```
mcq :- 
1. Q: Difference between innerHTML and textContent?

a) innerHTML parses HTML, textContent shows plain text  // ✅
b) Both are same
c) textContent is faster
d) innerHTML is deprecated
2. Q: Prevent form submission?

a) return false in onsubmit
b) event.preventDefault()    // ✅ Modern way
c) form.stop()
d) Both a and b             // ✅ Also correct

## JSON

1. Language independent
2. ✅ Native JavaScript support
3. ❌ Single quotes NOT allowed 'name'..
❌ Trailing comma NOT allowed..
❌ Comments NOT allowed..
❌ Functions NOT allowed..
❌ undefined NOT allowed (use null)..
### JSON Parsing (Very Important!)
1. String to Object - JSON.parse()
```
// JSON string
let jsonString = '{"name":"Raj","age":25}';

// Parse to object
let obj = JSON.parse(jsonString);
console.log(obj.name);  // "Raj"
console.log(obj.age);   // 25
```
2. Object to String - JSON.stringify()
```
// JavaScript object
let obj = { name: "Raj", age: 25 };

// Convert to JSON string
let jsonString = JSON.stringify(obj);
console.log(jsonString);  // '{"name":"Raj","age":25}'
```
```
1.  Output?
let str = '{"x":10}';
let obj = JSON.parse(str);
console.log(obj.x);

a) "10"
b) 10        // ✅ Correct (number)
c) undefined
d) Error

Q: Output?
let obj = {x: 10};
console.log(JSON.stringify(obj));

a) {x: 10}
b) {"x":10}  // ✅ Correct (string)
c) [object Object]
d) undefined
```

## JQuery
```
$(selector).action();

// Examples
$('#box').hide();           // ID selector
$('.red').show();           // Class selector
$('p').fadeIn();            // Tag selector
```
```
Q: jQuery syntax format?
a) $(selector).action()  // ✅ Correct
b) jQuery(selector)
c) document.querySelector()
d) getElementById()

Q: Select all paragraphs with class "intro"?
a) $('p.intro')       // ✅ Correct
b) $('#p.intro')
c) $('.p intro')
d) $('p intro')

Q: Select first paragraph?
a) $('p').first()     // ✅ Correct
b) $('p:first')       // ✅ Also correct
c) $('p[0]')
d) Both a and b       // ✅ Best answer

Q: Get parent of #child?
a) $('#child').parent()    // ✅ Correct
b) $('#child').parents()   // All ancestors
c) $('#child').find()
d) $('#child').children()

* $('#box').toggle();             // Toggle show/hide

Extends : 
let obj1 = {a: 1};
let obj2 = {b: 2};
$.extend(obj1, obj2);  // obj1 = {a:1, b:2}

Q4: Valid JSON data types?
Answer: String, Number, Boolean, null, Object, Array

Q1: jQuery syntax?
Answer: $(selector).action()

Q2: Select element by ID?
Answer: $('#myId')

Q3: Hide element with animation?
Answer: $('#box').hide(1000)

Q4: Get text content?
Answer: $('#box').text()

Q5: Document ready?
Answer: $(document).ready() or $(function(){})
```

## AJAX
AJAX = Asynchronous JavaScript And XML

1. Web page ko reload kiye bina server se data fetch/send kar sakte ho
2. Asynchronous = Page freeze nahi hota, background me kaam hota hai
3. Modern web apps me bahut use hota hai (Facebook, Gmail, etc.)
4.  // Fetch data without reload
    fetchData();
```
    $.ajax({ url, type, success, error })
$.get(url, callback)
$.post(url, data, callback)
```

## NODE JS

1. Const :- Variable me phir se assign nhi kar sakte but
   // But objects/arrays can be modified
const arr = [1, 2];
arr.push(3);  // OK
2. REPL - read eval print loop
3. Node.js is single-threaded and asynchronous
4. const [a, b] = [10, 20] is Destructuring
5. To start REPL, just type node
6. .save filename saves the current session
7. Tail recursion means recursive call is the last operation
8. 
```
const arr = [1, 2, 3];
arr.push(4);  // ✅ WORKS! (reference nahi badla)
arr = [5, 6]; // ❌ ERROR! (reference change nahi kar sakte)
```
9. Destructuring
```
// Array Destructuring
const [a, b] = [1, 2];

// Object Destructuring
const {name, age} = {name: "John", age: 25};

// Renaming
const {name: userName} = {name: "John"}; // userName = "John"
```
10. REPL
```
_           // Last result store karta hai
.help       // All commands dikhata hai
.exit       // Exit REPL
.save file  // Session save karta hai
.load file  // File load karta hai
.break      // Multi-line expression exit
Ctrl+C (2x) // Exit REPL
Ctrl+D      // Exit REPL
Underscore _ stores last result
```
11. REcusrion
```
Key Concepts

Stack = Recursive calls store hote hain
Stack Overflow = Base case na ho to infinite recursion
Tail Recursion = Last operation recursive call ho
Memoization = Results cache karke optimization
```

12. Promise
* Promise.all() sabhi promises resolve hone tak wait
* Promise.race() - Jo pehle complete ho uska result
* Promise.any() - Pehla fulfilled promise ka result
```
Key Points ✅

async function always returns Promise
await pauses execution until Promise resolves
Cleaner than .then() chains
Use try-catch for error handling
await only works inside async function
process.nextTick() has highest priority (Node.js)
```
```
Key Points ✅

setTimeout = One time execution
setInterval = Repeated execution
clearTimeout() / clearInterval() = Cancel
setTimeout(fn, 0) NOT immediate (Event Loop)
process.nextTick() > Promises > setTimeout
```
```
console.log("A");

setTimeout(() => console.log("B"), 0);

Promise.resolve().then(() => console.log("C"));

console.log("D");

// Output: A D C B
```
Q4: await without async (ERROR!)
javascriptfunction test() {
    await fetch('url'); // ❌ SyntaxError!
}
Q5: Promise States

Initial → Pending
Success → Fulfilled (resolved)
Failure → Rejected
```
Promise Methods

Promise.all([]) → All must resolve
Promise.race([]) → First to settle
Promise.allSettled([]) → All settled (any state)
Promise.any([]) → First fulfilled
```


## Node.js Asynchronous Programming
https://docs.google.com/document/d/1lIqA5OEUojAbEO4AGeAFPJ46N4CEmAZxeX7xroU1hNc/edit?tab=t.m3awniv4ujc5

```
Detailed Explanations for Wrong Answers
Q3: Wrong - c is correct
javascript[1,2,3].map(x => x * 2) // SYNCHRONOUS callback
map() immediately execute hota hai, async nahi. fs.readFile async hai.

Q7: Wrong - c is correct
fs.readFile(path, callback) - ye callback use karta hai.
fs.readFileSync() synchronous hai, callback nahi leta.

Q11: Wrong - a is correct ⚠️ CRITICAL
javascriptconst p = new Promise((resolve, reject) => {
    resolve("Success");  // Promise settled!
    reject("Error");     // IGNORED! (already settled)
});
Output: Success
Promise ek baar settle ho jaye to state change nahi hota!

Q15: Wrong - b is correct
Promise.race() returns first SETTLED promise (fulfilled ya rejected).
Fastest result milta hai, sirf successful nahi.

Q16: Wrong - c is correct
.finally() always executes, chahe Promise resolve ho ya reject.
.always() exist nahi karta.

Q18: Wrong - b is correct ⚠️ IMPORTANT
No! Promise ek baar settle (fulfilled/rejected) ho jaye to state NEVER change nahi hota.

Q19: Wrong - b is correct
Promise.allSettled() waits for ALL promises to settle (fulfilled OR rejected).
Result mein status dikhata hai har promise ka.

Q20: Wrong - b is correct ⚠️ CRITICAL EVENT LOOP
javascriptnew Promise((resolve) => {
    console.log("A");      // Sync - immediately
    resolve("B");
}).then(console.log);      // Microtask queue
console.log("C");          // Sync - immediately
Output: A C B
Promise constructor sync execute hota hai, .then() microtask queue mein jaata hai!

Q21: Wrong - c is correct ⚠️ FUNDAMENTAL
async function ALWAYS returns Promise.
javascriptasync function test() { return "Hello"; }
// Returns: Promise { 'Hello' }

Q24: Wrong - b is correct
Correct equivalent:
javascriptasync function getData() {
    const data = await fetchData();
    console.log(data);
}

Q25: Wrong - b is correct
async/await mein error handling try-catch se hota hai:
javascripttry {
    const data = await fetchData();
} catch(error) {
    console.log(error);
}

Q26: Wrong - b is correct ⚠️ IMPORTANT
javascriptasync function test() { return "Hello"; }
console.log(test()); // Promise { 'Hello' }
async function Promise return karta hai, direct value nahi!

Q27: Wrong - a is correct
await pauses execution until Promise resolves/rejects.
Ye uska main purpose hai!

Q28: Wrong - c is correct
Both A and B are correct!
Dono valid error handling techniques hain:

Option A: try-catch (standard)
Option B: .catch() with await


Q34: Wrong - c is correct ⚠️ EVENT LOOP
Promise callbacks Microtask Queue mein jaate hain, Callback Queue mein nahi!
Microtask Queue ki priority zyada hai.

Q37: Wrong - b is correct

setTimeout → Once execute (ek baar)
setInterval → Repeatedly execute (bar bar)


Q38: Wrong - b is correct ⚠️ TRICKY
setTimeout(callback, 0) immediately execute NAHI hota!
Ye Call Stack empty hone ka wait karta hai (Event Loop).

Q39: Wrong - b is correct
clearInterval(id) se setInterval stop karte hain.
javascriptconst id = setInterval(() => {}, 1000);
clearInterval(id); // Stop

Q40: Missing Answer - a is correct ⚠️ MOST IMPORTANT
javascriptconsole.log("1");                          // Sync
setImmediate(() => console.log("2"));      // Check phase
setTimeout(() => console.log("3"), 0);      // Timer phase
process.nextTick(() => console.log("4"));  // Next tick queue
console.log("5");                          // Sync
Output: 1 5 4 3 2
Priority Order:

Sync code: 1, 5
process.nextTick(): 4 (highest async priority!)
setTimeout: 3 (Timer phase)
setImmediate: 2 (Check phase)


Critical Concepts to Master
🔴 Promise State (Q11, Q18)

Once settled → NEVER changes
resolve() ke baad reject() ignore hota hai

🔴 async/await Fundamentals (Q21, Q26)

async function → Always returns Promise
Direct value nahi milta, Promise milta hai

🔴 Event Loop Order (Q20, Q32, Q40)
Sync → process.nextTick() → Promises → setTimeout → setImmediate
🔴 Promise Callbacks Location (Q34)

Promise → Microtask Queue (high priority)
setTimeout → Callback Queue (low priority)

🔴 await Purpose (Q27)

Pauses execution until Promise resolves
Blocking behavior (but non-blocking for Event Loop)

🔴 setTimeout(0) Behavior (Q38)

NOT immediate!
Waits for Call Stack to clear


Topics Needing More Practice

Promise State Management ⚠️

Once settled, never changes
Multiple resolve/reject calls ignore hote hain


Event Loop Execution Order 🔥

Sync → nextTick → Microtasks → Macrotasks
Promise vs setTimeout timing


async/await Return Types 📦

async always wraps return in Promise
await pauses execution


Promise Methods

Promise.race() vs Promise.all() vs Promise.allSettled()


Timer Behaviors

setTimeout(0) immediate nahi hai
clearInterval() for stopping
```

## Node.js Modules & npm
```
Q: Difference between exports and module.exports?
a) exports is object, module.exports can be anything  ✅
b) Both are same
c) exports is faster
d) module.exports is deprecated

Q: Which is correct?
a) exports = function() {}     // ❌ Wrong
b) module.exports = function() {}  // ✅ Correct
c) require.exports = function() {}
d) export default function() {}
Q: Load local module?
a) require('myModule')      // ❌ npm package
b) require('./myModule')    // ✅ Correct
c) import myModule
d) include('./myModule')

Q: Load built-in module?
a) require('fs')            // ✅ Correct (no ./)
b) require('./fs')
c) require('/fs')
d) import fs

Yaad Rakho:

Built-in: require('fs') (no path)
Local: require('./file') (with ./)
npm: require('package') (no path)
```
### NPM Commands
```
npm init                    # Create package.json
npm init -y                 # Skip questions

npm install express         # Local install
npm install -g nodemon      # Global install (-g flag)
npm install express --save  # Add to dependencies
npm install jest --save-dev # Add to devDependencies

npm uninstall express       # Remove package
npm update                  # Update packages
npm list                    # List installed
npm list -g                 # List global

Q: Install package globally?
a) npm install -g package   ✅
b) npm install package -g   ✅ (both work)
c) npm global install package
d) npm install package --global  ✅ (also works)

Q: Create package.json quickly?
a) npm init                 // Takes input
b) npm init -y              ✅ Skip questions
c) npm create
d) npm new

Q: Entry point in package.json?
a) "start"
b) "main"               ✅ Correct
c) "entry"
d) "index"

Q: Development dependencies?
a) dependencies         // Production
b) devDependencies      ✅ Correct (dev only)
c) dev
d) testDependencies

Q: Run script "start"?
a) npm start            ✅ Correct
b) npm run start        ✅ Also works
c) node start
d) npm script start

Q: Purpose of package-lock.json?
a) Lock exact versions      ✅ Correct
b) Secure packages
c) List dependencies
d) Configure npm

Q: Should commit package-lock.json?
a) Yes                      ✅ Correct
b) No
c) Only for production
d) Optional

Q: When to install globally?
a) CLI tools (nodemon)      ✅ Correct
b) Project dependencies
c) All packages
d) Never

Q: Where local packages installed?
a) node_modules/            ✅ Correct
b) npm/
c) global/
d) packages/
```
###  FILE SYSTEM (fs) MODULE
1. Synchronous (Blocking):
```
const fs = require('fs');

// Read file
let data = fs.readFileSync('file.txt', 'utf8');
console.log(data);

// Write file
fs.writeFileSync('file.txt', 'Hello World');
```
2. Asynchronous (Non-blocking)
```
// Read file
fs.readFile('file.txt', 'utf8', (err, data) => {
    if (err) throw err;
    console.log(data);
});

// Write file
fs.writeFile('file.txt', 'Hello', (err) => {
    if (err) throw err;
    console.log('Written!');
});Q: Difference sync vs async?
a) Sync blocks, async doesn't    ✅ Correct
b) Sync is faster
c) Async is older
d) No difference

Q: readFileSync returns?
a) Data directly                 ✅ Correct
b) Promise
c) Callback
d) undefined

Q: readFile needs?
a) Callback function             ✅ Correct
b) Promise
c) await
d) return statement

Delete:
fs.unlinkSync('file.txt')
fs.unlink('file.txt', callback)

Check Exists:
fs.existsSync('file.txt')  // true/false
Q: Delete file method?
a) fs.delete()
b) fs.remove()
c) fs.unlink()              ✅ Correct
d) fs.deleteFile()

Q: Append to file?
a) fs.append()              
b) fs.appendFile()          ✅ Correct
c) fs.add()
d) fs.write() // Overwrites

Q: Check file exists?
a) fs.exists()              // Deprecated
b) fs.existsSync()          ✅ Correct
c) fs.check()
d) fs.isFile()

Q: Create HTTP server?
a) http.createServer()      ✅ Correct
b) http.server()
c) http.create()
d) new http.Server()

Q: Start server on port?
a) server.start(3000)
b) server.listen(3000)      ✅ Correct
c) server.run(3000)
d) server.port(3000)

Q: Send response?
a) res.send()
b) res.end()                ✅ Correct
c) res.close()
d) res.finish()

Q: Get request URL?
a) req.path
b) req.url              ✅ Correct
c) req.route
d) req.uri

Q: Get HTTP method?
a) req.method           ✅ Correct
b) req.type
c) req.httpMethod
d) req.verb

Q: Set response header?
a) res.setHeader()          ✅ Correct
b) res.writeHead()          ✅ Also correct
c) res.header()
d) Both a and b             ✅ Best answer

Q: Content-Type for JSON?
a) 'text/json'
b) 'application/json'       ✅ Correct
c) 'json'
d) 'text/plain'

Q: Handle GET request?
a) if (req.method === 'GET')    ✅ Correct
b) if (req.type === 'GET')
c) if (req.get === true)
d) if (req.isGet())

Q: Check URL path?
a) req.path === '/home'
b) req.url === '/home'          ✅ Correct
c) req.route === '/home'
d) req.uri === '/home'
```
⚡ QUICK MCQ REVISION
```
Q1: Export single function?
Answer: module.exports = function() {}

Q2: Load local module?
Answer: require('./module')

Q3: Load built-in module?
Answer: require('fs')

Q1: Sync vs Async?
Answer: Sync blocks, Async doesn't

Q2: Delete file method?
Answer: fs.unlink()

Q3: Append to file?
Answer: fs.appendFile()

Q1: Create server?
Answer: http.createServer()

Q2: Start server?
Answer: server.listen(port)

Q3: Get request URL?
Answer: req.url

Q4: Get HTTP method?
Answer: req.method

Q5: End response?
Answer: res.end()

In Node.js, exports is an object.

const fs = require('fs');
let data = fs.readFileSync('file.txt', 'utf8');
console.log(typeof data);

a) "buffer"
b) "string"  ✅
c) "object"
d) "undefined"
Q28. How to check if file exists?
javascripta) fs.exists()
b) fs.existsSync() ✅
c) fs.checkFile()
d) fs.isFile()

Q29. What does 'utf8' specify in readFile?
javascripta) File format
b) Encoding ✅
c) File type
d) Read mode

writeFile() overwrites (error nahi)
```
## EXPRESS
```
app.get('/user', (req, res) => {
    console.log(req.method);        // HTTP method (GET, POST)
    console.log(req.url);           // URL path
    console.log(req.params);        // URL parameters
    console.log(req.query);         // Query strings
    console.log(req.body);          // Request body (POST data)
    console.log(req.headers);       // HTTP headers
});
```
1. Query Parameters (? ke baad):
   // URL: /search?name=Raj&age=25
2. Route Parameters (: ke saath):
   // URL: /user/123
https://docs.google.com/document/d/1lIqA5OEUojAbEO4AGeAFPJ46N4CEmAZxeX7xroU1hNc/edit?tab=t.axph7c22nena
```
MCQ Important:

req.params → Route parameters (:id)  -- ${req.params.id}
req.query → Query strings (?name=value)
req.body → POST data (middleware needed!)
res.send() vs res.json() → json auto-converts to JSON
Status codes: 200 (OK), 404 (Not Found), 500 (Server Error)

// Use router
app.use('/users', userRoutes);
`express.Router()` modular routes ke liye
app.use('/path', router)` router mount karta hai


```
### **Middleware kya hai?**
Functions jo **request aur response ke beech** run hote hain.
```
// Middleware function
function logger(req, res, next) {
    console.log(`${req.method} ${req.url}`);
    next();  // Pass to next middleware/route
}

// Use middleware
app.use(logger);

// Now all routes will log
app.get('/', (req, res) => {
    res.send('Home');
});
```
Types :- 
1. Application-level
2. Route-level
3. Built-in Middleware :-
4. Third-party Middleware :-cors


Error middleware has 4 parameters: (err, req, res, next)

### EJS
1. app.set('view engine', 'ejs');
2. res.render('viewName', data) renders view
3. <%- include() %> includes partials
4. <% %> JavaScript code (no output)

```
// ❌ Wrong - route defined before middleware
app.get('/', (req, res) => {
    res.send('Home');
});
app.use(logger);  // Won't apply to above route!

// ✅ Correct - middleware first
app.use(logger);
app.get('/', (req, res) => {
    res.send('Home');
});
```
### MCQ
```
1. const express = require('express');
const app = express();
console.log(typeof app);  // function

b) params from URL path, query from query string

Q23. How to create modular routes?
a) express.route()
b) express.Router() ✅
c) express.module()
d) app.router()

Q26. What does :id? mean in /user/:id??
a) Required parameter
b) Optional parameter ✅
c) Query parameter
d) Error

2. app.get('/test', (req, res) => {
    res.send('Hello');   // Response sent
    res.send('World');   // Error! Can't send again
});  // Ek request me sirf ek response bhej sakte ho!

3: express.static() --- (Serves static files)
```
```
// ❌ Wrong - Multiple responses
res.send('First');
res.send('Second');  // Error!

// ✅ Correct - One response
res.send('Only one');

// ✅ Correct - Return stops execution
if(condition) {
    return res.send('Stop here');
}
res.send('This won't run');
```

## React
MCQ Important:

1. npm start runs React app
2. index.js is entry point
3. App.js is main component
4. JSX Rules:
```
// 1. Single parent element
// ❌ Wrong
return (
    <h1>Title</h1>
    <p>Text</p>
);

// ✅ Correct
return (
    <div>
        <h1>Title</h1>
        <p>Text</p>
    </div>
);

// 2. Close all tags
<img src="pic.jpg" />  // Self-closing
<br />

// 3. className (not class)
<div className="box"></div>

// 4. Expressions in {}
const name = "Raj";
<h1>Hello {name}</h1>
<p>{2 + 3}</p>  // 5

// 5. camelCase for attributes
<div onClick={handleClick}>  // not onclick

MCQ Traps:

className (not class)
onClick (not onclick)
Must have one parent
{} for JavaScript expressions


MCQ Important:

Function components are modern
Class components need extends React.Component
Class must have render() method
Function components don't use this
```
5. Props Rules
```
// 1. Props are READ-ONLY (can't change)
// ❌ Wrong
function Welcome(props) {
    props.name = "Changed";  // Error!
}

// 2. Pass any data type
<User name="Raj" age={25} isAdmin={true} data={[1,2,3]} />

// 3. Default props
function Welcome({ name = "Guest" }) {
    return <h1>Hello {name}</h1>;
}
<Welcome />  // "Hello Guest"
<Welcome name="Raj" />  // "Hello Raj"

MCQ Traps:

Props are read-only (immutable)
Pass as attributes
Access with props.propertyName
Numbers/booleans in {}

Data flows parent → child (props)
```
### State & Lifecycle
State = Component's memory (data that changes) - useState
```
MCQ Important:

State is mutable (can change)
Props are immutable (can't change)
useState for function components
this.state for class components
useEffect replaces lifecycle methods
Context: Global state (avoid prop drilling)
Pass function reference, not call: onClick={handleClick} ✅, onClick={handleClick()} ❌
condition && <Component /> (show if true)
Can return null to render nothing
```


### 🎯 Quick MCQ Revision Points:
```
React Basics:

React is a library (not framework)
Uses Virtual DOM
JSX: className, onClick, single parent, {} for JS
Function components are modern

Components:

Function: Simple, no this, hooks
Class: Complex, this, lifecycle methods
Must start with capital letter

Props vs State:

Props: Read-only, parent → child
State: Mutable, component's data
Props in {} for non-strings: age={25}

Events:

onClick={handleClick} ✅
onClick={handleClick()} ❌
onClick={() => handleClick(id)} ✅

Hooks:

useState(initialValue) → [value, setValue]
useEffect(() => {}, []) → componentDidMount
useEffect(() => {}, [dep]) → runs when dep changes

Conditional:

{condition ? true : false} (ternary)
{condition && <Component />} (show if true)

Lists:

map() to render lists
key prop required (unique)
```

### MCQ
```
1. npx create-react-app my-app
2. javascriptclass Welcome extends React.Component {
    // What is needed here?
}
a) constructor() method
b) render() method ✅
c) display() method
d) show() method

// ❌ Wrong - lowercase
function welcome() {
    return <h1>Hi</h1>;
}
<welcome />  // React treats as HTML tag, not component!

// ✅ Correct - Uppercase
function Welcome() {
    return <h1>Hi</h1>;
}
<Welcome />  // React component
Rule: Component names must start with capital letter!

// ❌ Wrong
<User age="25" />     // String "25"
<User age=(25) />     // Syntax error

// ✅ Correct
<User age={25} />     // Number 25
<User active={true} /> // Boolean
<User data={[1,2,3]} /> // Array
-------------------------------------
const [count, setCount] = useState(0);

// ❌ Wrong - Direct assignment
count = 5;  // Error! Assignment to constant variable

// ✅ Correct - Use setter
setCount(5);

-------------------------------------
Q28: useEffect without dependency ❌
Your Answer: d (Only on mount) | Correct: b (On every render)
---------------------------------

Q29: What triggers re-render? ❌
Your Answer: a (State change) | Correct: c (Both state & props)
------------------------------------------


Q30: Modify state directly in class ❌
Your Answer: d (Only with hooks) | Correct: b (No, use setState)
// ❌ Wrong - Direct mutation
        this.state.count = 5;  // Won't trigger re-render!
        
        // ✅ Correct
        this.setState({ count: 5 });  // Triggers re-render
-------------------------------
const [count, setCount] = useState(10);
setCount(count + 1);  // count is still 10
setCount(count + 1);  // count is still 10
console.log(count);   // 10 (not updated yet!)
Why? State updates are asynchronous! count is still 10 when console.log runs.
----------------------------------------
Q36: e.preventDefault() ❌
Your Answer: a (Stops event propagation) | Correct: b (Prevents default behavior)
// stopPropagation() - Stops event bubbling

preventDefault() → Stops default browser behavior
stopPropagation() → Stops event bubbling to parent
```
```
Controlled: value + onChange
e.preventDefault() stops form submission
Use e.target.value to get input value
