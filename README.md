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
