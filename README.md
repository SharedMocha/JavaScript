# JavaScript
JavaScript -read raw version

**NMot to forget
**One of JavaScript’s greatest assets is its non-blocking properties, or that it is an asynchronous language. //JavaScript uses an event loop to handle asynchronous function calls. When a program is run, function calls are made and added to a stack. The functions that make requests that need to wait for servers to respond then get sent to a separate queue. Once the stack has cleared, then the functions in the queue are executed.
**In object use , for each line.wheras in calss use ; ->simple right?  //{a=b,function,,,,} -> object
**for api calls use fetch with async ..await

1.) when using for loop use let-> this is given in ES6 for block level scope(function,for loop,anything inside {},if,else). (u cant use let on browser a not supported yet,on jodejs u can) (https://stackoverflow.com/questions/762011/whats-the-difference-between-using-let-and-var)
2.)in nodejs u can replace var with let --but not on browser..
3.) To fully distinguish the difference between JavaScript and ECMAScript: if you want to create an app or program you can use JavaScript — if you want to create a new scripting language you can follow the guidelines in ECMAScript. So, when you see ES6 or JavaScript ES6, it means that that version of JavaScript is following the specifications in the sixth edition of ECMAScript!
4.) ===,!== (compare and not compare operatoes)
5.) * Truthy and falsy -checks is a variable exists and has a value other than falsy values = 0,empty string,null,undefined,NaN (NOT A NUMBER);
5.1) let defaultName = username || 'Stranger';  //Because || or statements check the left-hand condition first, the variable defaultName will be assigned the actual value of username if is truthy, and it will be assigned the value of 'Stranger' if username is falsy. This concept is also referred to as short-circuit evaluation.
6.)Ternary Operator - condition ? firstExpression : secondExpression
7.)create randon  numbers under 1000 ->  Math.floor(Math.random() * 1000);
8.) hoisting - caling function before it is executed--pls make sure you wont use this ..or call botton decalred function on top..follow procdedural or structutral programming.
9.) Helper Functions -- function calling another function
10.)Types of function --regaular, function expression (const val = function(){}),arrow function,Concise Body Arrow Functions
12.)scope-global,,block(variable inside block are called local vairbale) --note that Scope pollution is when we have too many global variables that exist in the global namespace
13.)While it’s important to know what global scope is, it’s best practice to not define variables in the global scope.
14.0arrays can have types of differebnt-string,number,boolean
15.remember array methods - https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array
16. pass-by-reference  - So when you pass an array into a function, if the array is mutated inside the function, that change will be maintained outside the function as well. You might also see this concept explained as pass-by-reference since what we’re actually passing the function is a reference to where the variable memory is stored and changing the memory. // addFlower(flowers); here flowers is passed as reference and its a array or memory location
17.)remeber array methods- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/join
18.)So you may be wondering when to use a while loop! The syntax of a for loop is ideal when we know how many times the loop should run, but we don’t always know this in advance. Think of eating like a while loop: when you start taking bites, you don’t know the exact number you’ll need to become full. Rather you’ll eat while you’re hungry. In situations when we want a loop to execute an undetermined number of times, while loops are the best choice.
19.)In some cases, you want a piece of code to run at least once and then loop based on a specific condition after its initial run. This is where the do...while statement comes in.
20.)The break keyword allows programs to “break” out of the loop from within the loop’s block.
21.) abstraction ->  In programming, we can accomplish “abstraction” by writing functions. In addition to allowing us to reuse our code, functions help to make clear, readable programs.
22.) higher order function -> Higher-order functions are functions that accept other functions as arguments and/or return functions as output. This enables us to build abstractions on other abstractions, just like “We hosted a birthday party” is an abstraction that may build on the abstraction “We made a cake.”
23.)In JavaScript, functions are first class objects. This means that, like other objects you’ve encountered, JavaScript functions can have properties and methods.
24.)Since functions are a type of object, they have properties such as .length and .name and methods such as .toString().
25.) VV IMP -> JavaScript functions behave like any other data type in the language; we can assign functions to variables, and we can reassign them to new variables. //const busy = announceThatIAmDoingImportantWork; //ASSIGNING ONE FUNCTION to anothetr property
26.)Since functions can behave like any other type of data in JavaScript, it might not surprise you to learn that we can also pass functions (into other functions) as parameters.A higher-order function is a function that either accepts functions as parameters, returns a function, or both!
27.)When we pass in a higher order function, it is by reference, not by return value. We want to invoke it only once it is inside the other function’s body. (https://discuss.codecademy.com/t/crossing-wires-somewhere-with-callbacks-and-hof-s/395283/2)
27.) callbacks--when u pass a function as param to another function -- the passed function is not invoked first..isntead the called function will be invoked which interns called the param funciton we passed.
28.)https://discuss.codecademy.com/t/when-should-we-use-callbacks-vs-directly-calling-a-function/376857
29.)iterator method - array.forEach() -> runs a function on each array item --for each takes array itema nd function and will return new
30.)iterator method -  array.map() -> map rforturns an array by taking in individual elemts of an array ->Like remove numbers froma  given array //const secretMessage = animals.map(animal => {return animal.charAt(0)}); -->here we return as we send value directly
30.1)-> u need a const like 'secretmessage'' for map to store the returned new array values.
31.) iterator method - filter() -> returns a new array ->However, .filter() returns an array of elements after filtering out certain elements from the original array.The callback function for the .filter() method should return true or false depending on the element that is passed to it. The elements that cause the callback function to return true are added to the new array
31.1)const longFavoriteWords = favoriteWords.filter(_ => {return _.length > 7}); //save return values to const and you must have a validation condition as only the one evaluated to true will be added...
32.)iterator method - findIndex ->We sometimes want to find the location of an element in an array. That’s where the .findIndex() method comes in! Calling .findIndex() on an array will return the index of the first element that evaluates to true in the callback function.
32.1)const startsWithS = animals.findIndex(animal => {return animal[0] === 's';});//same like others--store the first found indx in const value;
33.)iterator method -  reduce->Another widely used iteration method is .reduce(). The .reduce() method returns a single value after iterating through the elements of an array, thereby reducing the arra
34.) array iterator methods -> https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array#Iteration_methods
35) Foeach->used when we want to go through array list and print something or perform some operation for each elemtn
36) filter -> used to filter based on a condiiton and get a new array
37)reduce--choose to get a single value from array
38)map -> modify array elemts and return new array
39)some- >used to return boolean value // nums.some(num => num < 0);
40.) story.split(' '); // break array using space //story.join() //join using , 
41.0) Object- has properties,methods,privary variables,getters,setters(getetrs and setters are used to set valus to private or privacy variables which havw _ infront),factory functions are abstract objects which has some basic,default propers,methods and getters and setters..
41.)Objects can be assigned to variables just like any JavaScript type. We use curly braces, {}, to designate an object literal: let spaceship = {}; // spaceship is an empty object //We fill an object with unordered data. This data is organized into key-value pairs. A key is like a variable name that points to a location in memory that holds a value. (https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-objects/objectliteraldiagram.svg)
41.1)let fasterShip = {color:'silver','Fuel Type':'Turbo Fuel'}; //quotes for 'fuel type' are used because they have special char which is space.
*three ways of accessing values from objects -> .,[],{} destructured assignment
41.2)To access values of object --one way us-- . oeprator -> objectname.propertyname
41.3))To access values of object --one way us--[] //spaceship['Active Duty']; //object name with [propertyname]
41.3.1)We *must* use bracket notation when accessing keys that have numbers, spaces, or special characters in them.
41.4)To access values of object -- onbe way is to destrcutured assignment ->We often want to extract key-value pairs from objects and save them as variables. Take for example the following object: //const { residence } = vampire;  // vampire is json object and residence is a key inside vampire object..
42.) You can assign values to json object properties - https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-objects/object+update+property.svg
42.1)If property exits then itst value is updated -->if not it will be appended to the object. //It’s important to know that although we can’t reassign an object declared with const, we can still mutate it, meaning we can add new properties and change the properties that are there.
43)anyone can delete property inside object -> delete spaceship['Secret Mission'];
44) objects can have methods -console.log() //here console is  object which has key ,values and log is  amethod defeined in it 
45)Objects are passed by reference. This means when we pass a variable assigned to an object into a function as an argument, the computer interprets the parameter name as pointing to the space in memory holding that object. As a result, functions which change object properties actually mutate the object permanently (even when the object is assigned to a const variable).
46) here use pass by reference to pass object and its internal value to modify ->const greenEnergy = objectParam =>{objectParam['Property Name'] ='avocado oil'; };
47)to iternate on object --you will use for...in ..not foreach //https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for...in
48)The this keyword references the calling object which provides access to the calling object’s properties. In the example above, the calling object is goat and by using this we’re accessing the goat object itself, and then the dietType property of goat by using property dot notation.
49) VVIMP -> Arrow Functions and this -> NEVER USER this keyword when using arrow functioninside an object -as it wont work -- Arrow functions inherently bind, or tie, an already defined this value to the function itself that is NOT the calling object. In the code snippet above, the value of this is the global object, or an object that exists in the global scope, which doesn’t have a dietType property and therefore returns undefined.
50.)privary in js->Rather, JavaScript developers follow naming conventions that signal to other developers how to interact with a property. One common convention is to place an underscore _ before the name of a property to mean that the property should not be altered. Here’s an example of using _ to prepend a property.
51). get object keys -  Object.keys(robot);
52.) get object keys and values --Object.entries(robot)
53.)add  extra fields to object -  //const newRobot = Object.assign({laserBlaster: true, voiceRecognition: true}, robot);
54)->see more object methods like above --> https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object#Methods_of_the_Object_constructor
55) factory functions(returns new object,not one that modfiied an existying object)--remember--u cant use arrow functions...as this wont work-->use getetr and setter where u can use this keyword...factrors fucntions hasve privay variable like _name--these are kind of private and use getter and setter to update them..
56.) getters inside functions- > Getters can perform an action on the data when getting a property. Getters can return different values using conditionals.In a getter, we can access the properties of the calling object using this.The functionality of our code is easier for other developers to understand.
56.1.)Another thing to keep in mind when using getter (and setter) methods is that properties cannot share the same name as the getter/setter function. If we do so, then calling the method will result in an infinite call stack error. One workaround is to add an underscore before the property name like we did in the example above.
57.)setter inside function ->  include checking input, performing actions on properties, and displaying a clear intention for how the object is supposed to be used. Nonetheless, even with a setter method, it is still possible to directly reassign properties. 
uses objects or factory functions if we will always have one object like db instance--> if we will have several instance then uses classes..
58.)JavaScript is an object-oriented programming (OOP) language we can use to model real-world items
**********class is similar to object---but u can create multiple instances wheras for object u can't- class has constructor,methods,getters,setters and static methods(methods we cna call without creatin an instance of class)
58.1) -> js objects are unique --meaning u need 10 objects wiht similar methods to show 10 people--isntead use classes as it creates instances of one object
58.2) main variation between class and object is -> classes uses cosntructor wheras object directly define properties like json object.. object{_name: 'Halley',_behavior: 0} -class {  constructor(name) {this._name = name;this._behavior = 0;}}
58.3) JavaScript calls the constructor() method every time it creates a new instance of a class. ->Inside of the constructor() method, we use the this keyword. In the context of a class, this refers to an instance of that class. In the Dog class, we use this to set the value of the Dog instance’s name property to the name argument.
59.) Notice, we call super on the first line of our constructor(), then set the usesLitter property on the second line. In a constructor(), you must always call the super method before you can use the this keyword — if you do not, JavaScript will throw a reference error.   //class Cat extends Animal {constructor(name, usesLitter) {super(name);this._usesLitter = usesLitter;}}
60.)Static Methods in classes-> can be called without instantiaon-- not like java ex--Date.now();
*problem is latest js might not be supported by all versions of browser --so use below 2 tools to check what is compatiable and use babel to auto convert..
61.) caniuse.com — A website that provides data on web browser compatibility for HTML, CSS, and JavaScript features. You will learn how to use it to look up ES6 feature support.
62.)Babel — A Javascript library that you can use to convert new, unsupported JavaScript (ES6), into an older version (ES5) that is recognized by most modern browsers.
62.1) first babel install ->npm install babel-cli
62.2) second babel install -> npm install babel-preset-env
64.)devDependencies in package.json is the key as it enable 'npm install' rather than specifying each package to install like 'npm install xx' -> u can add a package to it by appending -D .Exmaple ' npm install babel-preset-env -D';
65.)Modules--> We can also wrap any collection of data and functions in an object, and export the object using module.exports.
65.0)let Menu = {}; //note here that M is upper case--because this will an export like  'module.exports = Menu;'
65.1) The pattern we use to export modules is thus: Define an object to represent the module.Add data or behavior to the module.Export the module.
65.2) to import module we use something like 'const Menu = require('./menu.js');'
there are  3 ways to export,import .old way before es6- module.export = ObjectName , after est there are 2 ways , a.)export default Object b.) export {property names, function names} //this is named export
66.) we can also include export infornt of property or function -thus making it export imemdialty.. for import we still use 'import {} from '';' syntax
67.) masked or named export --like if you want to give alias name to an export function ->export { specialty as chefsSpecial, isVegetarian as isVeg, isLowSodium }; for import we use the aliased names similr to 'import {} from ''';
68.)We can also use named exports and default exports together in a  file ..same way we can use both old and new ways to import modules 'import GlutenFree from './menu'; or import { specialty, isVegetarian, isLowSodium } from './menu';
69.) Promise - 3 states (pending,fulfilled,rejected) (pending-working,fulfileed-complted,rejected-some issues and failed) (https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-promises/Art-346-01.svg)
69.1) promise has .then() and .cath() //.then() to execute code after promise resolves. catch() to handle errors
69.2.) chanining promise. .then(return x).then(return y) //here return is must or else u will not take previous promise value isntead u will rely on the root
69.3) promise.all() //used to execute many promise at ones-- will give result as array or stops if one of them fails
70.) async/await -is just a sugar coat on top of promise
70.1) async is keyword telling this funciton is async and await is operator which stops execution till promise resolves
70.2)you code async//await by creting child functions with promise and include them in a aprent function with keyword async and all its child functions with await.
70.3)  bettee use try,catch in async await.
70.4) concuerey is possible in async/await along with .all()
** 3 WAYS TO MAKE API CALLS -XMLHTTPREQUESTS,promise~then, async and await (u can use fetch combined with prmise and async anda wait)
71)AJAX - Asynchronous JavaScript and XML (AJAX), enables requests to be made after the initial page load. Initially, AJAX was used only for XML formatted data, now it can be used to make requests that have many different formats.
72)Similarly, the XMLHttpRequest (XHR) API, named for XML, can be used to make many kinds of requests and supports other forms of data.
721.)XMLHttpRequest response types- > document(HTML,XML),json,text(DOMSTRING   i.e utf-16),blob(images,videos),arraybuffer(js array)
73) creating a request or api,get,post -> https://s3.amazonaws.com/codecademy-content/courses/intermediate-javascript-requests/diagrams/XHR+GET+transparent.svg
74)json.STRINGIFY //converts data to string to send in post body
75.)fetchGET - https://s3.amazonaws.com/codecademy-content/courses/intermediate-javascript-requests/diagrams/fetch+GET+transparent.svg
76.)FETCH POST- https://s3.amazonaws.com/codecademy-content/courses/intermediate-javascript-requests/diagrams/fetch+POST+transparent.svg
77) GET requwest using async -> https://s3.amazonaws.com/codecademy-content/courses/intermediate-javascript-requests/diagrams/async+await+GET+diagram.svg
78.)getr request post-check github 


