# JavaScriptFundamentals
Aim: To understand fundamentals of JavaScript in which as foundation for me to be excellence as FE Developer


Learning Source: FreeCodeCamp

[freeCodeCamp.org](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/)

- **Comment**: Comment in code will help to clarify the function and part of code, and will help us to later figure out what the code actually does
    
    ```jsx
    // This is an in-line comment
    ```
    
    ```jsx
    /*  this is a 
    multi-line comment */
    ```
    
- **Variable**:  a simple name to represent the data we want to refer to, which could contain or store eight different data types in Javascript, which are:
    
    [JavaScript Data Types](https://www.w3schools.com/js/js_datatypes.asp)
    
    [JavaScript data types and data structures - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures)
    
    Primitive: [https://developer.mozilla.org/en-US/docs/Glossary/Primitive](https://developer.mozilla.org/en-US/docs/Glossary/Primitive)
    
    In [JavaScript](https://developer.mozilla.org/en-US/docs/Glossary/JavaScript), a **primitive** (primitive value, primitive data type) is data that is not an [object](https://developer.mozilla.org/en-US/docs/Glossary/Object) and has no [methods](https://developer.mozilla.org/en-US/docs/Glossary/Method). There are 7 primitive data types: [string](https://developer.mozilla.org/en-US/docs/Glossary/String), [number](https://developer.mozilla.org/en-US/docs/Glossary/Number), [bigint](https://developer.mozilla.org/en-US/docs/Glossary/BigInt), [boolean](https://developer.mozilla.org/en-US/docs/Glossary/Boolean), [undefined](https://developer.mozilla.org/en-US/docs/Glossary/undefined), [symbol](https://developer.mozilla.org/en-US/docs/Glossary/Symbol), and [null](https://developer.mozilla.org/en-US/docs/Glossary/Null).
    
    How & Rules:
    
    - JavaScript evaluates expressions from left to right.
    - 
    
    What:
    
    `undefined`
    
    variable without a value has `undefined` as a value, and can be assigned to undefined as `undefined` types. but if the variable assigned to be empty value with strings, so the value gonna be empty with type data as strings.
    
    ```jsx
    var me; // Value is undefined, type is undefined
    var me = undefined // Value is undefined, type is undefined
    var me = ""; // the value is "", the typeof is "string"
    ```
    
    `null`
    
    null type has only one value: `null` , as invalid object or represents absence of any object value. but compared to undefined, null only has the equality with undefined but not as identity.
    
    null also mean pointing to not pointing to any object, and expected that no object is relevant to those.
    
    ```jsx
    null === undefined   // false
    null  == undefined   // true
    ```
    
    `boolean`,
    
    have two value, `true` or `false` , booleans often used on conditional testing.
    
    ```jsx
    var x = 7;
    var y = 7;
    var x = 10;
    
    (x == y) // return true
    (x == z) // return false
    ```
    
    `string`, 
    
    String written with quotes, we can use single or double quotes, and we can use quotes inside a string, as long they doesn’t match with the surrounding quotes.
    
    ```jsx
    var myName1 = "Apis" // using double quotes
    var myName2 = 'Apis' // using single quotes
    var wordA = "It's okay" // single inside double
    var wordB = "Absolutely, called me 'Apis'" //single inside double
    var wordC = 'Absolutely, called me "Apis"' // double insude single
    ```
    
    `symbol`
    
    A Symbol is a **unique** and **immutable** primitive value and may be used as the key of an Object property. more about symbols check here: [https://developer.mozilla.org/en-US/docs/Glossary/Symbol](https://developer.mozilla.org/en-US/docs/Glossary/Symbol)
    
     *ps: I still don’t know when to use this* 😄
    
    `bigint` 
    
    BigInt is a numeric primitive, can represent integers, we can use the operators `+ * - **`and `%` with BigInts—just like with Numbers. A BigInt is not strictly equal to a Number,
    
    *ps: I still don’t know when to use this* 😄
    
    `number` 
    
    number can write with pr without a decimals, and large numbers can be write with scientific notation
    
    ```jsx
    var x1 = 30.9 // with decimals
    var x2 = 77 // without decimals
    var x3 = 123e5 // 12300000
    var x4 = 123e-5 // 0.00123
    ```
    
    `object`
    
    written with curly braces `{}`, separated by commas, its has direct value pairs, object as well called the collection of properties.
    
    ```jsx
    const me = {nickName:'Apis', age:28, favColor:"black"};
    ```
    
    `arrays`
    
    written with square brackets, separated by commas, array index starting from zero, which first item gonna be [0], and the next is [1], and so on.
    
    ```jsx
    const pets = ['cat', 'dog', 'fish'];
    ```
    
    to declare a variable, use `var` then `theName` of variable, and ends with semicolon 
    
    ```jsx
    var myName;
    ```
    

- camelCase
    
    Write variable names in JavaScript in *camelCase*. In *camelCase*, multi-word variable names have the first word in lowercase and the first letter of each subsequent word is capitalized.
    
    ```jsx
    var someVariable;
    var anotherVariableName;
    var thisVariableNameIsSoLong;
    ```
    
    It is strongly recommended that for the sake of clarity
    
- var, let & const
    
    One of the biggest problems with declaring variables with the `var`keyword is that you can easily overwrite variable declarations
    
    In a small application, you might not run into this type of problem. But as your codebase becomes larger, you might accidentally overwrite a variable that you did not intend to. Because this behavior does not throw an error, searching for and fixing bugs becomes more difficult.
    
    So unlike `var`, when you use `let`, a variable with the same name can only be declared once. 
    
    const comes in different way, as new feature in ES6, that variables declared using `const` are read-only. They are a constant value, which means that once a variable is assigned with `const`, it cannot be reassigned:
    
    ```jsx
    var me = 'Apis';
    var me = 'Nakula';
    console.log(me); // Nakula
    
    //unlike var, using let can return error, 
    // because the similar variable with same name can only declare once
    let me = 'Apis';
    let me = 'Nakula';
    console.log(me); // error
    
    // const means constant, and shared similar feature that let has,
    // but const only has one-time assigned
    const whatIsmyName = 'Apis';
    whatIsmyName = 'Nakula';
    console.log(whatIsmyName); // error
    ```
    

Progress December 31, 2021 Day 1 of #100DaysOfCode 

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/903893ac-dd8a-47d3-8b39-af4802f41335/Untitled.png)

Day 2 of #100DaysOfCode 

- JS Math operators
    
    Subtract ( `-` ); multiply ( `*` ); divide ( `/` );  increment ( `++  → i++`); decrement ( `-- → i--`); decimal (decimal numbers often referred as *floating point* numbers, in JS also works for multiplying or divides decimals); remainder ( `%` ) → gives the remainder of the division of two numbers: according to MDN → The remainder operator (`%`) returns the remainder left over when one operand is divided by a second operand. It always takes the sign of the dividend.
    
    ```jsx
    // Example of reminder
    const remainder = 11 % 3; // return 2, 
    // because Math.floor( 11 / 3) = 3 (Quotient)
    // 3 * 3 = 9 
    // 11 - 9 = 2 (Remainder)
    
    // Remainder (%) operator most often used in?
    ```
    
    - to compound assignment, we can use augmented audition using `+=` operator, for instance:
        
        ```jsx
        let myApis = 1;
        myApis += 5;
        console.log(myApis); // 6
        ```
        
    - compound assignment works as well for subtraction, multiplication, & division , by following :
        
        ```jsx
        // subtraction
        let myApis = myApis - 7;
        //can be written as follow
        myApis -= 7;
        
        // multiplication
        let myApis = myApis * 7;
        //can be written as follow
        myApis *= 7;
        
        // division
        let myApis = myApis / 7;
        //can be written as follow
        myApis /= 7;
        ```
        
    
- Strings in JavaScript:
    - When you’d like to write quotes inside a string, we can use backslash (\) in front:
        
        ```jsx
        const sampleWords= "Apis said, \"Nakula currently sleeping\".";
        // return -> Apis said, "Nakula currently sleeping".
        ```
        

- Quoting strings also works on singles quotes:
    
    ```jsx
    const goodStr = 'Jake asks Finn, "Hey, let\'s go on an adventure?"'; 
    const badStr = 'Finn responds, "Let's go!"';
    
    // by adding backslash before ( ' ) will make it not reads as end of the strings
    ```
    
- How to escape sequence in strings?
    
    [freeCodeCamp.org](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/escape-sequences-in-strings)
    

- Concatenating Strings with Plus Operator
    
    we can combine two strings in a row by using plus operator in JS, but this plus (+) operator between the two strings will not act as space, so we gotta adding manually on each strings respectively
    
    ```jsx
    const ourStr = "I come first. " + "I come second."; // I come first. I come second.
    ```
    

- when we dealing with long strings that could be turn into several lines, so very helpful using Plus Equal Operators `+=`
    
    ```jsx
    let ourStr = "I come first. ";
    ourStr += "I come second.";
    
    // I come first. I come second.
    ```
    
- When we’d like using reference variable that has certain value (constant or changing), we can insert one or more variables into a string using `+` operator
    
    ```jsx
    const myName = "Apis";
    const greeting = "Hello, my name is " + myName + ", and you?";
    // Hello, my name is Apis, and you?
    ```
    
- `+=` operator also can be used when we’d like to appending variables into strings,
    
    ```jsx
    const anAdjective = "awesome!";
    let ourStr = "freeCodeCamp is ";
    ourStr += anAdjective;
    
    // ourStr would have the value -> freeCodeCamp is awesome!.
    ```
    
- Somehow we’d like to identify the length of a String in some cases, to find out, using `.length` after the variable name would return us how much character’s length for those variable:
    
    ```jsx
    let lastNameLength = 0;
    const lastName = "Lovelace";
    lastNameLength = lastName.length;
    
    console.log(lastNameLength); // 8
    ```
    
- To get specific character in a string, we can find the index by using Bracket Notation `[]` , because Javascript was Zero-based indexing, so all the index will start with`[0]`
    
    ```jsx
    const firstName = "Apis";
    const firstLetter = firstName[0];
    
    console.log(firstLetter); // A
    ```
    

- String in JavaScript is immutable, its means that they cannot be altered once created, the only way to change by assign new strings, but cannot just one character for the value of those variable.


Day 3 of #100DaysOfCode 20:00-22:00

- In order to target specific sequence character in a string, we could mentioned index sequence in a bracket `myStr[2]`, and as well to identify last character in a string, we could use `.length -1` , and also works if we’d like to Find the Nth-to-Last Character in a String
    
    ```jsx
    const lastName = "Lovelace";
    
    // identify last character in a string
    const lastLetterOfLastName = lastName[lastName.length-1];
    console.log(lastLetterOfLastName); // e
    
    // Find the Nth-to-Last Character in a String
    const secondToLastLetterOfLastName = lastName[lastName.length - 2];
    console.log(secondToLastLetterOfLastName); // c
    ```
    

- JS Array `[]` also can store values, the value might vary based on our needs, we declare the value inside bracket with comma to separate each value. And nested arrays also works inside an array, incase we’d like to grouping several values
    
    ```jsx
    const myArray = ["Fish", 7];
    console.log(myArray); // [Fish, 7]
    
    // nested array
    const myArray = [["Fish", 7], ["Fish2", 8]];
    console.log(myArray); // ["Fish", 7], ["Fish2", 8]
    ```
    
- To access Array data, we can use indexes, as similar to strings, array index use zero-based indexing method.
    
    Arrays value are mutable, so it highly possible to changes and assign to new value, unlike strings.
    
    With multidimensional arrays, accessing index also has similar approach but with following next pointed index as referring next level entries inside.
    
    ```jsx
    const myArray = [50, 60, 70];
    const myData = myArray[0];
    console.log(myData); // 50
    
    // Modify array value
    const myArray = [18, 64, 99];
    myArray[0] = 45;
    console.log(myArray); //[45, 64, 99]
    
    // multi-dimensional array
    const myArray = [
      [1, 2, 3],
      [4, 5, 6],
      [7, 8, 9],
      [[10, 11, 12], 13, 14],
    ];
    const myData = myArray[2][1];
    console.log(myData); // 8
    ```
    
- Manipulating arrays
    
    `.push()` often use to append data to the end of an array, means `.push()` function will add new value inside the arrays.
    
    if we’d like to dismiss end of array’s value, using `.pop()` function will removes the last element from an array and return those elements
    
    `.shift()` function was the opposite of `.pop()` function, it would removes our first element in arrays
    
    When it comes to adding new value in the first element of an array, `.unshift()` function will add them as the opposite `.push()`
    
    ```jsx
    // .push()
    const myArray = [["John", 23], ["cat", 2]];
    myArray.push(["dog", 3]);
    console.log(myArray); //[ [ 'John', 23 ], [ 'cat', 2 ], [ 'dog', 3 ] ]
    
    // .pop()
    const myArray = [["John", 23], ["cat", 2]];
    const removedFromMyArray = myArray.pop();
    console.log(removedFromMyArray); //[ 'cat', 2 ]
    console.log(myArray); //[ [ 'John', 23 ] ]
    
    // .shift()
    const myArray = [["John", 23], ["dog", 3]];
    const removedFromMyArray = myArray.shift();
    console.log(myArray); // [ 'dog', 3 ]
    
    // .unshift()
    const myArray = [["John", 23], ["dog", 3]];
    myArray.shift();
    myArray.unshift(["Paul", 35]);
    console.log(myArray); // [ [ 'Paul', 35 ], [ 'dog', 3 ] ]
    ```
    
- Functions in JavaScript are reusable, and it will be print the result every time those functions being called in dev console.
    
    Every functions use parameters to passing a values, parameters are variable that act as placeholders for the values that are to be input to a function when it is called
    
    ```jsx
    function reusableFunction() {
      console.log("Hi World");
    }
    reusableFunction(); // Hi World
    
    // passing values with arguments
    function functionWithArgs(a,b) {
      console.log(a+b);
    }
    functionWithArgs(7,9); //16
    functionWithArgs(1,2); //3
    ```
    
    we also can return value from a function with `return`
    
    ```jsx
    function timesFive(n) {
      return n * 5;
    }
    const answer = timesFive(5);
    console.log(answer); //25
    ```
    
    
    Day 4 of #100DaysOfCode #FCC

- Global Scope & Function
    
    Scope in JS means visibility or access ranges that variables had once it declared. If we didn’t use `let` or `const` at the outside of function, then the variables became global scope: which has override consequence if we use similar variables in other place.
    
    ```jsx
    const myGlobal = 10;
    function fun1() {
      // Assign 5 to oopsGlobal Here
       oopsGlobal = 5;
    }
    function fun2() {
      var output = "";
      if (typeof myGlobal != "undefined") {
        output += "myGlobal: " + myGlobal;
      }
      if (typeof oopsGlobal != "undefined") {
        output += " oopsGlobal: " + oopsGlobal;
      }
      console.log(output); // myGlobal: 10 oopsGlobal: 5
    }
    
    ```
    
- Local Scope & Function
    
    Local scope means any variables that declare within a function, and this variable cannot be access from outside of those function
    
    ```jsx
    function myLocalScope() {
      // Only change code below this line
      const myVar = "Apis";
    
      console.log('inside myLocalScope', myVar); // inside myLocalScope Apis
    }
    myLocalScope(); // ReferenceError: Can't find variable: myVar
    ```
    
    If the similar variable name was declared in local and global scope, it still works well & highly possible, and they will return the assigned value each of them.
    
    ```jsx
    const outerWear = "T-Shirt";
    
    function myOutfit() {
      const outerWear = "sweater";
      return outerWear;
    }
    
    myOutfit(); // sweater
    ```
    
- Function returning undefined value
    
    Normally function will proceed inner code that assigned to them, but it would returning `undefined` of there is no `return` statement inside the function
    
- Queue is an abstract Data Structure where items are kept in order, for any new item will be add at the back of the order, and old item will taken off from the front queue
    
    ```jsx
    
    ```
    
    ##Day 5 of #100DaysOfCode #FCC

- Boolean Values
    
    Boolean has two values, it was `true` and `false`, without a string when to write them in JS
    
- If Statement
    
    If will be used to create a decision when the function return `true` then logic inside curly braces will be executed, and it will not runs when hit `false`
    
    ```jsx
    function trueOrFalse(wasThatTrue) {
    if(wasThatTrue) {
      return "Yes, that was true";
    } return "No, that was false";
    }
    ```
    
- Comparison Operators
    
    When we’d like to compare the equality between two values, we could use `==` which wud return boolean ( true or false). 
    
    ```jsx
    function testEqual(val) {
      if (val == 12) {  
        return "Equal";
      }
      return "Not Equal";
    }
    testEqual(10); // Not Equal
    ```
    
    Unlike the equality operator, Strict Equality ( `===` ) will not perform any type of similarity conversion, the comparing value should be has share similar type or value.
    
    ```jsx
    function testStrict(val) {
      if (val === 7) {
        return "Equal";
      }
      return "Not Equal";
    }
    testStrict(10); // Not Equal
    ```
    
    Inequality Operator ( `≠` → `!`(no space)`=` ) is the opposite of `==` , which wud be return `false`, 
    
    ```jsx
    function testNotEqual(val) {
      if ( val != 99) { 
        return "Not Equal";
      }
      return "Equal";
    }
    testNotEqual(10);
    ```
    
    And Strict Equality also has the opposite comparison operator, that was Strict Inequality (`! ==`), which means strict not equal and return `false`, 
    
    ```jsx
    function testStrictNotEqual(val) {
      if (val !== 17) {  
        return "Not Equal";
      }
      return "Equal";
    }
    testStrictNotEqual(10);
    ```
    
    Greater Than Operator (`>`) also works like equality operator, it will be convert data types of value when comparing, and will return `true` when number on left side is greater than right side
    
    ```jsx
    function testGreaterThan(val) {
      if (val > 100 ) {  
        return "Over 100";
      }
      if (val > 10) {  
        return "Over 10";
      }
      return "10 or Under";
    }
    testGreaterThan(10);
    ```
    
    `≥`  (Greater Than Or Equal To) was used to compares two numbers, and it works like the `>` operator, but including the left number as baseline comparison
    
    ```jsx
    function testGreaterOrEqual(val) {
      if (val >= 20 ) {   
        return "20 or Over";
      }
      if (val >= 10 ) {   
        return "10 or Over";
      }
      return "Less than 10";
    }
    testGreaterOrEqual(10);
    ```
    
    Less Than Operator (`<`), works the opposite way of Greater Than Operator.
    
    ```jsx
    function testLessThan(val) {
      if (val < 25) { 
        return "Under 25";
      }
      if (val < 55 ) {   
        return "Under 55";
      }
      return "55 or Over";
    }
    testLessThan(10);
    ```
    
    Less Than or Equal To Operator ( `≤`), works the opposite way of `≥`
    
    ```jsx
    function testLessOrEqual(val) {
      if (val <= 12 ) {  
        return "Smaller Than or Equal to 12";
      }
      if (val <= 24 ) {  
        return "Smaller Than or Equal to 24";
      }
      return "More Than 24";
    }
    testLessOrEqual(10);
    ```
    
    Comparison with Logical And Operator (`&&`), will return `true` if the *operands* to the left and right of it are true
    
    ```jsx
    function testLogicalAnd(val) {
      if (val <= 50 && val >= 25) {
          return "Yes";
      }
      return "No";
    }
    testLogicalAnd(10);
    ```
    
    Logical Or Operator (`||`), will return `true` if the *operands* to the left and right of it are true, otherwise `false`
    
    ```jsx
    function testLogicalOr(val) {
      if (val < 10 || val > 20) {
        return "Outside";
      } 
      return "Inside";
    }
    testLogicalOr(15); // Inside
    ```
    

- Else & Switch Statements
    
    Following block of code will execute when the if statement is true, but if not, the alternate one (after the first code statement) will execute.
    
    ```jsx
    function testElse(val) {
      let result = "";
      if (val > 5) {
        result = "Bigger than 5";
      } else {
        result = "5 or Smaller";
        }
      return result;
      
    }
    testElse(4);
    ```
    
    multiple condition if statements also known as `else if` statements
    
    ```jsx
    function testElseIf(val) {
      if (val > 10) {
        return "Greater than 10";
      } else if (val < 5) {
        return "Smaller than 5";
      } else {
      return "Between 5 and 10";
      }
    }
    testElseIf(7);
    ```
    
    both `if` and `else if` statement will apply sequence order from top to bottom, so we had to carefully craft them
    
    ```jsx
    function orderMyLogic(val) {
      if (val < 5) {
        return "Less than 5";
      } else if 
        (val < 10) {
        return "Less than 10";
      } else {
        return "Greater than or equal to 10";
      }
    }
    
    orderMyLogic(7);
    ```
    
    `switch` statements : A `switch` statement tests a value and can have many *case* statements which define various possible values. Statements are executed from the first matched `case` value until a `break` is encountered.
    
    ```jsx
    function caseInSwitch(val) {
      let answer = "";
        switch(val) {
        case 1:
          answer = "alpha";
          break;
        case 2:
          answer = "beta";
          break;
        case 3:
          answer = "gamma";
          break;
        case 4:
          answer = "delta";
          break;}
      return answer;
    }
    
    caseInSwitch(1);
    ```
    
    We also can set default switch statement as final statement if none of case would match
    
    ```jsx
    function switchOfStuff(val) {
      let answer = "";
     switch(val) {
       case "a":
        answer = "apple";
        break;
      case "b":
        answer = "bird";
        break;
      case "c":
        answer = "cat";
        break;
      default:
        answer = "stuff";
        break
     }
      return answer;
    }
    
    switchOfStuff(1);
    ```
    
    switch statement with multiple inputs with the same output also can perform in group like this one
    
    ```jsx
    function sequentialSizes(val) {
      let answer = "";
      switch(val) {
        case 1:
        case 2:
        case 3:
          answer = "Low";
          break;
        case 4:
        case 5:
        case 6:
          answer = "Mid";
          break;
        case 7:
        case 8:
        case 9:
          answer = "High";
          break;
      }
      return answer;
    }
    
    sequentialSizes(1);
    
    //---------
    // If you have many options to choose from, 
    // a switch statement can be easier to write than many chained 
    // if/else if statements. The following:
    
    function chainToSwitch(val) {
      let answer = "";
      // Only change code below this line
    if (val === 1) {
      answer = "a";
    
    // into
    switch(val) {
      case 1:
        answer = "a";
        break;
    
    // ------------
    
    // sample
    switch(val){
      case "bob":
        answer = "Marley";
        break;
      case 42:
        answer = "The Answer";
        break;
      case 1:
        answer = "There is no #1";
        break;
      case 99:
        answer = "Missed me by this much!";
        break;
      case 7:
        answer = "Ate Nine";
        break;
    }
      return answer;
    }
    
    ```
    Day 6 of #100DaysOfCode

- `RegEx`  is AN object is used for matching text with a pattern.
    
    [RegExp - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp)
    
    ```jsx
    let count = 0;
    
    function cc(card) {
      var regex = /[JQKA]/;
      if (card > 1 && card < 7) {
        count++;
      } else if (card === 10 || regex.test(card)) {
        count--;
      }
      if (count > 0) return count + " Bet";
      return count + " Hold";
    }
    cc(2); cc(3); cc(7); cc('K'); cc('A');
    ```
    
- JavaScript Object
    
    In most cases Object are similar to an arrays, to access and modify object data, we can use `properties` , Object being used to store data in a structured way, and can represent real world objects.
    
    ```jsx
    const myDog = {
      "name": "puppy",
      "legs": 4,
      "tails": 1,
      "friends": ["cats", "lion", "tiger"],
    };
    ```
    
    to access object properties, we can use Dot Notation ( `.` ), and bracket notation `[]`. Dot Notation are used when we know the name of the properties.
    
    ```jsx
    const testObj = {
      "hat": "ballcap",
      "shirt": "jersey",
      "shoes": "cleats"
    };
    const hatValue = testObj.hat;  // ballcap
    const shirtValue = testObj.shirt; // jersey
    
    // using Bracket Notation
    const testObj = {
      "an entree": "hamburger",
      "my side": "veggies",
      "the drink": "water"
    };
    const entreeValue = testObj['an entree'];   
    const drinkValue = testObj['the drink'];   
    
    // another exercise
    const testObj = {
      12: "Namath",
      16: "Montana",
      19: "Unitas"
    };
    const playerNumber =  16 
    const player = testObj[playerNumber]; // Montana
    ```
    
    Object properties also can be updated, we can use either dot or bracket notation to update.
    
    ```jsx
    const myDog = {
      "name": "Coder",
      "legs": 4,
      "tails": 1,
      "friends": ["freeCodeCamp Campers"]
    };
    myDog.name = "Happy Coder";
    ```
    
    To add new properties to JavaScript Object, as the similar way to modify the properties itself:
    
    ```jsx
    const myDog = {
      "name": "Happy Coder",
      "legs": 4,
      "tails": 1,
      "friends": ["freeCodeCamp Campers"]
    };
    myDog.bark = "woof";
    console.log(myDog);
    
    /* { name: 'Happy Coder',
      legs: 4,
      tails: 1,
      friends: [ 'freeCodeCamp Campers' ],
      bark: 'woof' } */
    ```
    
    When we’d like to delete properties from JS Object, simply use `delete` properties like this:
    
    ```jsx
    const myDog = {
      "name": "Happy Coder",
      "legs": 4,
      "tails": 1,
      "friends": ["freeCodeCamp Campers"],
      "bark": "woof"
    };
    delete myDog.tails;
    console.log(myDog);
    ```
    
    Using Objects for Lookups.
    
    ```jsx
    function phoneticLookup(val) {
      let result= "";
      const lookup = {
        "alpha": "Adams",
        "bravo": "Boston",
        "charlie": "Chicago",
        "delta": "Denver",
        "echo": "Easy",
        "foxtrot": "Frank",
      };
      result = lookup[val];
      return result;
    }
    
    phoneticLookup("charlie");
    ```
    
    `.hasOwnProperty(propname)`  is method to determine if that object has the given property name.  `.hasOwnProperty()`returns `true` or `false` if the property is found or not.
    
    ```jsx
    function checkObj(obj, checkProp) {
      if (obj.hasOwnProperty(checkProp)) {
        return obj[checkProp];
      } else {
        return "Not Found";
      }
    }
    ```
 Day 7 of #100DaysOfCode

- Manipulating complex object
    
    a flexible Data Structure are commonly used in JavaScript, this flexible data can perform combinations of *strings, numbers, booleans, arrays, functions,* and *objects.*
    
    this approach also called JavaScript Object Notation or JSON: is a related data interchanges format used to store data:
    
    ```jsx
    const myMusic = [ 
    {
      "artist": "Daft Punk",
      "title": "Homework",
      "release_year": 1997,
      "formats": [ 
        "CD",
        "Cassette",
        "LP"
      ],
      "gold": true
    	}
    ]
    ```
    

- Accessing nested objects
    
    To access the sub-properties of an objects, by chaining together the dot or bracket notation.
    
    ```jsx
    const myStorage = {
      "car": {
        "inside": {
          "glove box": "maps",
          "passenger seat": "crumbs"
         },
        "outside": {
          "trunk": "jack"
        }
      }
    };
    
    const gloveBoxContents = myStorage.car.inside["glove box"];
    ```
    
- Accessing nested arrays
    
    To access nested arrays is similar way on accessing nested objects, array bracket notation can be chained to access nested arrays.
    
    ```jsx
    const myPlants = [
      {
        type: "flowers",
        list: [
          "rose",
          "tulip",
          "dandelion"
        ]
      },
      {
        type: "trees",
        list: [
          "fir",
          "pine",
          "birch"
        ]
      }
    ];
    const secondTree = myPlants[1].list[1]; // pine
    ```
    

- JavaScript While Loops
    
    while loops will runs when a specific condition is true and stops once that conditions is no longer true
    
    ```jsx
    // Setup
    const myArray = [];
    let i = 5;
    while (i >= 0) {
      myArray.push(i);
      i--;
    }
    console.log(myArray); // [5,4,3,2,1,0]
    ```
    
- JavaScript For Loops
    
    for loop has declared with three optional expressions separated by semicolons:
    
    `for (a; b; c)`, where `a` is the initialization statement, `b` is the condition statement, and `c` is the final expression.
    
    ```jsx
    const myArray = [];
    for (let i = 1; i < 6; i++) {
      myArray.push(i);
    }
    console.log(myArray); //[ 1, 2, 3, 4, 5 ]
    ```
    
    How if we’d like to iterate Odd Numbers with For Loop: For loops don't have to iterate one at a time. By changing our `final-expression`, we can count by even numbers.
    
    ```jsx
    const myArray = [];
    for (let i = 1; i < 10; i += 2 ) {
      myArray.push(i);
    }
    console.log(myArray)// [ 1, 3, 5, 7, 9 ]
    ```
    
    Counting backwards also can perform using For Loop, In order to decrement by two each iteration, we'll need to change our initialization, condition, and final expression.
    
    ```jsx
    const myArray = [];
    for (let i = 9; i > 0; i -= 2) {
      myArray.push(i);
    }
    console.log(myArray); // [ 9, 7, 5, 3, 1 ]
    ```
    
    For Loop also can be used for iterate through an array, by running the loop as long the `i` is equal to `length`.
    
    ```jsx
    const myArr = [2, 3, 4, 5, 6];
    let total = 0;
    for (let i= 0 ; i < myArr.length; i++  ) {
      total += myArr[i];
    }
    console.log(total); // 20
    ```
    
- JavaScript Do...While Loops
    
    It is called a `do...while` loop because it will first `do` one pass of the code inside the loop no matter what, and then continue to run the loop `while` the specified condition evaluates to `true`.
    
    what makes the `do...while` different from other loops is how it behaves when the condition fails on the first check. Essentially, a `do...while` loop ensures that the code inside the loop will run at least once.
    
    ```jsx
    const myArray = [];
    let i = 10;
     do {
      myArray.push(i);
      i++;
    } while (i < 5);
    ```
  
 Day 8 of #100DaysOfCode
- Replacing Loops with Recursion is the concept can be expressed in terms of itself.
    

