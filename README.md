# MERN_CCEE
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