Java script project setup with babel-->
1.)npm init -> creates package.json file. //this has 'Metadata — This includes a project title, description, authors, and more.' //A list of node packages required for the project — If another developer wants to run your project, npm looks inside package.json and downloads the packages in this list.//Key-value pairs for command line scripts — You can use npm to run these shorthand scripts to perform some process. In a later exercise, we will add a script that runs Babel and transpiles ES6 to ES5.
2.) (dont run this-move to next step)npm install package name  //The install command creates a folder called node_modules and copies the package files to it. The install command also installs all of the dependencies for the given package.
3.)Instal bebel ->2 commans (1.)npm install babel-cli -D 2.)npm install babel-preset-env -D )//The -D flag instructs npm to add each package to a property called devDependencies in package.json.
4.) after installing babel u need to specify which version of the source jvascipt code we will use. to do this follow below steps
4.1) create or open .babelrc file
4.2) include below code in order to tell  'transpiling code from an ES6+ source' //meaning we write code in es6 and it gets converted to es5.  'env' in below instructs Babel to transpile any code from versions ES6 and later.

{
  "presets": ["env"]
}
4.3)We need to specify a script in package.json that initiates the ES6+ to ES5 transpilation.
4.3.1) open package.json  - Inside of the package.json file, there is a property named "scripts" that holds an object for specifying command line shortcuts --here add 'build' like below. "babel src -d lib" is a command line method that transpiles ES6+ code to ES5. Let’s consider each argument in the method call:

...
"scripts": {
  "test": "echo \"Error: no test specified\" && exit 1",
  "build": "babel src -d lib"
}


explanation-
babel — The Babel command call responsible for transpiling code.
src — Instructs Babel to transpile all JavaScript code inside the src directory.
-d — Instructs Babel to write the transpiled code to a directory.
lib — Babel writes the transpiled code to a directory called lib.

5.) test it by running 'npm run build'-notice that new folder lib is created which has files that are converted to es5 from es6 code in our 'src' folder
--------------------------->


ES6 -> Came in 2015 - below are thiongs it got
1.) 2 new keywords -let and const. BEFORE THIS THERE IS ONLY var
1.1) Let -> used inside block only -for(let i=); wheras var is used at a functional level-check this -> https://stackoverflow.com/questions/762011/whats-the-difference-between-using-let-and-var
1.2) const --used to give cosntant values-
1.3) Variables declared with the const keyword cannot be reassigned. However, elements in an array declared with const remain mutable. Meaning that we can change the contents of a const array, but cannot reassign a new array or a different value.

2.)String interpolation->
2.1) const myPet = 'armadillo'; // console.log(`I own a pet ${myPet}.`);


3.)default paramaters--One of the features added in ES6 is the ability to use default parameters. Default parameters allow parameters to have a predetermined value in case there is no argument passed into the function or if the argument is undefined when called.
function greeting (name = 'stranger') {
  console.log(`Hello, ${name}!`)
}

4.) using const for 'Function expressions' //here const is the function name..
https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-functions/Diagram/expression.svg

5.) Arrow functions -- “fat arrow” () => notation. //U CANT USE ARROW FUNCTIONS INSIDE A FACTORY DFUNCTION--AS SCOPE OF ARROW IS A GLOBAL .this rather than calling object..
Arrow functions remove the need to type out the keyword function every time you need to create a function. Instead, you first include the parameters inside the ( ) and then add an arrow => that points to the function body surrounded in { } like this:
const rectangleArea = (width, height) => {
  let area = width * height;
  return area;
};

6.)With the new method syntax introduced in ES6 we can omit the colon and the function keyword when we write function inside  aobject
before es6-
const alienShip = {
  invade: function () { 
    console.log('Hello! We have come to dominate your planet. Instead of Earth, it shall be called New Xaculon.')
  }
};


after es6-
const alienShip = {
  invade () { 
    console.log('Hello! We have come to dominate your planet. Instead of Earth, it shall be called New Xaculon.')
  }
};

Object methods are invoked by appending the object’s name with the dot operator followed by the method name and parentheses:  alienShip.invade();
---------------------->
greeting('Nick') // Output: Hello, Nick!
greeting() // Output: Hello, stranger!


7.)Property Value Shorthand - ES6 introduced some new shortcuts for assigning properties to variables known as destructuring.
before es6-In the previous exercise, we created a factory function that helped us create objects. We had to assign each property a key and value even though the key name was the same as the parameter name we assigned to it. To remind ourselves, here’s a truncated version of the factory function:
const monsterFactory = (name, age) => {
  return { 
    name: name,
    age: age
  }
};

after es6-
const monsterFactory = (name, age) => {
  return { 
    name,
    age 
  }
};



8.)Destructured Assignment - const { residence } = vampire; 


9.) export default->As of ES6, JavaScript has implemented a new more readable and flexible syntax for exporting modules. These are usually broken down into one of two techniques, default export and named exports.
**export default uses the JavaScript export statement to export JavaScript objects, functions, and primitive data types.

before es6-
let Menu = {};
module.exports = Menu;

after es6-
let Menu = {};

export default Menu;


9.1) es6-import->

import Menu from './menu';

The import keyword begins the statement.
The keyword Menu here specifies the name of the variable to store the default export in.
from specifies where to load the module from.
'./menu' is the name of the module to load. When dealing with local files, it specifically refers to the name of the file without the extension of the file.


10) export named->ES6 introduced a second common approach to export modules. In addition to default export, named exports allow us to export data through the use of variables.
beauty is -u dont need to add propertites or methods to a export object and delcare like 'let Airplane' isntead u can use 'let airplane' and decalre variable and functions seperate -
Ex->
let specialty = '';
function isVegetarian() {
}; 
function isLowSodium() {
}; 

Notice that, when we use named exports, we are not setting the properties on an object. Each export is stored in its own variable.
specialty is a string object, while isVegetarian and isLowSodium are objects in the form of functions. Recall that in JavaScript, every function is in fact a function object.
export { specialty, isVegetarian }; exports objects by their variable names. Notice the keyword export is the prefix.
specialty and isVegetarian are exported, while isLowSodium is not exported, since it is not specified.


10.1) names improts->
import { specialty, isVegetarian } from './menu';

console.log(specialty);


explanation-
Here specialty and isVegetarian are imported.
If we did not want to import either of these variables, we could omit them from the import statement.
We can then use these objects as in within our code. For example, we would use specialty instead of Menu.specialty.



11.) es6- request --> fetch(),async(),await()

fetch-GET- https://s3.amazonaws.com/codecademy-content/courses/intermediate-javascript-requests/diagrams/fetch+GET+transparent.svg
FETCH POST-https://s3.amazonaws.com/codecademy-content/courses/intermediate-javascript-requests/diagrams/fetch+POST+transparent.svg
--------------------------ES8->
Originally, JavaScript used callback functions to handle asynchronous actions. The problem with callbacks is that they encourage complexly nested code which quickly becomes difficult to read, debug, and scale. With ES6, JavaScript integrated native promises which allow us to write significantly more readable code. JavaScript is continually improving, and ES8 provides a new syntax for handling our asynchronous action, async...await. The async...await syntax allows us to write asynchronous code that reads similarly to traditional synchronous, 

The async...await syntax is syntactic sugar— it doesn’t introduce new functionality into the language, but rather introduces a new syntax for using promises and generators. Both of these were already built in to the language. Despite this, async...await powerfully improves the readability and scalability of our code. Let’s learn how to use it!



------
-----------
javascript -
Object- Same like instance - It has methods and properties.
scope for variable - global scope (var), functional scope(var), block scope (let keyword)
-> console.log(5) //CONSOLE IS AN OBJECT WITH METHOD LOG//we mix these 2 using dot operator
-----------------------------------

Comments- 2 ways
1.) //
2.) /* --- */
-----------------------------------
Types -  Data
Primitive data types-
1.) Int,String,Boolean,null,undefined,symbol
-----------------------------------
Arthimetic operators-
+,-,*,/*%
--------------------------
String methods by java script->
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/prototype

ootb java script objects-
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects

keywords->
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Lexical_grammar#Keywords


variables -
3 ways to create one - (es6 in 2015 brought 2 new ones -let and const)-->
var,let,const-
->write var names in camel casing- > ex-myName
-->
in JS we create variables,store or update info stored in it and get the value stored.
https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-variables/variable+boxes.svg



Java script most common used --
*console.log('Teaching the world how to code'.length); //prints length using . operator
*console.log('hello'.toUpperCase()); // Prints 'HELLO'
*console.log('Hey'.startsWith('H')); // Prints true
*levelUp += 5; //
*powerLevel -= 100;
*multiplyMe *= 11;
*quarterMe /= 4;
*a++ //The incre ment operator will increase the value of the variable by 1
*b--; //The decrement operator will decrease the value of the variable by 1
*console.log(typeof unknown1); // Output: string 
*if statement
*if...else
*comparison operators: <,>,<=,>=,===,!==
*logical operatoes -> &&, || 
* Truthy and falsy -checks is a variable exists and has a value other than falsy values = 0,empty string,null,undefined,NaN (NOT A NUMBER);
*Tenary Operator - expression ? true : false 
* else if statement - 
* switch keyword - 
*Types of function --regaular, function expression (const val = function(){}),arrow function
 **Regular Function ->
  function rectangleArea(width, height) {
  if (width < 0 || height < 0) {
    return 'You need positive integers to calculate area!';
  }
  return width * height;
  }
 ** Function expression: (10.) remember 'Function expressions' -> here we create a no name/anonymus function and and store in a variable in order to refer if  (const length = function(width,height){return width*height}))
 https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-functions/Diagram/expression.svg
 ** Arrow functions
 Arrow functions remove the need to type out the keyword function every time you need to create a function. Instead, you first include the parameters inside the ( ) and then add an arrow => that points to the function body surrounded in { } like this:
const rectangleArea = (width, height) => {
  let area = width * height;
  return area;
};
 **Concise Body Arrow Functions --they wont contain return--isntead they simply give back value computed like a + b ..but not return a +b ;
 https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-functions/Diagram/parameters.svg
 https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-functions/Diagram/return.svg
 ** const getSleepHours = day = {if(day === 'monday'){return 8;}}; // here getSleepHours is the funciton name
*scope-global,local,block
 **global -- In global scope, variables are declared outside of blocks. These variables are called global variables. Because global variables are not bound inside a block, they can be accessed by any code in the program, including code in blocks.
 **block-Variables that are declared with block scope are known as local variables because they are only available to the code that is part of the same block.
*array -One way we can create an array is to use an array literal. An array literal creates an array by wrapping items in square brackets [] (https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-arrays/array+literal.svg)
 **array.length,.pop() and .push(),.join(), .slice(), .splice(), .shift(), .unshift(), and .concat()
 **array.push() //One method, .push() allows us to add items to the end of an array. Here is an example of how this is used: //itemTracker.push('item 3', 'item 4');
 **array.pop() - // Another array method, .pop(), removes the last item of an array.
 **array methods - https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array
  groceryList.shift();
console.log(groceryList);
groceryList.unshift('popcorn');
console.log(groceryList);
console.log(groceryList.slice(1,4));
console.log(groceryList);
const pastaIndex = groceryList.indexOf('pasta');
console.log(pastaIndex);
 ** const nestedArr = [[1], [2, 3]];
*array.splice(indexToStart, numberOfIndices, 'stringToAdd');

**iterators --for loop -->example
   const animals = ['Grizzly Bear', 'Sloth', 'Sea Lion'];
for (let i = 0; i < animals.length; i++){
  console.log(animals[i]);
}


while loop- //set how countertwo is outside and how we increment based on condition.
// A while loop that prints 1, 2, and 3
let counterTwo = 1;
while (counterTwo < 4) {
  console.log(counterTwo);
  counterTwo++;
}
//What would happen if we didn’t increment counterTwo inside our block? If we didn’t include this, counterTwo would always have its initial value, 1. That would mean the testing condition counterTwo < 4 would always evaluate to true and our loop would never stop running! This is called an infinite loop and it’s something we always want to avoid. Infinite loops can take up all of your computer’s processing power potentially freezing your computer.
//

*In some cases, you want a piece of code to run at least once and then loop based on a specific condition after its initial run. This is where the do...while statement comes in.A do...while statement says to do a task once and then keep doing it until a specified condition is no longer met. The syntax for a do...while statement looks like this:
example -->

   let countString = '';
let i = 0;

do {
  countString = countString + i;
  i++;
} while (i < 5);

console.log(countString);

explanation ->In this example, the code block makes changes to the countString variable by appending the string form of the i variable to it. First, the code block after the do keyword is executed once. Then the condition is evaluated. If the condition evaluates to true, the block will execute again. The looping stops when the condition evaluates to false.

**The break keyword allows programs to “break” out of the loop from within the loop’s block.

*Function
 ** basic function properties -> https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function#Properties
 ** basic function methods. -->https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function#Methods
 *ways to call function for map or for each
  **const bigNums = [1, 2, 3, 4, 5].map(el => el * 5);
  **const bigNums = [1, 2, 3, 4, 5].map(function(el){return el * 5;});
*fiLTER->
Another useful iterator method is .filter(). Like .map(), .filter() returns a new array. However, .filter() returns an array of elements after filtering out certain elements from the original array. The callback function for the .filter() method should return true or false depending on the element that is passed to it. The elements that cause the callback function to return true are added to the new array. Take a look at the following example:
const words = ['chair', 'music', 'pillow', 'brick', 'pen', 'door']; 

const shortWords = words.filter(word => {
  return word.length < 6;
});

**find index-->
We sometimes want to find the location of an element in an array. That’s where the .findIndex() method comes in! Calling .findIndex() on an array will return the index of the first element that evaluates to true in the callback function.
const jumbledNums = [123, 25, 78, 5, 9]; 

const lessThanTen = jumbledNums.findIndex(num => {
  return num < 10;
});

**reduce->Another widely used iteration method is .reduce(). The .reduce() method returns a single value after iterating through the elements of an array, thereby reducing the array

-->
const numbers = [1, 2, 4, 10];

const summedNums = numbers.reduce((accumulator, currentValue) => {
  return accumulator + currentValue
})

console.log(summedNums) // Output: 17
-->
Now let’s go over the use of .reduce() from the example above:

numbers is an array that contains numbers.
summedNums is a variable that stores the returned value of invoking .reduce() on numbers.
numbers.reduce() calls the .reduce() method on the numbers array and takes in a callback function as argument.
The callback function has two parameters, accumulator and currentValue. The value of accumulator starts off as the value of the first element in the array and the currentValue starts as the second element. To see the value of accumulator and currentValue change, review the chart above.
As .reduce() iterates through the array, the return value of the callback function becomes the accumulator value for the next iteration, currentValue takes on the value of the current element in the looping process.
The .reduce() method can also take an optional second parameter to set an initial value for accumulator (remember, the first argument is the callback function!). For instance:
const numbers = [1, 2, 4, 10];

const summedNums = numbers.reduce((accumulator, currentValue) => {
  return accumulator + currentValue
}, 100)  // <- Second argument for .reduce()

console.log(summedNums); // Output: 117

factory function->abstract methods-- > So far we’ve been creating objects individually, but there are times where we want to create many instances of an object quickly. Here’s where factory functions come in. A real world factory manufactures multiple copies of an item quickly and on a massive scale. A factory function is a function that returns an object and can be reused to make multiple object instances. Factory functions can also have parameters allowing us to customize the object that gets returned.

Let’s say we wanted to create an object to represent monsters in JavaScript. There are many different types of monsters and we could go about making each monster individually but we can also use a factory function to make our lives easier. To achieve this diabolical plan of creating multiple monsters objects, we can use a factory function that has parameters:-->
example--
const monsterFactory = (name, age, energySource, catchPhrase) => {
  return { 
    name: name,
    age: age, 
    energySource: energySource,
    scare() {
      console.log(catchPhrase);
    } 
  }
};

Modules--
step1 -> write a module
The pattern we use to export modules is thus:

Define an object to represent the module.
Add data or behavior to the module.
Export the module.

exxample->
let Airplane = {}; //not uppercase A for airplane--we use when exporting
Airplane.myAirplane = "StarJet";
module.export  = Airplane;

step2 - import a module


code-
const Menu = require('./menu.js');

function placeOrder() {
  console.log('My order is: ' + Menu.specialty);
}

placeOrder();

anonymous function->
 displayAirplane: function() {
    return this.myAirplane;
  }
  
 
  
  
  readme.2 file-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  

Variables->
Variables hold reusable data in a program and associate it with a name.
Variables are stored in memory.
The var keyword is used in pre-ES6 versions of JS.
let is the preferred way to declare a variable when it can be reassigned, and const is the preferred way to declare a variable with a constant value.
Variables that have not been initialized store the primitive data type undefined.
Mathematical assignment operators make it easy to calculate a new value and assign it to the same variable.
The + operator is used to concatenate strings including string values held in variables
In ES6, template literals use backticks ` and ${} to interpolate values into a string.
The typeof keyword returns the data type (as a string) of a value.


CONDITIONAL STATEMENTS ->
An if statement checks a condition and will execute a task if that condition evaluates to true.
if...else statements make binary decisions and execute different code blocks based on a provided condition.
We can add more conditions using else if statements.
Comparison operators, including <, >, <=, >=, ===, and !== can compare two values.
The logical and operator, &&, or “and”, checks if both provided expressions are truthy.
The logical operator ||, or “or”, checks if either provided expression is truthy.
The bang operator, !, switches the truthiness and falsiness of a value.
The ternary operator is shorthand to simplify concise if...else statements.
A switch statement can be used to simplify the process of writing multiple else if statements. The break keyword stops the remaining cases from being checked and executed in a switch statement.



Functions-
A function is a reusable block of code that groups together a sequence of statements to perform a specific task.
A function declaration :https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-functions/Diagram/declaration.svg
A parameter is a named variable inside a function’s block which will be assigned the value of the argument passed in when the function is invoked:https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-functions/Diagram/function+parameters.svg
To call a function in your code:https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-functions/Diagram/name.svg
ES6 introduces new ways of handling arbitrary parameters through default parameters which allow us to assign a default value to a parameter in case no argument is passed into the function.
To return a value from a function, we use a return statement.
To define a function using function expressions:https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-functions/Diagram/expression.svg
To define a function using arrow function notation:https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-functions/Diagram/arrow+notation.svg
Function definition can be made concise using concise arrow notation:https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-functions/Diagram/return.svg
https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-functions/Diagram/parameters.svg
https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-functions/Diagram/return.svg

Scope-
Scope is the idea in programming that some variables are accessible/inaccessible from other parts of the program.
Blocks are statements that exist within curly braces {}.
Global scope refers to the context within which variables are accessible to every part of the program.
Global variables are variables that exist within global scope.
Block scope refers to the context within which variables that are accessible only within the block they are defined.
Local variables are variables that exist within block scope.
Global namespace is the space in our code that contains globally scoped information.
Scope pollution is when too many variables exist in a namespace or variable names are reused.

Arrays-
Arrays are lists that store data in JavaScript.
Arrays are created with brackets [].
Each item inside of an array is at a numbered position, or index, starting at 0.
We can access one item in an array using its index, with syntax like: myArray[0].
We can also change an item in an array using its index, with syntax like myArray[0] = 'new string';
Arrays have a length property, which allows you to see how many items are in an array.
Arrays have their own methods, including .push() and .pop(), which add and remove items from an array, respectively.
Arrays have many methods that perform different tasks, such as .slice() and .shift(), you can find documentation at the Mozilla Developer Network website.
Some built-in methods are mutating, meaning the method will change the array, while others are not mutating. You can always check the documentation.
Variables that contain arrays can be declared with let or const. Even when declared with const, arrays are still mutable. However, a variable declared with const cannot be reassigned.
Arrays mutated inside of a function will keep that change even outside the function.
Arrays can be nested inside other arrays.
To access elements in nested arrays chain indices using bracket notation.

Review
Great job! In this lesson, we learned how to write cleaner code with loops. You now know:

Loops perform repetitive actions so we don’t have to code that process manually every time.
How to write for loops with an iterator variable that increments or decrements
How to use a for loop to iterate through an array
A nested for loop is a loop inside another loop
while loops allow for different types of stopping conditions
Stopping conditions are crucial for avoiding infinite loops.
do...while loops run code at least once— only checking the stopping condition after the first execution
The break keyword allows programs to leave a loop during the execution of its block

HIGHER-ORDER FUNCTIONS
Abstraction allows us to write complicated code in a way that’s easy to reuse, debug, and understand for human readers
We can work with functions the same way we would any other type of data including reassigning them to new variables
JavaScript functions are first-class objects, so they have properties and methods like any object
Functions can be passed into other functions as parameters
A higher-order function is a function that either accepts functions as parameters, returns a function, or both
Example-
const timeFuncRuntime = funcParameter => {
   let t1 = Date.now();
   funcParameter();
   let t2 = Date.now();
   return t2 - t1;
}

const addOneToOne = () => 1 + 1;

timeFuncRuntime(addOneToOne);
We wrote a higher-order function, timeFuncRuntime(). It takes in a function as an argument, saves a starting time, invokes the callback function, records the time after the function was called, and returns the time the function took to run by subtracting the starting time from the ending time.
This higher-order function could be used with any callback function which makes it a potentially powerful piece of code.
We then invoked timeFuncRuntime() first with the addOneToOne() function - note how we passed in addOneToOne and did not invoke it.

Iterators ->
https://s3.amazonaws.com/codecademy-content/courses/learn-javascript-iterators/iterator+anatomy.svg
//groceries.forEach(groceryItem => console.log(groceryItem));
//fruits.forEach(_ => console.log(`I want to eat a ${_}`));




Iterators->https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array
.forEach() is used to execute the same code on every element in an array but does not change the array and returns undefined.
.map() executes the same code on every element in an array and returns a new array with the updated elements.
.filter() checks every element in an array to see if it meets certain criteria and returns a new array with the elements that return truthy for the criteria.
.findIndex() returns the index of the first element of an array which satisfies a condition in the callback function. It returns -1 if none of the elements in the array satisfies the condition.
.reduce() iterates through an array and takes the values of the elements and returns a single value.
All iterator methods takes a callback function that can be pre-defined, or a function expression, or an arrow function.
You can visit the Mozilla Developer Network to learn more about iterator methods (and all other parts of JavaScript!).

Examples-
const cities = ['Orlando', 'Dubai', 'Edinburgh', 'Chennai', 'Accra', 'Denver', 'Eskisehir', 'Medellin', 'Yokohama'];

const nums = [1, 50, 75, 200, 350, 525, 1000];

//  Choose a method that will return undefined
cities.forEach(city => console.log('Have you visited ' + city + '?'));

// Choose a method that will return a new array
const longCities = cities.filter(city => city.length > 7);

// Choose a method that will return a single value
const word = cities.reduce((acc, currVal) => {
  return acc + currVal[0]
}, "C");

console.log(word)

// Choose a method that will return a new array
const smallerNums = nums.map(num => num - 5);

// Choose a method that will return a boolean value
nums.some(num => num < 0);



Objects ->
Objects store collections of key-value pairs.
Each key-value pair is a property—when a property is a function it is known as a method.
An object literal is composed of comma-separated key-value pairs surrounded by curly braces.
You can access, add or edit a property within an object by using dot notation or bracket notation.
We can add methods to our object literals using key-value syntax with anonymous function expressions as values or by using the new ES6 method syntax.
We can navigate complex, nested objects by chaining operators.
Objects are mutable—we can change their properties even when they’re declared with const.
Objects are passed by reference— when we make changes to an object passed into a function, those changes are permanent.
We can iterate through objects using the For...in syntax.


 Advanced Objects!
 The object that a method belongs to is called the calling object.
The this keyword refers the calling object and can be used to access properties of the calling object.
Methods do not automatically have access to other internal properties of the calling object.
The value of this depends on where the this is being accessed from.
We cannot use arrow functions as methods if we want to access other internal properties.
JavaScript objects do not have built-in privacy, rather there are conventions to follow to notify other developers about the intent of the code.
The usage of an underscore before a property name means that the original developer did not intend for that property to be directly changed.
Setters and getter methods allow for more detailed ways of accessing and assigning properties.
Factory functions allow us to create object instances quickly and repeatedly.
There are different ways to use object destructuring: one way is the property value shorthand and another is destructured assignment.
As with any concept, it is a good skill to learn how to use the documentation with objects!




Classes are templates for objects.
Javascript calls a constructor method when we create a new instance of a class.
Inheritance is when we create a parent class with properties and methods that we can extend to child classes.
We use the extends keyword to create a subclass.
The super keyword calls the constructor() of a parent class.
Static methods are called on the class, but not on instances of the class.


BROWSER COMPATIBILITY AND TRANSPILATION

ES5 — The old JavaScript version that is supported by all modern web browsers.
ES6 — The new(er) JavaScript version that is not supported by all modern web browsers. The syntax is more readable, similar to other programming languages, and addresses the source of common bugs in ES5.
caniuse.com — a website you can use to look up HTML, CSS, and JavaScript browser compatibility information.
Babel — A JavaScript package that transpiles JavaScript ES6+ code to ES5.
npm init — A terminal command that creates a package.json file.
package.json — A file that contains information about a JavaScript project.
npm install — A command that installs Node packages.
babel-cli — A Node package that contains command line tools for Babel.
babel-preset-env — A Node package that contains ES6+ to ES5 syntax mapping information.
.babelrc — A file that specifies the version of the JavaScript source code.
"build" script — A package.json script that you use to tranpsile ES6+ code to ES5.
npm run build — A command that runs the build script and transpiles ES6+ code to ES5.
For future reference, here is a list of the steps needed to set up a project for transpilation:

Initialize your project using npm init and create a directory called src
Install babel dependencies by running
npm install babel-cli -D
npm install babel-preset-env -D
Create a .babelrc file inside your project and add the following code inside it:
{
  "presets": ["env"]
}
Add the following script to your scripts object in package.json:
"build": "babel src -d lib"
Run npm run build whenever you want to transpile your code from your src to lib directories.



Modules-
Review
We just learned how to use JavaScript modules. Let’s review what we learned:

Modules in JavaScript are reusable pieces of code that can be exported from one program and imported for use in another program.

module.exports exports the module for use in another program.
require() imports the module for use in the current program.
ES6 introduced a more flexible, easier syntax to export modules:
 default exports use export default to export JavaScript objects, functions, and primitive data types.
 named exports use the export keyword to export data in variables.
 named exports can be aliased with the as keyword.
 import is a keyword that imports any object, function, or data type.



Promise-
Promises are JavaScript objects that represent the eventual result of an asynchronous operation.
Promises can be in one of three states: pending, resolved, or rejected.
A promise is settled if it is either resolved or rejected.
We construct a promise by using the new keyword and passing an executor function to the Promise constructor method.
setTimeout() is a Node function which delays the execution of a callback function using the event-loop.
We use .then() with a success handler callback containing the logic for what should happen if a promise resolves.
We use .catch() with a failure handler callback containing the logic for what should happen if a promise rejects.
Promise composition enables us to write complex, asynchronous code that’s still readable. We do this by chaining multiple .then()‘s and .catch()‘s.
To use promise composition correctly, we have to remember to return promises constructed within a .then().
We should chain multiple promises rather than nesting them.
To take advantage of concurrency, we can use Promise.all().


ASYNC AWAIT- async is keyword that tell its a async function and await is a operator that haults funciton till promise comes back
sync...await is syntactic sugar built on native JavaScript promises and generators.
We declare an async function with the keyword async.
Inside an async function we use the await operator to pause execution of our function until an asynchronous action completes and the awaited promise is no longer pending .
await returns the resolved value of the awaited promise.
We can write multiple await statements to produce code that reads like synchronous code.
We use try...catch statements within our async functions for error handling.
We should still take advantage of concurrency by writing async functions that allow asynchronous actions to happen in concurrently whenever possible.


Request 1-
avaScript is the language of the web because of its asynchronous capabilities. AJAX, which stands for Asynchronous JavaScript and XML, is a set of tools that are used together to take advantage of JavaScript’s asynchronous capabilities.
There are many HTTP request methods, two of which are GET and POST.
GET requests only request information from other sources.
POST methods can introduce new information to other sources in addition to requesting it.
GET requests can be written using an XMLHttpRequest object and vanilla JavaScript.
POST requests can also be written using an XMLHttpRequest object and vanilla JavaScript.
Writing GET and POST requests with XHR objects and vanilla JavaScript requires constructing the XHR object using new, setting the responseType, creating a function that will handle the response object, and opening and sending the request.
To add a query string to a URL endpoint you can use ? and include a parameter.
To provide additional parameters, use & and then include a key-value pair, joined by =.
Determining how to correctly write the requests and how to properly implement them requires carefully reading the documentation of the API with which you’re working.


Review Requests II
Let’s recap on the concepts covered in the previous exercises:
GET and POST requests can be created a variety of ways.
Use AJAX to asynchronously request data from APIs. fetch() and async/await are new functionalities developed in ES6 (promises) and ES8 respectively.
Promises are a new type of JavaScript object that represent data that will eventually be returned from a request.
fetch() is a web API that can be used to create requests. fetch() will return promises.
We can chain .then() methods to handle promises returned by fetch().
The .json() method converts a returned promise to a JSON object.
async is a keyword that is used to create functions that will return promises.
await is a keyword that is used to tell a program to continue moving through the message queue while a promise resolves.
await can only be used within functions declared with async.

  
  
  
