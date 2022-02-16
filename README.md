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
- - Replacing Loops with Recursion is the concept can be expressed in terms of itself.
    
    ```jsx
    function sum(arr, n) {
      if(n <= 0) {
        return 0;
      } else {
        return sum(arr, n-1) + arr[n-1];
      }
    }
      console.log(sum([2,3,4], 1)) // 2
    ```
    
    ```jsx
    // exercise profile lookup
    const contacts = [
      {
        firstName: "Akira",
        lastName: "Laine",
        number: "0543236543",
        likes: ["Pizza", "Coding", "Brownie Points"],
      },
      {
        firstName: "Harry",
        lastName: "Potter",
        number: "0994372684",
        likes: ["Hogwarts", "Magic", "Hagrid"],
      },
      {
        firstName: "Sherlock",
        lastName: "Holmes",
        number: "0487345643",
        likes: ["Intriguing Cases", "Violin"],
      },
      {
        firstName: "Kristian",
        lastName: "Vos",
        number: "unknown",
        likes: ["JavaScript", "Gaming", "Foxes"],
      },
    ];
    // answer
    function lookUpProfile(name, prop) {
      for (let i = 0; i < contacts.length; i++) {
        if (contacts[i].firstName === name) {
          if(contacts[i].hasOwnProperty(prop)) {
            return contacts[i][prop]
          } else {
            return "No such property";
          }
        }
      }
      return "No such contact";
    }
    
    lookUpProfile("Akira", "likes");
    
    // explanation
    // The for loop runs, starting the first object in the contacts list
    // If the firstName parameter passed into the function matches the value of the "firstName" key in the first object, the if statement passes.
    // Then, we use .hasOwnPropertiy() to check with a prop as an argment, if it's was trus, the value of prop will returned
    // if statement of finding prop failes, "No such property" is returned
    // if the first if statements fails, for loop continues on the next object of contact list
    // If the firstName parameter isn’t matched by the final contacts object, the for loop exits and No such contact is returned.
    ```
    

- Random Fractions
    
    Random fractions in Javascript using `Math.random()` that generates a random decimal number between 0 and 1.
    
    ```jsx
    function randomFraction() {
      return Math.random();
    }
    console.log(randomFraction(2));// 0.3366139865105834
    ```
    
    we can also using random fraction to whole numbers, with helps multiply the `Math.random()` to certain numbers (eq. 20), then use `Math.floor()` to round down the number into nearest whole number.
    
    ```jsx
    function randomWholeNum() {
      return Math.floor(Math.random() * 10);
    }
    console.log(randomWholeNum(3));// 8
    ```
    
    To generate random whole numbers within a range, by define minimum numbers with min and a maximum number.
    
    ```jsx
    function randomRange(myMin, myMax) {
      return Math.floor(Math.random() * (myMax - myMin +1) + myMin);
    }
    ```
    

- Using `parseInt` function
    
    ```jsx
    function convertToInteger(str) {
     const a = parseInt(str);
     return a;
    }
    
    console.log(convertToInteger("56")); // 56
    ```
    
    The `parseInt()` function parses a string and returns an integer, 
    
    ```jsx
    function convertToInteger(str) {
      const a = parseInt(str, 2);
      return a;
    }
    console.log(convertToInteger("10011")); // 19
    ```
    
- **Conditional (Ternary) Operator**
    
    The syntax is `a ? b : c`, where `a` is the condition, `b` is the code to run when the condition returns `true`, and `c` is the code to run when the condition returns `false`.
    
    ```jsx
    function checkEqual(a, b) {
      return a == b ? "Equal" : "Not Equal";
    }
    
    console.log(checkEqual(1, 2)); // Not Equal
    ```
    
    ternary operator also works in multiple sequences,  by combine with `if`, `else if`, and `else` statements to check multiple conditions
    
    ```jsx
    function checkSign(num) {
     return (num > 0) ? "positive" 
     : (num < 0) ? "negative"
     : "zero";
    }
    console.log(checkSign(10)); // positive
    ```
    
    **Use Recursion to Create a Countdown**
    
    ```jsx
    function countdown(n){
      if (n < 1 ) {
        return [];
      } else {
        const array = countdown(n-1);
        array.unshift(n);
        return array;
      }
    }
    console.log(countdown(5));// [ 5, 4, 3, 2, 1 ]
    ```
    
    **Use Recursion to Create a Range of Numbers**
    
    ```jsx
    function rangeOfNumbers(startNum, endNum) {
      if ( endNum - startNum === 0) {
      return [startNum];
      } else {
        const arr  = rangeOfNumbers(startNum, endNum -1 );
        arr.push(endNum);
        return arr;
      }
    }
    
    console.log(rangeOfNumbers( 6,9)); // [ 6, 7, 8, 9 ]
    ```
   
   Day 9 of #100DaysOfCode

- Deep dive on Recursion
    
    [Recursion in Programming - Full Course](https://www.youtube.com/watch?v=IJDJ0kBx2LM)
    
    Recursion is nothing more than a method that calls itself. Condition that stopping the condition based on the Base Case, with looping Recursive Call.
    
    Trade Off: Pros
    
    - Bridges the gap between elegance & complexity
    - Reduce need for complex loops & auxiliary data structures, with implicit stacks, self manage looping contract
    - can reduce time complexity with memoization
    - works really well in trees, graphs, will focus on small tiny set recursive data structures
    
    Trade Off: Cons
    
    - slowness due to CPU overhead
    - Can lead to out memory errors / stack overflow exeptions
    - Can be unnecessary complex if poorly constructed
    
    Call Stack | Cases:
    
    We need to return value as base case to stop the function runs (stop invoking method)
    
    ```jsx
    public String reverseString(String input) {
    // what is the base case? (when can i no longer continue)
    // what is the smallest amount of work I can do in each iteration?
    ```
    
    - String Reversal
    - Palindrome
    - Decimal to Binary
    - Sum of Natural Numbers
    - Divide & Conquer
        - Binary Search
        - Fibonacci (Non-Optimized)
        - Merge Sort
        - Linked Lists
            - Reversal Linked Lists
            - Merge Two Sorted Linked Lists
   - Trees | The most works well with recursion
   - Insert Value Into Binary Search Tree
   - Print All Leaf Nodes
   - Graphs
        - Depth-First Seach
   - Optimization
        - Memoization & Caching
        - Tail-Call Recursion Optimization

<aside>
💡 As you considering the optimization technique, think about what language you’re using. and think about the compiler that you’re using and where your code is being executed to see if this sort of optimization is supported or not.

</aside>



ECMAScript -ES6
Day 10 of #100DaysOfCode
ES6 → Standardized version of JavaScript

- **Scopes of var & let**
    
    When variable declared with `var` keyword, then it wud be globally accessible, or locally if declared inside the function.
    
    and using `let` , will enables extra features: when let declared inside a block, statement or expression, its scope is limited to that block, statement, or expression.
    
    ```jsx
    function checkScope() {
      let i = 'function scope';
      if (true) {
        let i = 'block scope';
        console.log('Block scope i is: ', i);
      }
      console.log('Function scope i is: ', i);
      return i;
    }
    
    // Block scope i is:  block scope
    // Function scope i is:  function scope
    ```
    
- **Using `const` in JavaScript**
    
    Using the `const` declaration only prevents reassignment of the variable identifier. When const used on arrays and functions are still mutable.
    
- **Prevent Object from mutation**
    
    JavaScript provides a function `Object.freeze` to prevent data mutation.
    
    ```jsx
    function freezeObj() {
      const MATH_CONSTANTS = {
        PI: 3.14
      };
      Object.freeze(MATH_CONSTANTS);
      try {
        MATH_CONSTANTS.PI = 99;
      } catch(ex) {
        console.log(ex);
      }
      return MATH_CONSTANTS.PI;
    }
    const PI = freezeObj();
    console.log(PI); // 3.14
    ```
    
- **Arrow Functions**
    
    arrow function syntax allows you to omit the keyword `return` as well as the brackets surrounding the code. This helps simplify smaller functions into one-line statements:
    
    ```jsx
    const myFunc = () => "value";
    // also can be written like this
    const myFunc = function() {
      const myVar = "value";
      return myVar;
    }
    
    // both will return "value"
    ```
    
    Arrow function also used with parameters, just like regular function, it’s could be pass an arguments into arrow function.
    
    ```jsx
    const myConcat = (arr1, arr2) => {
      return arr1.concat(arr2);
    }
    console.log(myConcat([1, 2], [3, 4, 5])); // [ 1, 2, 3, 4, 5 ]
    ```
    
- **Default Parameters**
    
    In ES6, default parameters are given for help us to fill the argument when the argument is not specified, which the return value will shown as default parameter.
    
    ```jsx
    const increment = (number, value = 1) => number + value;
    console.log(increment(5)); // 6
    ```
    
- **Rest Parameters**
    
    With the rest parameter, which can create functions that take a variable number of arguments. These arguments are stored in an array that can be accessed later from inside the function.
    
    ```jsx
    const sum = (...args) => {
      return args.reduce((a, b) => a + b, 0);
    }
    console.log(sum(0,1,2)); // 3
    ```
    
- **Spread Operator**
    
    Spread Operator has ability to copy an array
    
    ```jsx
    const arr1 = ['JAN', 'FEB', 'MAR', 'APR', 'MAY'];
    let arr2;
    arr2 = [...arr1]; 
    console.log(arr2); // [ 'JAN', 'FEB', 'MAR', 'APR', 'MAY' ]
    ```
    
- **Destructuring Assignment**
    
    ```jsx
    const HIGH_TEMPERATURES = {
      yesterday: 75,
      today: 77,
      tomorrow: 80
    };
    
    const {today, tomorrow} = HIGH_TEMPERATURES;
    ```
```jsx
const result = {
  success: ["max-length", "no-amd", "prefer-arrow-functions"],
  failure: ["no-var", "var-on-top", "linebreak"],
  skipped: ["no-extra-semi", "no-dup-keys"]
};
function makeList(arr) {
  // ---------------------
  const failureItems = [];
   for (let i = 0; i < arr.length; i++) {
     failureItems.push(`<li class="text-warning">${arr[i]}</li>`);
   }
   ;
  // -------------

  return failureItems;
}

const failuresList = makeList(result.failure);

console.log(failuresList);

// answer
[ '<li class="text-warning">no-var</li>',
  '<li class="text-warning">var-on-top</li>',
  '<li class="text-warning">linebreak</li>' ]
```

- Object Property Shorthand
    
    ES6 provides the syntactic sugar to eliminate the redundancy of having to write `x: x`. You can simply write `x` once, and it will be converted to`x: x`
    
    ```jsx
    //from this
    const createPerson = (name, age, gender) => {
      return {
        name: name,
        age: age,
        gender: gender
      };
    };
    
    // to this
    const createPerson = (name, age, gender) => ({ name, age, gender});
    ```
    
- Concise Declarative Function in ES6
    
    ```jsx
    // ES5 function method
    const person = {
      name: "Taylor",
      sayHello: function() {
        return `Hello! My name is ${this.name}.`;
      }
    };
    
    //ES6 way
    const person = {
      name: "Taylor",
      sayHello() { // remove 'function'
        return `Hello! My name is ${this.name}.`;
      }
    };
    ```
    
- Class Syntax
    
    `class` keywords are used to create objects in ES6, to utilize this syntax, we need use UpperCamelCase and the `constructor` method (special method for creating and initializing an object created with a class)
    
    ```jsx
    class Vegetable {
      constructor(name) {
        this.name = name;
      }
    }
    const carrot = new Vegetable('carrot');
    console.log(carrot.name); // 'carrot'
    ```
    
- getters & setters
    
    Getter functions are meant to simply return (get) the value of an object's private variable to the user without the user directly accessing the private variable.
    
    Setter functions are meant to modify (set) the value of an object's private variable based on the value passed into the setter function.
    
    ```jsx
    class Thermostat{
      constructor(f) {
        this.f = f;
      }
      // getter
      get temperature() {
        return (5/9)*(this.f -32);
      }
      //setter
      set temperature(c) {
        this.f = (c*9.0)/5 + 32;
      }
    
    }
    const thermos = new Thermostat(76); // Setting in Fahrenheit scale
    let temp = thermos.temperature; // 24.44 in Celsius
    thermos.temperature = 26;
    temp = thermos.temperature; // 26 in Celsius
    ```
    
- Module Script
    
    In order to make JavaScript more modular, clean, and maintainable; ES6 introduced a way to easily share code among JavaScript files. This involves exporting parts of a file for use in one or more other files, and importing the parts you need, where you need them.
    
    ```jsx
    <html>
      <body>
    <script type="module" src="index.js"></script> 
      </body>
    </html>
    ```
    
- Export to share a code block
    
    variables can share from one to multiple Javascript files, by using `export` to the intended variables. When you export a variable or function, you can import it in another file and use it without having to rewrite the code.
    
    ```jsx
    const uppercaseString = (string) => {
      return string.toUpperCase();
    }
    
    const lowercaseString = (string) => {
      return string.toLowerCase()
    }
    
    export { uppercaseString, lowercaseString };
    ```
    
- Reuse JS Code using `import`
    
    `import` allows you to choose which parts of a file or module to load. and we can also import one or more item from the file
    
    ```jsx
    import { uppercaseString, lowercaseString } from './string_functions.js';
    
    uppercaseString("hello");
    lowercaseString("WORLD!");
    ```
    
- using `*` to import everything from the file
    
    ```jsx
    import * as stringFunctions from "./string_functions.js";
    
    stringFunctions.uppercaseString("hello");
    stringFunctions.lowercaseString("WORLD!");
    ```
    
- Export Fallback
    
    *export default*. Usually you will use this syntax if only one value is being exported from a file. It is also used to create a fallback value for a file or module.
    
    you can only have one value be a default export in each module or file. Additionally, you cannot use `export default` with `var`, `let`, or `const`
    
    ```jsx
    export default function subtract(x, y) {
      return x - y;
    }
    ```
    
- Import a Default Export
    
    To import a default export, you need to use a different  `import`   syntax, like this
    
    ```jsx
    import subtract from "./math_functions.js";
    subtract(7,4);
    ```
    
- JavaScript Promise
    
    `Promise` is a constructor function, so you need to use the `new`keyword to create one. It takes a function, as its argument, with two parameters - `resolve` and `reject`. These are methods used to determine the outcome of the promise. The syntax looks like this:
    
    ```jsx
    const myPromise = new Promise((resolve, reject) => {
    
    });
    ```
    
    A promise has three states: `pending`, `fulfilled`, and `rejected`. to actually finish the promise, we need build method to take the argument resolve or reject to fulfilled.
    
    ```jsx
    const myPromise = new Promise((resolve, reject) => {
      if(condition here) {
        resolve("Promise was fulfilled");
      } else {
        reject("Promise was rejected");
      }
    });
    
    // sample
    const makeServerRequest = new Promise((resolve, reject) => {
      // responseFromServer represents a response from a server
      let responseFromServer;
        
      if(responseFromServer) {
        resolve("We got the data");
      } else {  
        reject("Data not received");
      }
    });
    ```
    
    If we’d like to handle `Promise`, This can be achieved by using the `then` method. The `then` method is executed immediately after your promise is fulfilled with `resolve`.
    
    ```jsx
    myPromise.then(result => {
      
    });
    
    // sample
    const makeServerRequest = new Promise((resolve, reject) => {
      // responseFromServer is set to true to represent a successful response from a server
      let responseFromServer = true;
        
      if(responseFromServer) {
        resolve("We got the data");
      } else {  
        reject("Data not received");
      }
    });
    
    makeServerRequest.then(result => {
      console.log(result);
    })
    ```
    
    if the Promise got rejected, we handle them with `catch`
    
    ```jsx
    myPromise.catch(error => {
      
    });
    // sample
    const makeServerRequest = new Promise((resolve, reject) => {
      // responseFromServer is set to false to represent an unsuccessful response from a server
      let responseFromServer = false;
        
      if(responseFromServer) {
        resolve("We got the data");
      } else {  
        reject("Data not received");
      }
    });
    
    makeServerRequest.then(result => {
      console.log(result);
    });
    
    makeServerRequest.catch(error => {
      console.log(error);
      });
    ```
**REGULAR EXPRESSION**
Regular expressions are used in programming languages to match parts of strings. You create patterns to help you do that matching.

Day 13 of #100DaysOfCode

- `.test()` method
    
    takes the regex, applies it to a string (which is placed inside the parentheses), and returns `true` or `false` if your pattern finds something or not.
    
    ```jsx
    let myString = "Hello, World!";
    let myRegex = /Hello/;
    let result = myRegex.test(myString); // true
    ```
    
- Match a Literal String with Different Possibilities
    
    We can search for multiple patterns using the  `alternation`  or  `OR`  operator: `|`.
    
    ```jsx
    let petString = "James has a pet cat.";
    let petRegex = /dog|cat|bird|fish/; 
    let result = petRegex.test(petString);
    ```
    
- Ignore Case while matching
    
    This regex can match the strings `ignorecase`, `igNoreCase`, and `IgnoreCase`.
    
    ```jsx
    let myString = "freeCodeCamp";
    let fccRegex = /freeCodeCamp/i; 
    let result = fccRegex.test(myString);
    ```
    
- Extract Matches `.match()`
    
    Note that the `.match` syntax is the "opposite" of  the  `.test` method
    
    ```jsx
    'string'.match(/regex/);
    /regex/.test('string');
    
    //sample
    let extractStr = "Extract the word 'coding' from this string.";
    let codingRegex = /coding/; 
    let result = extractStr.match(codingRegex);
    ```
    
- `g` flag
    
    `g` flag was used to find more that the first match
    
    ```jsx
    let twinkleStar = "Twinkle, twinkle, little star";
    let starRegex = /Twinkle/gi; 
    let result = twinkleStar.match(starRegex); 
    ```
    
- Wildcard period
    
    The wildcard character `.` will match any one character. The wildcard is also called `dot` and `period`. You can use the wildcard character just like any other character in the regex. For example, if you wanted to match `hug`, `huh`, `hut`, and `hum`, you can use the regex `/hu./` to match all four words.
    
    ```jsx
    let exampleStr = "Let's have fun with regular expressions!";
    let unRegex = /un./; 
    let result = unRegex.test(exampleStr);
    ```
    
- Matching single character with multiple possibilities
    
    You can search for a literal pattern with some flexibility with *character classes*. Character classes allow you to define a group of characters you wish to match by placing them inside square (`[` and `]`) brackets.
    
    ```jsx
    let quoteSample = "Beware of bugs in the above code; I have only proved it correct, not tried it.";
    let vowelRegex = /[aeiou]/gi;
    let result = quoteSample.match(vowelRegex); 
    ```
    
- Match Letters of the Alphabet
    
    Inside a character set, you can define a range of characters to match using a hyphen character: `-`.
    
    For example, to match lowercase letters `a` through `e` you would use `[a-e]`.
    
    ```jsx
    let quoteSample = "The quick brown fox jumps over the lazy dog.";
    let alphabetRegex = /[a-z]/gi; 
    let result = quoteSample.match(alphabetRegex);
    ```
    
- Match Numbers and Letters of the Alphabet
    
    ```jsx
    let quoteSample = "Blueberry 3.141592653s are delicious.";
    let myRegex = /[h-s2-6]/ig; 
    let result = quoteSample.match(myRegex); 
    ```

- Find Character for one or more
    
    ```jsx
    let difficultSpelling = "Mississippi";
    let myRegex = /s+/g; // Change this line
    let result = difficultSpelling.match(myRegex);
    ```
    
- Match Characters that Occur Zero or More Times
    
    ```jsx
    // Only change code below this line
    let chewieRegex = /Aa*/; // Change this line
    // Only change code above this line
    
    let result = chewieQuote.match(chewieRegex);
    ```
    
- Find Characters with Lazy Matching
    
    you can use the `?` character to change it to lazy matching.
    
    ```jsx
    let text = "<h1>Winter is coming</h1>";
    let myRegex = /<.*?>/; // Change this line
    let result = text.match(myRegex);
    ```


- Match Beginning String Patterns
    
    We used the caret character (`^`) inside a character set to create a negated character set in the form `[^thingsThatWillNotBeMatched]`. Outside of a character set, the caret is used to search for patterns at the beginning of strings.
    
    ```jsx
    let rickyAndCal = "Cal and Ricky both like racing.";
    let calRegex = /^Cal/; 
    let result = calRegex.test(rickyAndCal);
    ```
    
- Match Ending String Patterns
    
    We can search the end of strings using the dollar sign character `$` at the end of the regex.
    
    ```jsx
    let caboose = "The last car on a train is the caboose";
    let lastRegex = /caboose$/;
    let result = lastRegex.test(caboose);
    ```


- match all number: `/\d/g`
- match all non numbers : `/\D/g`
- Using shorthand character class (`\w` )to match all letters and number
- Restrict Possible Username
    
    ```jsx
    //case
    //Usernames can only use alpha-numeric characters.
    //The only numbers in the username have to be at the end. There can be zero or more of them at the end. Username cannot start with the number.
    //Username letters can be lowercase and uppercase.
    //Usernames have to be at least two characters long. A two-character username can only use alphabet letters as characters.
    
    //solutions
    let username = "JackOfAllTrades";
    let userCheck = /^[a-z]([0-9]{2,}|[a-z]+\d*)$/i; 
    let result = userCheck.test(username);
    ```
    
- Match whitespace
    
    using `\s` to search the white space, This pattern not only matches whitespace, but also carriage return, tab, form feed, and new line characters.
    
    ```jsx
    let sample = "Whitespace is important in separating words";
    let countWhiteSpace = /\s/g;
    let result = sample.match(countWhiteSpace);
    ```
    

- Match Non-Whitespace Characters
    
    Search for non-whitespace using `\S`, which is an uppercase `s`. This pattern will not match whitespace, carriage return, tab, form feed, and new line characters.
    
    ```jsx
    let sample = "Whitespace is important in separating words";
    let countNonWhiteSpace = /\S/g; 
    let result = sample.match(countNonWhiteSpace);
    ```
    
- Specify Upper and Lower Number of Matches
    
    Recall that you use the plus sign `+` to look for one or more characters and the asterisk `` to look for zero or more characters.
    
    You can specify the lower and upper number of patterns with *quantity specifiers*. Quantity specifiers are used with curly brackets (`{` and `}`).
    
    ```jsx
    let ohStr = "Ohhh no";
    let ohRegex = /Oh{3,6}\sno/;
    let result = ohRegex.test(ohStr);
    ```
    
- Specify Only the Lower Number of Matches
    
    To only specify the lower number of patterns, keep the first number followed by a comma
    
    ```jsx
    let haStr = "Hazzzzah";
    let haRegex = /Haz{4,}ah/; // Change this line
    let result = haRegex.test(haStr);
    ```
    
- Specify Exact Number of Matches
    
    To specify a certain number of patterns, just have that one number between the curly brackets.
    
    ```jsx
    let timStr = "Timmmmber";
    let timRegex = /Tim{4}ber/; 
    let result = timRegex.test(timStr);
    ```
    
- Check for All or None
    
    You can specify the possible existence of an element with a question mark, `?`. This checks for zero or one of the preceding element. You can think of this symbol as saying the previous element is optional.
    
    ```jsx
    let favWord = "favorite";
    let favRegex = /favou?rite/;
    let result = favRegex.test(favWord);
    ```
    
- Positive and Negative Lookahead
    
    *Lookaheads* are patterns that tell JavaScript to look-ahead in your string to check for patterns further along. This can be useful when you want to search for multiple patterns over the same string.
    
    - A positive lookahead is used as `(?=...)` where the `...` is the required part that is not matched.
    - A negative lookahead is used as `(?!...)` where the `...` is the pattern that you do not want to be there.
    
    ```jsx
    let sampleWord = "astronaut";
    let pwRegex = /(?=\w{6,})(?=\w*\d{2})/;
    let result = pwRegex.test(sampleWord);
    ```
    
- Check For Mixed Grouping of Characters
    
    ```jsx
    let myString = "Eleanor Roosevelt";
    let myRegex = /(Eleanor|Franklin).*Roosevelt/;
    let result = myRegex.test(myString); 
    // After passing the challenge experiment with myString and see how the grouping works
    console.log(result); // true, (using .* to allow middle name
    ```
    
- Reuse Patterns Using Capture Groups
    
    ```jsx
    let repeatNum = "42 42 42";
    let reRegex = /^(\d+)\s\1\s\1$/;
    let result = reRegex.test(repeatNum);
    ```
    
- Use Capture Groups to Search and Replace
    
    You can search and replace text in a string using `.replace()` on a string. The inputs for `.replace()` is first the regex pattern you want to search for. The second parameter is the string to replace the match or a function to do something.
    
    ```jsx
    let str = "one two three";
    let fixRegex = /(\w+)\s(\w+)\s(\w+)/; 
    let replaceText = "$3 $2 $1"; 
    let result = str.replace(fixRegex, replaceText);
    ```
    
- Remove Whitespace from Start and End
    
    ```jsx
    let hello = "   Hello, World!  ";
    let wsRegex = /^\s+|\s+$/g; 
    let result = hello.replace(wsRegex, ""); 
    console.log(result);
    ```
    
**Debugging**

- **Use the JavaScript Console to Check the Value of a Variable**
    
    The `console.log()` method, which "prints" the output of what's within its parentheses to the console, will likely be the most helpful debugging tool.
    
- **Understanding the Differences between the freeCodeCamp and Browser Console**
    
    There are many methods to use with `console` to output messages. `log`, `warn`, and `clear` to name a few. The freeCodeCamp console will only output `log` messages, while the browser console will output all messages.
    
- **Use typeof to Check the Type of a Variable**
    
    use `typeof` to check the data structure, or type, of a variable.
    
    JavaScript recognizes six primitive (immutable) data types: `Boolean`, `Null`, `Undefined`, `Number`, `String`, and `Symbol` (new with ES6) and one type for mutable items: `Object`.
    
    ```jsx
    let seven = 7;
    let three = "3";
    console.log(seven + three); // 73
    console.log(typeof seven); // number
    console.log(typeof three); // string
    ```
    
- **Catch Misspelled Variable and Function Names**
- **Catch Unclosed Parentheses, Brackets, Braces and Quotes**
    
    One way to avoid this mistake is as soon as the opening character is typed, immediately include the closing match, then move the cursor back between them and continue coding.
    
- **Catch Use of Assignment Operator Instead of Equality Operator**
- **Catch Mixed Usage of Single and Double Quotes**
- **Catch Missing Open and Closing Parenthesis After a Function Call:** When a function or method doesn't take any arguments, you may forget to include the (empty) opening and closing parentheses when calling it.
    
    ```jsx
    function getNine() {
      let x = 6;
      let y = 3;
      return x + y;
    }
    
    let result = getNine();
    console.log(result);
    ```
    
- **Catch Arguments Passed in the Wrong Order When Calling a Function**
    
    ```jsx
    function raiseToPower(b, e) {
      return Math.pow(base, exp);
    }
    
    let base = 2;
    let exp = 3;
    let power = raiseToPower(base, exp);
    console.log(power);
    ```
    
- **Catch Off By One Errors When Using Indexing**
    
    *Off by one errors* (sometimes called OBOE) crop up when you're trying to target a specific index of a string or array (to slice or access a segment), or when looping over the indices of them. JavaScript indexing starts at zero, not one, which means the last index is always one less than the length of the item.
    
    ```jsx
    function countToFive() {
      let firstFive = "12345";
      let len = firstFive.length;
      // Only change code below this line
      for (let i = 0; i < len; i++) {
      // Only change code above this line
        console.log(firstFive[i]);
      }
    }
    
    countToFive(); // 1 2 3 4 5 
    ```
    
- **Use Caution When Reinitializing Variables Inside a Loop**
- **Prevent Infinite Loops with a Valid Terminal Condition**

**Basic Data Structures**
- **Use an Array to Store a Collection of Data**
    
    a *one-dimensional array*, meaning it only has one level, or that it does not have any other arrays nested within it. Notice it contains *booleans*, *strings*, and *numbers*, among other valid JavaScript data types.
    
    a *multi-dimensional array*, or an array that contains other arrays. Notice that this array also contains JavaScript *objects*
    
    ```jsx
    let yourArray = ['one', 2, 'three', true, false, undefined, null];Access an Array's Contents Using Bracket Notation
    ```
    
- **Access an Array's Contents Using Bracket Notation**
    
    In an array, each array item has an *index*. This index doubles as the position of that item in the array. JavaScript arrays are *zero-indexed*, meaning that the first element of an array is actually at the ***zeroth*** position, not the first.
    
    ```jsx
    let myArray = ["a", "b", "c", "d"];
    myArray[1] = "x"
    console.log(myArray); // ["a", "x", "c", "d"]
    ```
    
- **Add Items to an Array with push() and unshift()**
    
    Both methods take one or more elements as parameters and add those elements to the array the method is being called on; the `push()`method adds elements to the end of an array, and `unshift()` adds elements to the beginning.


- **Remove Items from an Array with pop() and shift()**
    
    , `pop()` *removes* an element from the end of an array, while `shift()` removes an element from the beginning.
    
    ```jsx
    function popShift(arr) {
      let popped = arr.pop();  
      let shifted = arr.shift(); 
      return [shifted, popped];
    }
    
    console.log(popShift(['challenge', 'is', 'not', 'complete'])); // [ 'challenge', 'complete' ]
    ```
    
- **Remove Items Using splice()**
    
    `splice()` allows us to do just that: **remove any number of consecutive elements** from anywhere in an array.
    
    ```jsx
    const arr = [2, 4, 5, 1, 7, 5, 2, 1];
    arr.splice(0,1);
    arr.splice(3,);
    console.log(arr); // [ 4, 5, 1]
    ```
    
- **Add Items Using splice()**
    
    `splice()` can take up to three parameters, by use the third parameter, comprised of one or more element(s), to add to the array. This can be incredibly useful for quickly switching out an element, or a set of elements, for another.
    
    ```jsx
    function htmlColorNames(arr) {
      arr.splice(0,2,'DarkSalmon','BlanchedAlmond');
      return arr;
    }
    
    console.log(htmlColorNames(['DarkGoldenRod', 'WhiteSmoke', 'LavenderBlush', 'PaleTurquoise', 'FireBrick']));
    /* [ 'DarkSalmon',
      'BlanchedAlmond',
      'LavenderBlush',
      'PaleTurquoise',
      'FireBrick' ] /*
    ```
    
- **Copy Array Items Using slice()**
    
    ```jsx
    function forecast(arr) {
      return arr.slice(2,4); // ['warm', 'sunny',]
    }
    console.log(forecast(['cold', 'rainy', 'warm', 'sunny', 'cool', 'thunderstorms']));
    ```
    
- **Copy an Array with the Spread Operator**
    
    new *spread operator* allows us to easily copy *all* of an array's elements, in order, with a simple and highly readable syntax. The spread syntax simply looks like this: `...`
    
    ```jsx
    function copyMachine(arr, num) {
      let newArr = [];
      while (num >= 1) {
        newArr.push([...arr]);
        num--;
      }
      return newArr;
    }
    
    console.log(copyMachine([true, false, true], 2));
    ```
    
- **Combine Arrays with the Spread Operator**
    
    to insert all the elements of one array into another, at any index.
    
    ```jsx
    function spreadOut() {
      let fragment = ['to', 'code'];
      let sentence = ['learning', ...fragment, 'is', 'fun'];
      return sentence;
    }
    
    console.log(spreadOut()); // [ 'learning', 'to', 'code', 'is', 'fun' ]
    ```
    
- **Check For The Presence of an Element With indexOf()**
    
    `indexOf()`takes an element as a parameter, and when called, it returns the position, or index, of that element, or `1` if the element does not exist on the array.
    
    ```jsx
    function quickCheck(arr, elem) {
      return arr.indexOf(elem) >= 0 ? true: false;
    }
    
    console.log(quickCheck(['squash', 'onions', 'shallots'], 'mushrooms'));
    // 
    ```
    
- **Iterate Through All an Array's Items Using For Loops**
    
    the technique which is most flexible and offers us the greatest amount of control is a simple `for` loop.
    the technique which is most flexible and offers us the greatest amount of control is a simple `for` loop.

```jsx
function filteredArray(arr, elem) {
  let newArr = [];

  for (let i = 0; i < arr.length; i++) {
    if(arr[i].indexOf(elem) == -1)
    // check every parameter of the element, if its not there, continue the code
     {
      newArr.push(arr[i]);
      // insert element of an array to new filtered array
    }
  }
  return newArr;
}

console.log(filteredArray([[3, 2, 3], [1, 6, 3], [3, 13, 26], [19, 3, 9]], 3));
```

Day 19 of #100DaysOfCode

- **Create complex multi-dimensional arrays**
    
    arrays can contain an infinite depth of arrays that can contain other arrays, each with their own arbitrary levels of depth, and so on.
    
    ```jsx
    let myNestedArray = [
      ['unshift', false, 1, 2, 3, 'complex', 'nested'],
      ['loop', 'shift', 6, 7, 1000, 'method'],
      ['concat', false, true, 'spread', 'array',['deep']],
      ['mutate', 1327.98, 'splice', 'slice', 'push',[['deeper']]],
      ['iterate', 1.3849, 7, '8.4876', 'arbitrary', 'depth',[[['deepest']]]
    ];
    ```
    
- **Add Key-Value Pairs to JavaScript Objects**
    
    Key-value pairs are pieces of data (*values*) mapped to unique identifiers called *properties* (*keys*).
    
    ```jsx
    let foods = {
      apples: 25,
      oranges: 32,
      plums: 28
    };
    
    foods.bananas = 13;
    foods.grapes = 35;
    foods.strawberries = 27;
    
    console.log(foods);
    /*
      apples: 25,
      oranges: 32,
      plums: 28
      bananas: 13,
      grapes: 35,
      strawberries: 27,
     */
    ```
    
- **Modify an Object Nested Within an Object**
    
    Object properties can be nested to an arbitrary depth, and their values can be any type of data supported by JavaScript
    
    ```jsx
    let userActivity = {
      id: 23894201352,
      date: 'January 1, 2017',
      data: {
        totalUsers: 51,
        online: 42
      }
    };
    userActivity.data.online = 45;
    console.log(userActivity);
    /* 
      id: 23894201352,
      date: 'January 1, 2017',
      data: {
        totalUsers: 51,
        online: 45
    */
    ```
    
- **Access Property Names with Bracket Notation**
- **Use the delete Keyword to Remove Object Properties**
    
    ```jsx
    let foods = {
      apples: 25,
      oranges: 32,
      plums: 28,
      bananas: 13,
      grapes: 35,
      strawberries: 27
    };
    
    delete foods.oranges;
    delete foods.plums;
    delete foods.strawberries;
    console.log(foods); // { apples: 25, bananas: 13, grapes: 35 }
    ```
    
- **Check if an Object has a Property**
    
    ```jsx
    let users = {
      Alan: {
        age: 27,
        online: true
      },
      Jeff: {
        age: 32,
        online: true
      },
      Sarah: {
        age: 48,
        online: true
      },
      Ryan: {
        age: 19,
        online: true
      }
    };
    
    function isEveryoneHere(userObj) {
      if (userObj.hasOwnProperty('Alan') &&
      userObj.hasOwnProperty('Jeff') &&
      userObj.hasOwnProperty('Sarah') &&
      userObj.hasOwnProperty('Ryan') ) {
        return true;
      }
      return false;
    }
    
    console.log(isEveryoneHere(users));
    ```
    
- **Iterate Through the Keys of an Object with a for...in Statement**
    
    Sometimes you may need to iterate through all the keys within an object. This requires a specific syntax in JavaScript called a *for...in* statement.
    
    ```jsx
    const users = {
      Alan: {
        online: false
      },
      Jeff: {
        online: true
      },
      Sarah: {
        online: false
      }
    }
    
    function countOnline(usersObj) {
      let count = 0;
      for ( let user in usersObj) {
        if (usersObj[user].online === true){
          count++;
        }
      }
      return count;
    }
    
    console.log(countOnline(users));
    ```
    
- **Generate an Array of All Object Keys with Object.keys()**
    
    using the `Object.keys()` method and passing in an object as the argument. This will return an array with strings representing each property in the object.
    
    ```jsx
    let users = {
      Alan: {
        age: 27,
        online: false
      },
      Jeff: {
        age: 32,
        online: true
      },
      Sarah: {
        age: 48,
        online: false
      },
      Ryan: {
        age: 19,
        online: true
      }
    };
    
    function getArrayOfUsers(obj) {
     return Object.keys(obj);
    }
    console.log(getArrayOfUsers(users));
    ```
    
- **Modify an Array Stored in an Object**
    
    ```jsx
    let user = {
      name: 'Kenneth',
      age: 28,
      data: {
        username: 'kennethCodesAllDay',
        joinDate: 'March 26, 2016',
        organization: 'freeCodeCamp',
        friends: [
          'Sam',
          'Kira',
          'Tomo'
        ],
        location: {
          city: 'San Francisco',
          state: 'CA',
          country: 'USA'
        }
      }
    };
    
    function addFriend(userObj, friend) {
      // Only change code below this line
     userObj.data.friends.push(friend);
     return userObj.data.friends;
      // Only change code above this line
    }
    
    console.log(addFriend(user, 'Pete')); // [ 'Sam', 'Kira', 'Tomo', 'Pete' ]
    ```
    
    ```jsx
Day 20-21

```jsx
function convertToF(celsius) {
  let fahrenheit = (9/5)*celsius + 32;
  return fahrenheit;
}

console.log(convertToF(30)); // 86
```

- Reverse a String
    
    ```jsx
    function reverseString(str) {
      var splitStr = str.split("");
      var reverseArr = splitStr.reverse();
      var joinStr = reverseArr.join("");
      return joinStr;
    }
    
    console.log(reverseString("hello")); // "olleh"
    ```
    
- **Factorialize a Number**
    
    ```jsx
    // with recursion
    function factorialize(num) {
    	// if the num is less than 0, reject it.
      if (num <0)
      return -1;
    
    	// if the num is 0, its factorial is 1
      else if (num == 0)
      return 1;
    	// otherwise, call the recursive procedure again
       else {
         return (num * factorialize(num-1));
       }
    }
    
    console.log(factorialize(5)); // 120
    
    // with while loop
    function factorialize(num) {
    	// variable that store num
      let result = num;
    	
    	// if num = 0, or = 1, the factorial will return 1
      if(num === 0 || num === 1)
      return 1;
    
    	// while loop, ehich decrementation by 2 at each iteration
      while (num>1) {
        num--;
        result = result * num;
      }
    	// return the factorial
      return result;
    }
    
    console.log(factorialize(5));
    
    // with for loop
    function factorialize(num) {
    	// if num = 0, or = 1, the factorial will return 1
      if(num === 0 || num === 1)
      return 1;
    
    	// decrement i after each iteration
      for (let i = num - 1; i >= 1; i--) {
    	// this will store the value of num at each iteration
        num = num * i;
      }
    	// return the factorial
      return num;
    }
    
    console.log(factorialize(5));
    ```
    
- **Find the Longest Word in a String**
    
    ```jsx
    // using for loop
    function findLongestWordLength(str) {
    
    	// give split with space .split(' ') for separate each word
      let strSplit = str.split(' ');
      let longestWord = 0;
    
      // for loop
      for ( let i = 0; i < strSplit.length; i++) {
    		// if current word are the longerst than prev, make the current word = longest
        if(strSplit[i].length > longestWord) {
          longestWord = strSplit[i].length
        }
      }
      return longestWord;
    }
    
    console.log(findLongestWordLength("The quick brown fox jumped over the lazy dog")); // 6
    ```
    
- **Return Largest Numbers in Arrays**
    
    ```jsx
    // using for loop
    function largestOfFour(arr) {
      let results = [];
      for (let i = 0; i < arr.length; i++) {
        let largestNumber = arr[i][0];
        for (let j = 1; j < arr[i].length; j++) {
          if (arr[i][j] > largestNumber) {
            largestNumber = arr[i][j];
          }
        }
        results[i] = largestNumber;
      }
      return results;
    }
    console.log(largestOfFour([[4, 5, 1, 3], [13, 27, 18, 26], [32, 35, 37, 39], [1000, 1001, 857, 1]]));
    // [ 5, 27, 39, 1001 ]
    ```
    
- **Confirm the Ending**
    
    ```jsx
    function confirmEnding(str, target) {
      return (str.substr(-target.length) === target) ? true : false;
    }
    
    console.log(confirmEnding("Bastian", "n")); // true
    ```
    
- **Repeat a String Repeat a String**
    
    ```jsx
    // using while loop
    function repeatStringNumTimes(str, num) {
       let rptStr = "";
       while (num > 0) {
         rptStr += str;
         num--;
       }
       return rptStr;
    }
    
    console.log(repeatStringNumTimes("abc", 3)); // abcabcabc
    ```
    
- **Truncate a String**
    
    ```jsx
    function truncateString(str, num) {
      return str.length > num ? str.slice(0, num) + "...": str ;
    }
    
    console.log(truncateString("A-tisket a-tasket A green and yellow basket", 8)); // A-tisket...
    ```
- **Finders Keepers**
    
    ```jsx
    function findElement(arr, func) {
      let num = 0;
      for (let i=0; i < arr.length; i++) {
        num = arr[i];
    		// the num variable is being passed into the function,
    		// set into each index in array
        if(func(num)){
          return num;
        }
      }
      return undefined;
    }
    
    console.log(findElement([1, 2, 3, 4], num => num % 2 === 0)); // 2
    ```
    
- **Boo who**
    
    Checking if any value is classified as boolean primitive.
    
    ```jsx
    function booWho(bool) {
      return typeof bool === 'boolean';
    }
    
    console.log(booWho(null)); // false
    ```
    
- **Title Case a Sentence**
    
    ```jsx
    function titleCase(str) {
      return str.replace(
        /\w\S*/g,
        function(txt){
          return txt.charAt(0).toUpperCase() + txt.substr(1).toLowerCase();
        }
      );
    }
    
    console.log(titleCase("I'm a little tea pot")); //I'm A Little Tea Pot
    ```
    
- **Slice and Splice**
    
    ```jsx
    function frankenSplice(arr1, arr2, n) {
      
      // create a copy of arr2, using slice() = extracts a section of a string and returns it as a new string
      let combineArr = arr2.slice(); // [4,5,6]
    
      // use spread opt on arr1 for copy each element on arr1
      // splice() hanges the contents of an array by removing
    	// or replacing existing elements and/or adding new elements.
      combineArr.splice(n, 0, ...arr1);
      
      return combineArr;
    }
    
    console.log(frankenSplice([1, 2, 3], [4, 5, 6], 1)); // [ 4, 1, 2, 3, 5, 6 ]
    ```
    
- **Falsy Bouncer**
    
    Falsy values in JavaScript are `false`, `null`, `0`, `""`, `undefined`, and `NaN`.
    
    ```jsx
    function bouncer(arr) {
      let newArray = [];
      for (let i = 0; i < arr.length; i++) {
        if (arr[i]) newArray.push(arr[i]);
      }
      return newArray;
    }
    
    console.log(bouncer([7, "ate", "", false, 9])); // [ 7, 'ate', 9 ]
    ```
- **Where do I Belong**
    
    ```jsx
    function getIndexToIns(arr, num) {
      arr.sort((a,b) => a-b)
    
      for (let i = 0; i < arr.length; i++) {
        if (arr[i] >= num) {
          return i;
        }
      }
      
      return arr.length;
    }
    
    console.log(getIndexToIns([40, 60], 50)); // 1
    ```
    
- Mutation
    
    Using `for loop`, and `indexOf`
    
    ```jsx
    function mutation(arr) {
    let test = arr[1].toLowerCase();
    let target = arr[0].toLowerCase();
    
    for (let i = 0; i < test.length; i++) {
    if (target.indexOf(test[i]) < 0) return false;
    }
    
    return true;
    } 
    console.log(mutation(["hello", "hey"])); // false
    ```
    
- **Chunky Monkey**
    
    Write a function that splits an array (first argument) into groups the length of `size` (second argument) and returns them as a two-dimensional array.
    
    ```jsx
    function chunkArrayInGroups(arr, size) {
    // create mty array to store data
    let newArr = [];
    // using for loop, start with 0, and increment by size value,
    
    for (let i = 0; i < arr.length; i += size) {
    	newArr.push(arr.slice(i, i + size));
    }
    	return newArr;
    }
    
    console.log(chunkArrayInGroups(["a", "b", "c", "d"], 2));
    // [ [ 'a', 'b' ], [ 'c', 'd' ] ]
    ```
  
  - **Use Dot Notation to Access the Properties of an Object**
    
    ```jsx
    let dog = {
      name: "Spot",
      numLegs: 4
    };
    console.log(dog.name); // Spot
    console.log(dog.numLegs); // 4
    ```
    
- **Create a Method on an Object**
    
    Methods are properties that are functions. This adds different behavior to an object.
    
    ```jsx
    let dog = {
      name: "Spot",
      numLegs: 4,
      sayLegs: function() {
        return "This dog has "+ dog.numLegs +  " legs.";
      }
    
    };
    
    console.log(dog.sayLegs()); // This dog has 4 legs.
    ```
    
- **Make Code More Reusable with the this Keyword**
    
    `this` keyword: refers to the object that the method is associated with.
    
    ```jsx
    let dog = {
      name: "Spot",
      numLegs: 4,
      sayLegs: function() {return "This dog has " + this.numLegs + " legs.";}
    };
    
    dog.sayLegs();
    ```
    
- **Define a Constructor Function**
    
    *Constructors* are functions that create new objects. They define properties and behaviors that will belong to the new object.
    
    ```jsx
    function Dog() {
      this.name = "Puppy";
      this.color = "black";
      this.numLegs = 4;
    }
    ```
    
- **Use a Constructor to Create Objects**
    
    ```jsx
    function Dog() {
      this.name = "Rupert";
      this.color = "brown";
      this.numLegs = 4;
    }
    let hound = new Dog();
    ```

- **Extend Constructors to Receive Argument**

```jsx
function Dog(name, color) {
this.name = name;
this.color = color;
this.numLegs = 4;
}

let terrier = new Dog("George", "White");

console.log(terrier); 
```

- **Verify an Object's Constructor with instanceoF**
    
    ```jsx
    // instanceof allows to compate an object to a constructor, return true or false
    function House(numBedrooms) {
      this.numBedrooms = numBedrooms;
    }
    
    let myHouse = new House(7);
    myHouse instanceof House;
    ```
    
- **Understand Own Properties**
    
    ```jsx
    function Bird(name) {
      this.name = name;
      this.numLegs = 2;
    }
    
    let canary = new Bird("Tweety");
    let ownProps = [];
    
    for (let property in canary){
      if(canary.hasOwnProperty(property)){
        ownProps.push(property);
      }
    }
    
    console.log(ownProps); // [name, numLegs]
    ```
    
- **Use Prototype Properties to Reduce Duplicate Code**
    
    Nearly every object in JavaScript has a `prototype` property which is part of the constructor function that created it.
    
    ```jsx
    function Dog(name) {
      this.name = name;
    }
    
    Dog.prototype.numLegs = 2;
    let beagle = new Dog("Snoopy");
    
    // Now all instances of Dog have the numLegs property.
    ```
    
- **Iterate Over All Properties**
    
    Own properties are defined directly on the object instance itself. And prototype properties are defined on the `prototype`.
    
    ```jsx
    function Dog(name) {
      this.name = name;
    }
    
    Dog.prototype.numLegs = 4;
    
    let beagle = new Dog("Snoopy");
    
    let ownProps = [];
    let prototypeProps = [];
    
    // Only change code below this line
    for (let property in beagle){
       if(Dog.hasOwnProperty(property)) {
        ownProps.push(property);
      } else {
        prototypeProps.push(property);
      }
    }
    
    console.log(ownProps); // [ 'name']
    console.log(prototypeProps); // [ 'numLegs' ]
    ```
    
- **Understand the Constructor Property**
    
    ```jsx
    function Dog(name) {
      this.name = name;
    }
    
    function joinDogFraternity(candidate) {
      if(candidate.constructor === Dog) {
        return true;
      } else {
        return false;
      }
    }
    ```
    
- **Change the Prototype to a New Object**
    
    ```jsx
    function Dog(name) {
      this.name = name;
    }
    
    Dog.prototype = {
      numLegs: 4,
      eat: function() {
        console.log("nyam nyam");
      },
      describe: function() {
        console.log("My Dog is" + this.name)
      }
    };
    ```
- **Remember to Set the Constructor Property when Changing the Prototype**
    
    Manually set the prototype to a new object could remove the `constructor` property.
    
    ```jsx
    function Dog(name) {
      this.name = name;
    }
    
    Dog.prototype = {
    
      constructor: Dog, // solution
      numLegs: 4,
      eat: function() {
        console.log("nom nom nom");
      },
      describe: function() {
        console.log("My name is " + this.name);
      }
    };
    ```
    
- **Understand Where an Object’s Prototype Comes From**
    
    ```jsx
    function Dog(name) {
      this.name = name;
    }
    
    let beagle = new Dog("Snoopy");
    
    console.log(Dog.prototype.isPrototypeOf(beagle)); // true
    ```
    
- **Understand the Prototype Chain**
    
    All objects in JavaScript (with a few exceptions) have a `prototype`. Also, an object’s `prototype` itself is an object.
    
    ```jsx
    function Dog(name) {
      this.name = name;
    }
    
    let beagle = new Dog("Snoopy");
    
    Dog.prototype.isPrototypeOf(beagle);  // yields true
    
    Object.prototype.isPrototypeOf(Dog.prototype);
    ```
    
- **Use Inheritance So You Don't Repeat Yourself**
    
    ```jsx
    function Cat(name) {
      this.name = name;
    }
    
    Cat.prototype = {
      constructor: Cat,
    };
    
    function Bear(name) {
      this.name = name;
    }
    
    Bear.prototype = {
      constructor: Bear,
    };
    
    function Animal() { }
    
    Animal.prototype = {
      constructor: Animal,
      eat: function() {
        console.log("nom nom nom");
      }
    
    };
    
    // Remove the “eat” method from Cat.prototype and Bear.prototype and add it to the Animal.prototype.
    ```
    
- **Inherit Behaviors from a Supertype**
    
    ```jsx
    function Animal() { }
    
    Animal.prototype = {
      constructor: Animal,
      eat: function() {
        console.log("nom nom nom");
      }
    };
    
    let animal = new Animal();
    
    let duck = Object.create(Animal.prototype); 
    let beagle = Object.create(Animal.prototype); 
    
    // Object.create(obj) creates a new object, and
    // sets obj as the new object's prototype. 
    // Recall that the prototype is like the "recipe" 
    // for creating an object. By setting the prototype of
    // animal to be the prototype of Animal, 
    // you are effectively giving the animal instance 
    // the same "recipe" as any other instance of Animal.
    ```
    
- **Set the Child's Prototype to an Instance of the Parent**
    
    ```jsx
    function Animal() { }
    
    Animal.prototype = {
      constructor: Animal,
      eat: function() {
        console.log("nom nom nom");
      }
    };
    
    function Dog() { }
    
    // Only change code below this line
    Dog.prototype = Object.create(Animal.prototype);
    
    let beagle = new Dog();
    beagle.eat(); // nom nom nom
    ```
- **Reset an Inherited Constructor Property**
    
    ```jsx
    function Animal() { }
    function Bird() { }
    function Dog() { }
    
    Bird.prototype = Object.create(Animal.prototype);
    Dog.prototype = Object.create(Animal.prototype);
    
    // answers
    Bird.prototype.constructor = Bird;
    Dog.prototype.constructor = Dog;
    
    let duck = new Bird();
    let beagle = new Dog();
    ```
    
- **Add Methods After Inheritance**
    
    A constructor function that inherits its `prototype` object from a supertype constructor function can still have its own methods in addition to inherited methods.
    
    ```jsx
    function Animal() { }
    Animal.prototype.eat = function() { console.log("nom nom nom"); };
    
    function Dog() { }
    
    Dog.prototype = Object.create(Animal.prototype);
    Dog.prototype.constructor = Dog;
    
    Dog.prototype.bark = function() {
      console.log("Woof!");
    };
    
    let beagle = new Dog();
  
  ```
  
- **Override Inherited Methods**
    
    ```jsx
    function Bird() { }
    
    Bird.prototype.fly = function() { return "I am flying!"; };
    
    function Penguin() { }
    Penguin.prototype = Object.create(Bird.prototype);
    Penguin.prototype.constructor = Penguin;
    
    Penguin.prototype.fly = function() {
      return "Alas, this is a flightless bird.";
    };
    
    let penguin = new Penguin();
    console.log(penguin.fly());
    ```
    
- **Use a Mixin to Add Common Behavior Between Unrelated Objects**
    
    A mixin allows other objects to use a collection of functions.
    
    ```jsx
    let bird = {
      name: "Donald",
      numLegs: 2
    };
    
    let boat = {
      name: "Warrior",
      type: "race-boat"
    };
    
    let glideMixin = function(obj) {
      obj.glide = function() {
        console.log("Flying, wooosh!");
      }
    };
    
    glideMixin(bird);
    glideMixin(boat);
    
    bird.glide(); // Flying, wooosh!
    boat.glide(); // Flying, wooosh!
    ```
    
 - **Use Closure to Protect Properties Within an Object from Being Modified Externally**
    
    ```jsx
    function Bird() {
      let weight = 15;
      this.getWeight = () => weight;  // 15
    }
    ```
  
- **Understand the Immediately Invoked Function Expression (IIFE)**
    
    The two parentheses () at the end of the function expression cause it to be immediately executed or invoked. This pattern is known as an *immediately invoked function expression* or *IIFE*.
    
    ```jsx
    (function () {
      console.log("A cozy nest is ready");
    })();
    ```
    
- **Use an IIFE to Create a Module**
    
    ```jsx
    let funModule = (function(){
      return {
        isCuteMixin : function(obj) {
      obj.isCute = function() {
        return true;
      };
        },
        singMixin: function(obj) {
      obj.sing = function() {
        console.log("Singing to an awesome tune");
      };
        }
      }
    })();
    ```
    
- **Learn About Functional Programming**
    
    Functional programming is a style of programming where solutions are simple, isolated functions, without any side effects outside of the function scope
    
    - Isolated function
    - Pure functions
    - Limited Side Effects
    
    ```jsx
    // Function that returns a string representing a cup of green tea
    const prepareTea = () => 'greenTea';
    
    /*
    Given a function (representing the tea type) and number of cups needed, the
    following function returns an array of strings (each representing a cup of
    a specific type of tea).
    */
    const getTea = (numOfCups) => {
      const teaCups = [];
    
      for(let cups = 1; cups <= numOfCups; cups += 1) {
        const teaCup = prepareTea();
        teaCups.push(teaCup);
      }
      return teaCups;
    };
    
    // call getTea for 40 cups and store in tea4TeamFCC
    const tea4TeamFCC = getTea(40);
    ```
    
- **Understand Functional Programming Terminology**
    
    ```jsx
    // Function that returns a string representing a cup of green tea
    const prepareGreenTea = () => 'greenTea';
    
    // Function that returns a string representing a cup of black tea
    const prepareBlackTea = () => 'blackTea';
    
    /*
    Given a function (representing the tea type) and number of cups needed, the
    following function returns an array of strings (each representing a cup of
    a specific type of tea).
    */
    const getTea = (prepareTea, numOfCups) => {
      const teaCups = [];
    
      for(let cups = 1; cups <= numOfCups; cups += 1) {
        const teaCup = prepareTea();
        teaCups.push(teaCup);
      }
      return teaCups;
    };
    
    // 27 green tea, 13 black tea
    const tea4GreenTeamFCC = getTea(prepareGreenTea, 27);
    const tea4BlackTeamFCC = getTea(prepareBlackTea, 13);
    
    console.log(
      tea4GreenTeamFCC,
      tea4BlackTeamFCC
    );
    ```
    
- **Understand the Hazards of Using Imperative Code**
    
    ```jsx
    // tabs is an array of titles of each site open within the window
    const Window = function(tabs) {
      this.tabs = tabs; // We keep a record of the array inside the object
    };
    
    // When you join two windows into one window
    Window.prototype.join = function(otherWindow) {
      this.tabs = this.tabs.concat(otherWindow.tabs);
      return this;
    };
    
    // When you open a new tab at the end
    Window.prototype.tabOpen = function(tab) {
      this.tabs.push('new tab'); // Let's open a new tab for now
      return this;
    };
    
    // When you close a tab
    Window.prototype.tabClose = function(index) {
    
      // change the splice into slice()
    
      const tabsBeforeIndex = this.tabs.slice(0, index); // Get the tabs before the tab
      const tabsAfterIndex = this.tabs.slice(index + 1); // Get the tabs after the tab
    
      this.tabs = tabsBeforeIndex.concat(tabsAfterIndex); // Join them together
    
      return this;
     };
    
    // Let's create three browser windows
    const workWindow = new Window(['GMail', 'Inbox', 'Work mail', 'Docs', 'freeCodeCamp']); // Your mailbox, drive, and other work sites
    const socialWindow = new Window(['FB', 'Gitter', 'Reddit', 'Twitter', 'Medium']); // Social sites
    const videoWindow = new Window(['Netflix', 'YouTube', 'Vimeo', 'Vine']); // Entertainment sites
    
    // Now perform the tab opening, closing, and other operations
    const finalTabs = socialWindow
      .tabOpen() // Open a new tab for cat memes
      .join(videoWindow.tabClose(2)) // Close third tab in video window, and join
      .join(workWindow.tabClose(1).tabOpen());
    console.log(finalTabs.tabs);
    ```
- **Avoid Mutations and Side Effects Using Functional Programming**
    
    One of the core principles of functional programming is to not change things. Changes lead to bugs. It's easier to prevent bugs knowing that your functions don't change anything, including the function arguments or any global variable.
    
    Recall that in functional programming, changing or altering things is called *mutation*, and the outcome is called a *side effect*. A function, ideally, should be a *pure function*, meaning that it does not cause any side effects.
    
    ```jsx
    // The global variable
    let fixedValue = 4;
    
    function incrementer() {
      return fixedValue + 1;
    }
    
    var newValue = incrementer(); // 5
    console.log(fixedValue); //  4
    ```
    
- **Pass Arguments to Avoid External Dependence in a Function**
    
    Another principle of functional programming is to always declare your dependencies explicitly. This means if a function depends on a variable or object being present, then pass that variable or object directly into the function as an argument.
    
    ```jsx
    // The global variable
    let fixedValue = 4;
    
    function incrementer(a) {
    var newValue = a + 1
    return newValue;
    
    }
    
    console.log(incrementer(fixedValue)); // 5
    ```

- **Refactor Global Variables Out of Functions**
Principles for functional programming:

1. Don't alter a variable or object - create new variables and objects and return them if need be from a function. Hint: using something like `const newArr = arrVar`, where `arrVar` is an array will simply create a reference to the existing variable and not a copy. So changing a value in `newArr` would change the value in `arrVar`.
2. Declare function parameters - any computation inside a function depends only on the arguments passed to the function, and not on any global object or variable.

```jsx
// The global variable
const bookList = ["The Hound of the Baskervilles", "On The Electrodynamics of Moving Bodies", "Philosophiæ Naturalis Principia Mathematica", "Disquisitiones Arithmeticae"];

function add(arr, bookName) {
  let bookList = [...arr]; // copy list of an array

  bookList.push(bookName); //Add bookName parameter to the end of the new bookList
  return bookList; // return the new array
  
}

function remove(arr, bookName) {
  let bookList = [...arr];
  if (bookList.indexOf(bookName) >= 0) {
		// check whether the bookName parameter is in the new array
    bookList.splice(bookList.indexOf(bookName), 1); // remove the given parameter from new array
    return bookList; // return new array
  }
    
}
```

Day 34 - 35 of #100DaysOfCode

- **Use the map Method to Extract Data from an Array**
    
    Functions are considered as first class object in JavaScript, which mean they can used like any other objects, where can be saved in variables, stored in an object, or passed as function arguments.
    
    The `map`method iterates over each item in an array and returns a new array containing the results of calling the callback function on each element. It does this without mutating the original array.
    
    ```jsx
    // sample code
    // The global variable
    const watchList = [
      {
        "Title": "Inception",
        "Year": "2010",
        "Rated": "PG-13",
        "Released": "16 Jul 2010",
        "Runtime": "148 min",
        "Genre": "Action, Adventure, Crime",
        "Director": "Christopher Nolan",
        "Writer": "Christopher Nolan",
        "Actors": "Leonardo DiCaprio, Joseph Gordon-Levitt, Elliot Page, Tom Hardy",
        "Plot": "A thief, who steals corporate secrets through use of dream-sharing technology, is given the inverse task of planting an idea into the mind of a CEO.",
        "Language": "English, Japanese, French",
        "Country": "USA, UK",
        "Awards": "Won 4 Oscars. Another 143 wins & 198 nominations.",
        "Poster": "http://ia.media-imdb.com/images/M/MV5BMjAxMzY3NjcxNF5BMl5BanBnXkFtZTcwNTI5OTM0Mw@@._V1_SX300.jpg",
        "Metascore": "74",
        "imdbRating": "8.8",
        "imdbVotes": "1,446,708",
        "imdbID": "tt1375666",
        "Type": "movie",
        "Response": "True"
      },
      {
        "Title": "Interstellar",
        "Year": "2014",
        "Rated": "PG-13",
        "Released": "07 Nov 2014",
        "Runtime": "169 min",
        "Genre": "Adventure, Drama, Sci-Fi",
        "Director": "Christopher Nolan",
        "Writer": "Jonathan Nolan, Christopher Nolan",
        "Actors": "Ellen Burstyn, Matthew McConaughey, Mackenzie Foy, John Lithgow",
        "Plot": "A team of explorers travel through a wormhole in space in an attempt to ensure humanity's survival.",
        "Language": "English",
        "Country": "USA, UK",
        "Awards": "Won 1 Oscar. Another 39 wins & 132 nominations.",
        "Poster": "http://ia.media-imdb.com/images/M/MV5BMjIxNTU4MzY4MF5BMl5BanBnXkFtZTgwMzM4ODI3MjE@._V1_SX300.jpg",
        "Metascore": "74",
        "imdbRating": "8.6",
        "imdbVotes": "910,366",
        "imdbID": "tt0816692",
        "Type": "movie",
        "Response": "True"
      },
      {
        "Title": "The Dark Knight",
        "Year": "2008",
        "Rated": "PG-13",
        "Released": "18 Jul 2008",
        "Runtime": "152 min",
        "Genre": "Action, Adventure, Crime",
        "Director": "Christopher Nolan",
        "Writer": "Jonathan Nolan (screenplay), Christopher Nolan (screenplay), Christopher Nolan (story), David S. Goyer (story), Bob Kane (characters)",
        "Actors": "Christian Bale, Heath Ledger, Aaron Eckhart, Michael Caine",
        "Plot": "When the menace known as the Joker wreaks havoc and chaos on the people of Gotham, the caped crusader must come to terms with one of the greatest psychological tests of his ability to fight injustice.",
        "Language": "English, Mandarin",
        "Country": "USA, UK",
        "Awards": "Won 2 Oscars. Another 146 wins & 142 nominations.",
        "Poster": "http://ia.media-imdb.com/images/M/MV5BMTMxNTMwODM0NF5BMl5BanBnXkFtZTcwODAyMTk2Mw@@._V1_SX300.jpg",
        "Metascore": "82",
        "imdbRating": "9.0",
        "imdbVotes": "1,652,832",
        "imdbID": "tt0468569",
        "Type": "movie",
        "Response": "True"
      },
      {
        "Title": "Batman Begins",
        "Year": "2005",
        "Rated": "PG-13",
        "Released": "15 Jun 2005",
        "Runtime": "140 min",
        "Genre": "Action, Adventure",
        "Director": "Christopher Nolan",
        "Writer": "Bob Kane (characters), David S. Goyer (story), Christopher Nolan (screenplay), David S. Goyer (screenplay)",
        "Actors": "Christian Bale, Michael Caine, Liam Neeson, Katie Holmes",
        "Plot": "After training with his mentor, Batman begins his fight to free crime-ridden Gotham City from the corruption that Scarecrow and the League of Shadows have cast upon it.",
        "Language": "English, Urdu, Mandarin",
        "Country": "USA, UK",
        "Awards": "Nominated for 1 Oscar. Another 15 wins & 66 nominations.",
        "Poster": "http://ia.media-imdb.com/images/M/MV5BNTM3OTc0MzM2OV5BMl5BanBnXkFtZTYwNzUwMTI3._V1_SX300.jpg",
        "Metascore": "70",
        "imdbRating": "8.3",
        "imdbVotes": "972,584",
        "imdbID": "tt0372784",
        "Type": "movie",
        "Response": "True"
      },
      {
        "Title": "Avatar",
        "Year": "2009",
        "Rated": "PG-13",
        "Released": "18 Dec 2009",
        "Runtime": "162 min",
        "Genre": "Action, Adventure, Fantasy",
        "Director": "James Cameron",
        "Writer": "James Cameron",
        "Actors": "Sam Worthington, Zoe Saldana, Sigourney Weaver, Stephen Lang",
        "Plot": "A paraplegic marine dispatched to the moon Pandora on a unique mission becomes torn between following his orders and protecting the world he feels is his home.",
        "Language": "English, Spanish",
        "Country": "USA, UK",
        "Awards": "Won 3 Oscars. Another 80 wins & 121 nominations.",
        "Poster": "http://ia.media-imdb.com/images/M/MV5BMTYwOTEwNjAzMl5BMl5BanBnXkFtZTcwODc5MTUwMw@@._V1_SX300.jpg",
        "Metascore": "83",
        "imdbRating": "7.9",
        "imdbVotes": "876,575",
        "imdbID": "tt0499549",
        "Type": "movie",
        "Response": "True"
      }
    ];
    
    // each item in array is processed to extract title and rating
    
    const ratings = watchList.map(item => ({
      title: item["Title"],
      rating: item["imdbRating"],
    }));
    
    console.log(JSON.stringify(ratings));
    ```
    
- **Implement map on a Prototype**
    
    `map` is a pure function, and its output depends solely on its inputs. Plus, it takes another function as its argument.
    
    ```jsx
    // The global variable
    const s = [23, 65, 98, 5];
    
    Array.prototype.myMap = function(callback) {
      const newArray = [];
      // for loop allows to apply the callback function to 
      // every item in the global array, and the push
      // the modified items to the empty new array
    for (let i = 0; i < this.length; i++) {
      newArray.push(callback(this[i]));
    }
     
      return newArray;
    };
    
    const new_s = s.myMap(function(item) {
      return item * 2;
    });
    
    console.log(new_s);// [ 46, 130, 196, 10 ]
    ```
    
- **Use the filter Method to Extract Data from an Array**
    
    `filter` calls a function on each element of an array and returns a new array containing only the elements for which that function returns `true`
    
    ```jsx
    // The global variable
    const watchList = [
      {
        "Title": "Inception",
        "Year": "2010",
        "Rated": "PG-13",
        "Released": "16 Jul 2010",
        "Runtime": "148 min",
        "Genre": "Action, Adventure, Crime",
        "Director": "Christopher Nolan",
        "Writer": "Christopher Nolan",
        "Actors": "Leonardo DiCaprio, Joseph Gordon-Levitt, Elliot Page, Tom Hardy",
        "Plot": "A thief, who steals corporate secrets through use of dream-sharing technology, is given the inverse task of planting an idea into the mind of a CEO.",
        "Language": "English, Japanese, French",
        "Country": "USA, UK",
        "Awards": "Won 4 Oscars. Another 143 wins & 198 nominations.",
        "Poster": "http://ia.media-imdb.com/images/M/MV5BMjAxMzY3NjcxNF5BMl5BanBnXkFtZTcwNTI5OTM0Mw@@._V1_SX300.jpg",
        "Metascore": "74",
        "imdbRating": "8.8",
        "imdbVotes": "1,446,708",
        "imdbID": "tt1375666",
        "Type": "movie",
        "Response": "True"
      },
      {
        "Title": "Interstellar",
        "Year": "2014",
        "Rated": "PG-13",
        "Released": "07 Nov 2014",
        "Runtime": "169 min",
        "Genre": "Adventure, Drama, Sci-Fi",
        "Director": "Christopher Nolan",
        "Writer": "Jonathan Nolan, Christopher Nolan",
        "Actors": "Ellen Burstyn, Matthew McConaughey, Mackenzie Foy, John Lithgow",
        "Plot": "A team of explorers travel through a wormhole in space in an attempt to ensure humanity's survival.",
        "Language": "English",
        "Country": "USA, UK",
        "Awards": "Won 1 Oscar. Another 39 wins & 132 nominations.",
        "Poster": "http://ia.media-imdb.com/images/M/MV5BMjIxNTU4MzY4MF5BMl5BanBnXkFtZTgwMzM4ODI3MjE@._V1_SX300.jpg",
        "Metascore": "74",
        "imdbRating": "8.6",
        "imdbVotes": "910,366",
        "imdbID": "tt0816692",
        "Type": "movie",
        "Response": "True"
      },
      {
        "Title": "The Dark Knight",
        "Year": "2008",
        "Rated": "PG-13",
        "Released": "18 Jul 2008",
        "Runtime": "152 min",
        "Genre": "Action, Adventure, Crime",
        "Director": "Christopher Nolan",
        "Writer": "Jonathan Nolan (screenplay), Christopher Nolan (screenplay), Christopher Nolan (story), David S. Goyer (story), Bob Kane (characters)",
        "Actors": "Christian Bale, Heath Ledger, Aaron Eckhart, Michael Caine",
        "Plot": "When the menace known as the Joker wreaks havoc and chaos on the people of Gotham, the caped crusader must come to terms with one of the greatest psychological tests of his ability to fight injustice.",
        "Language": "English, Mandarin",
        "Country": "USA, UK",
        "Awards": "Won 2 Oscars. Another 146 wins & 142 nominations.",
        "Poster": "http://ia.media-imdb.com/images/M/MV5BMTMxNTMwODM0NF5BMl5BanBnXkFtZTcwODAyMTk2Mw@@._V1_SX300.jpg",
        "Metascore": "82",
        "imdbRating": "9.0",
        "imdbVotes": "1,652,832",
        "imdbID": "tt0468569",
        "Type": "movie",
        "Response": "True"
      },
      {
        "Title": "Batman Begins",
        "Year": "2005",
        "Rated": "PG-13",
        "Released": "15 Jun 2005",
        "Runtime": "140 min",
        "Genre": "Action, Adventure",
        "Director": "Christopher Nolan",
        "Writer": "Bob Kane (characters), David S. Goyer (story), Christopher Nolan (screenplay), David S. Goyer (screenplay)",
        "Actors": "Christian Bale, Michael Caine, Liam Neeson, Katie Holmes",
        "Plot": "After training with his mentor, Batman begins his fight to free crime-ridden Gotham City from the corruption that Scarecrow and the League of Shadows have cast upon it.",
        "Language": "English, Urdu, Mandarin",
        "Country": "USA, UK",
        "Awards": "Nominated for 1 Oscar. Another 15 wins & 66 nominations.",
        "Poster": "http://ia.media-imdb.com/images/M/MV5BNTM3OTc0MzM2OV5BMl5BanBnXkFtZTYwNzUwMTI3._V1_SX300.jpg",
        "Metascore": "70",
        "imdbRating": "8.3",
        "imdbVotes": "972,584",
        "imdbID": "tt0372784",
        "Type": "movie",
        "Response": "True"
      },
      {
        "Title": "Avatar",
        "Year": "2009",
        "Rated": "PG-13",
        "Released": "18 Dec 2009",
        "Runtime": "162 min",
        "Genre": "Action, Adventure, Fantasy",
        "Director": "James Cameron",
        "Writer": "James Cameron",
        "Actors": "Sam Worthington, Zoe Saldana, Sigourney Weaver, Stephen Lang",
        "Plot": "A paraplegic marine dispatched to the moon Pandora on a unique mission becomes torn between following his orders and protecting the world he feels is his home.",
        "Language": "English, Spanish",
        "Country": "USA, UK",
        "Awards": "Won 3 Oscars. Another 80 wins & 121 nominations.",
        "Poster": "http://ia.media-imdb.com/images/M/MV5BMTYwOTEwNjAzMl5BMl5BanBnXkFtZTcwODc5MTUwMw@@._V1_SX300.jpg",
        "Metascore": "83",
        "imdbRating": "7.9",
        "imdbVotes": "876,575",
        "imdbID": "tt0499549",
        "Type": "movie",
        "Response": "True"
      }
    ];
    
    // map the array to reduce amount of data
    
    const filteredList = watchList.map(item => {
     return {
      title: item["Title"],
      rating: item["imdbRating"],
     };
    }).filter( item => {
      // return an lis tof item we needed only
      return parseFloat(item.rating) >= 8.0;
    });
    
    console.log(filteredList);
    
    /* 
    [ { title: 'Inception', rating: '8.8' },
      { title: 'Interstellar', rating: '8.6' },
      { title: 'The Dark Knight', rating: '9.0' },
      { title: 'Batman Begins', rating: '8.3' } ]
    */
    ```
 - **Implement the filter Method on a Prototype**
    
    ```jsx
    // The global variable
    const s = [23, 65, 98, 5];
    
    Array.prototype.myFilter = function(callback) {
      const newArray = [];
      this.forEach(function(x) {
    	if (callback(x) == true) {
    	 newArray.push(x);
     }
    });
      return newArray;
    };
    
    const new_s = s.myFilter(function(item) {
      return item % 2 === 1;
    });
    ```
    
- **Return Part of an Array Using the slice Method**
    
    the slice will returns a copy of certain elements of an array.
    
    containing two arguments; 1st will take begining, and 2nd will be end of slice.
    
    ```jsx
    function sliceArray(anim, beginSlice, endSlice) {
      return anim.slice(beginSlice, endSlice);
    }
    
    const inputAnim = ["Cat", "Dog", "Tiger", "Zebra", "Ant"];
    sliceArray(inputAnim, 1, 3);
    ```
    
- **Remove Elements from an Array Using slice Instead of splice**
    
    `splice` will delete of an item in array, and keep the rest from it.
    
    ```jsx
    function nonMutatingSplice(cities) {
      
       let newCity = cities.slice(0,3); // taking index of 0 to 3
       return newCity; // returning new array
    }
    
    const inputCities = ["Chicago", "Delhi", "Islamabad", "London", "Berlin"];
    console.log(nonMutatingSplice(inputCities)); // [ 'Chicago', 'Delhi', 'Islamabad' ]
    ```
    
- **Combine Two Arrays Using the concat Method**
    
    *Concatenation* means to join items end to end.
    
    ```jsx
    function nonMutatingConcat(original, attach) {
      let arr = original.concat(attach); // merging array
      return arr; // return new concatenated array
    }
    
    const first = [1, 2, 3];
    const second = [4, 5];
    console.log(nonMutatingConcat(first, second)); // [ 1, 2, 3, 4, 5 ]
    ```
    
- **Add Elements to the End of an Array Using concat Instead of push**
    
    Coz push adds an item to the end of the same array its called on. which concat just combine arrays into new one without mutating the original arrays.
    
    ```jsx
    function nonMutatingPush(original, newItem) {
      return original.concat(newItem);
    }
    
    const first = [1, 2, 3];
    const second = [4, 5];
    console.log(nonMutatingPush(first, second)); // 1, 2, 3, 4, 5 ]
    ```
    
- **Use the reduce Method to Analyze Data**
    
    The `reduce` method iterates over each item in an array and returns a single value (i.e. string, number, object, array). This is achieved via a callback function that is called on each iteration.
    
    
The `reduce` method iterates over each item in an array and returns a single value (i.e. string, number, object, array). This is achieved via a callback function that is called on each iteration.

```jsx

// The global variable
const watchList = [
  {
    "Title": "Inception",
    "Year": "2010",
    "Rated": "PG-13",
    "Released": "16 Jul 2010",
    "Runtime": "148 min",
    "Genre": "Action, Adventure, Crime",
    "Director": "Christopher Nolan",
    "Writer": "Christopher Nolan",
    "Actors": "Leonardo DiCaprio, Joseph Gordon-Levitt, Elliot Page, Tom Hardy",
    "Plot": "A thief, who steals corporate secrets through use of dream-sharing technology, is given the inverse task of planting an idea into the mind of a CEO.",
    "Language": "English, Japanese, French",
    "Country": "USA, UK",
    "Awards": "Won 4 Oscars. Another 143 wins & 198 nominations.",
    "Poster": "http://ia.media-imdb.com/images/M/MV5BMjAxMzY3NjcxNF5BMl5BanBnXkFtZTcwNTI5OTM0Mw@@._V1_SX300.jpg",
    "Metascore": "74",
    "imdbRating": "8.8",
    "imdbVotes": "1,446,708",
    "imdbID": "tt1375666",
    "Type": "movie",
    "Response": "True"
  },
  {
    "Title": "Interstellar",
    "Year": "2014",
    "Rated": "PG-13",
    "Released": "07 Nov 2014",
    "Runtime": "169 min",
    "Genre": "Adventure, Drama, Sci-Fi",
    "Director": "Christopher Nolan",
    "Writer": "Jonathan Nolan, Christopher Nolan",
    "Actors": "Ellen Burstyn, Matthew McConaughey, Mackenzie Foy, John Lithgow",
    "Plot": "A team of explorers travel through a wormhole in space in an attempt to ensure humanity's survival.",
    "Language": "English",
    "Country": "USA, UK",
    "Awards": "Won 1 Oscar. Another 39 wins & 132 nominations.",
    "Poster": "http://ia.media-imdb.com/images/M/MV5BMjIxNTU4MzY4MF5BMl5BanBnXkFtZTgwMzM4ODI3MjE@._V1_SX300.jpg",
    "Metascore": "74",
    "imdbRating": "8.6",
    "imdbVotes": "910,366",
    "imdbID": "tt0816692",
    "Type": "movie",
    "Response": "True"
  },
  {
    "Title": "The Dark Knight",
    "Year": "2008",
    "Rated": "PG-13",
    "Released": "18 Jul 2008",
    "Runtime": "152 min",
    "Genre": "Action, Adventure, Crime",
    "Director": "Christopher Nolan",
    "Writer": "Jonathan Nolan (screenplay), Christopher Nolan (screenplay), Christopher Nolan (story), David S. Goyer (story), Bob Kane (characters)",
    "Actors": "Christian Bale, Heath Ledger, Aaron Eckhart, Michael Caine",
    "Plot": "When the menace known as the Joker wreaks havoc and chaos on the people of Gotham, the caped crusader must come to terms with one of the greatest psychological tests of his ability to fight injustice.",
    "Language": "English, Mandarin",
    "Country": "USA, UK",
    "Awards": "Won 2 Oscars. Another 146 wins & 142 nominations.",
    "Poster": "http://ia.media-imdb.com/images/M/MV5BMTMxNTMwODM0NF5BMl5BanBnXkFtZTcwODAyMTk2Mw@@._V1_SX300.jpg",
    "Metascore": "82",
    "imdbRating": "9.0",
    "imdbVotes": "1,652,832",
    "imdbID": "tt0468569",
    "Type": "movie",
    "Response": "True"
  },
  {
    "Title": "Batman Begins",
    "Year": "2005",
    "Rated": "PG-13",
    "Released": "15 Jun 2005",
    "Runtime": "140 min",
    "Genre": "Action, Adventure",
    "Director": "Christopher Nolan",
    "Writer": "Bob Kane (characters), David S. Goyer (story), Christopher Nolan (screenplay), David S. Goyer (screenplay)",
    "Actors": "Christian Bale, Michael Caine, Liam Neeson, Katie Holmes",
    "Plot": "After training with his mentor, Batman begins his fight to free crime-ridden Gotham City from the corruption that Scarecrow and the League of Shadows have cast upon it.",
    "Language": "English, Urdu, Mandarin",
    "Country": "USA, UK",
    "Awards": "Nominated for 1 Oscar. Another 15 wins & 66 nominations.",
    "Poster": "http://ia.media-imdb.com/images/M/MV5BNTM3OTc0MzM2OV5BMl5BanBnXkFtZTYwNzUwMTI3._V1_SX300.jpg",
    "Metascore": "70",
    "imdbRating": "8.3",
    "imdbVotes": "972,584",
    "imdbID": "tt0372784",
    "Type": "movie",
    "Response": "True"
  },
  {
    "Title": "Avatar",
    "Year": "2009",
    "Rated": "PG-13",
    "Released": "18 Dec 2009",
    "Runtime": "162 min",
    "Genre": "Action, Adventure, Fantasy",
    "Director": "James Cameron",
    "Writer": "James Cameron",
    "Actors": "Sam Worthington, Zoe Saldana, Sigourney Weaver, Stephen Lang",
    "Plot": "A paraplegic marine dispatched to the moon Pandora on a unique mission becomes torn between following his orders and protecting the world he feels is his home.",
    "Language": "English, Spanish",
    "Country": "USA, UK",
    "Awards": "Won 3 Oscars. Another 80 wins & 121 nominations.",
    "Poster": "http://ia.media-imdb.com/images/M/MV5BMTYwOTEwNjAzMl5BMl5BanBnXkFtZTcwODc5MTUwMw@@._V1_SX300.jpg",
    "Metascore": "83",
    "imdbRating": "7.9",
    "imdbVotes": "876,575",
    "imdbID": "tt0499549",
    "Type": "movie",
    "Response": "True"
  }
];

function getRating(watchList) {
  // Filter which directed by Christoper
  const avgRating = watchList.filter(film => film.Director === "Christopher Nolan")
  // map to convert rating into number
  .map(film => Number(film.imdbRating))
  // reduce to add ratings
  .reduce((sumOfRatings, rating) => sumOfRatings + rating) /
  // devide by total of nolan film
  watchList.filter(film => film.Director === "Christopher Nolan").length;
 

  // Only change code above this line
  return avgRating;
}

console.log(getRating(watchList));
```

- **Use Higher-Order Functions map, filter, or reduce to Solve a Complex Problem**
    
    ```jsx
    const squareList = arr => {
      
    // usinfilter and map function to square all positive integers
      return arr
      .filter(num => num > 0 && num % parseInt(num) === 0)
    .map(num => Math.pow(num,2));
      
    };
    
    const squaredIntegers = squareList([-3, 4.8, 5, 3, -3.2]);
    console.log(squaredIntegers);
    ```
    
- **Sort an Array Alphabetically using the sort Method**
    
    ```jsx
    function alphabeticalOrder(arr) {
      
      return arr.sort(function(a,b){
        return a === b ? 0 : a > b ? 1: -1;
      });
      
    }
    
    console.log(alphabeticalOrder(["a", "d", "c", "a", "z", "g"]));
    ```
    
- **Return a Sorted Array Without Changing the Original Array**
    
    ```jsx
    const globalArray = [5, 6, 3, 2, 9];
    
    function nonMutatingSort(arr) {
      // copy array without mutating using slice method
      let newArr = arr.slice();
    	// sort the new array descendantly
      return newArr.sort(function(a,b){
        return a === b ? 0 : a > b ? 1: -1;
      });
    
    console.log(nonMutatingSort(globalArray)); // [3,3,5,6,9]
    ```
    
- **Split a String into an Array Using the split Method**
    
    The split method will splits a string into an array of strings.
    
    ```jsx
    function splitify(str) {
    		// /\W/ Matches any non-word character.
    		// This includes spaces and punctuation, but not underscores
        let arr = str.split(/\W/);
        return arr;
    }
    
    console.log(splitify("Hello World,I-am code")); 
    // [ 'Hello', 'World', 'I', 'am', 'code' ]
    ```
    
- **Combine an Array into a String Using the join Method**
    
    The `join` method is used to join the elements of an array together to create a string.
    
    ```jsx
    function sentensify(str) {
      // split the array into strings
      let newStr = str.split(/\W/);
    	// join the array without strings
      const myStr = newStr.join(" ");
    	//  return the final join
      return myStr;
    }
    
    console.log(sentensify("May-the-force-be-with-you")); // May the force be with you
    ```
    
- **Apply Functional Programming to Convert Strings to URL Slugs**
    
    ```jsx
    
    function urlSlug(title) {
      return title
        .toLowerCase() // turn all lower case
        .trim() // remove any more than one spacing
        .split(/\s+/) // split into string
        .join("-"); // join all into hyphen
    
    }
    
    console.log(urlSlug("A Mind Needs Books Like A Sword Needs A Whetstone"));
    
    // a-mind-needs-books-like-a-sword-needs-a-whetstone
    ```
   
 
- **Use the every Method to Check that Every Element in an Array Meets a Criteria** -
  
- **Use the every Method to Check that Every Element in an Array Meets a Criteria**
    
    ```jsx
    function checkPositive(arr) {
      return arr.every(val => val > 0);
    }
    
    console.log(checkPositive([1, 2, 3, -4, 5])); // false
    ```
    
- **Use the some Method to Check that Any Elements in an Array Meet a Criteria**
    
    ```jsx
    function checkPositive(arr) {
    return arr.some(val => val > 0);
    }
    
    console.log(checkPositive([1, 2, 3, -4, 5])); // true
    ```
    
- **Introduction to Currying and Partial Application**
    
    ```jsx
    function add(x) {
      return function(y) {
        return function(z) {
    	    return x + y + z;
            };
      };
    }
    console.log(add(10)(20)(30)); // 60 
    ```

Intermediate Algorithm Scripting

- **Sum All Numbers in a Range**
    
    Return the sum of those two numbers plus the sum of all the numbers between them. The lowest number will not always come first.
    
    ```jsx
    function sumAll(arr) {
      let max = Math.max(arr[0], arr[1]);
      let min = Math.min(arr[0], arr[1]);
      let sumBetween = 0;
      for (let i = min; i <= max; i++) {
    	  sumBetween += i;
        }
        return sumBetween;
      }
    
    console.log(sumAll([1, 4])); // 10
    ```
  
  
- **Diff Two Arrays**
    
    Compare two arrays and return a new array with any items only found in one of the two given arrays, but not both.
    
    ```jsx
    
    function diffArray(arr1, arr2) {
      // creating new array
    let newArr = [];
    
    // loop through array to capture unique item
    function checkInFirst(first, second) {
      for (var i = 0; i < first.length; i++) {
        if (second.indexOf(first[i]) === -1) {
    // pushing unique item to first array
        newArr.push(first[i]);
        }
      }
    }
    
    checkInFirst(arr1, arr2);
    checkInFirst(arr2, arr1);
    return newArr;
    }
    
    console.log(diffArray([1, 2, 3, 5], [1, 2, 3, 4, 5])); // 4
    ```
    
- **Seek and Destroy**
    
    provided with an initial array (the first argument in the `destroyer`function), followed by one or more arguments. Remove all elements from the initial array that are of the same value as these arguments.
    
    ```jsx
    function destroyer(arr) {
    // create a new array for comparison  
    let valRemove = Object.values(arguments).slice(1);
    
    // iterate the object between two array and compare them
      for (let i = 0; i < arr.length; i++) {
        for (let j = 0; j < valRemove.length; j++) {
          
    // if the item equal, delete it
    if (arr[i] === valRemove[j]) {
            delete arr[i];
          }
        }
      }
     
    // return filtered item that was not null 
      return arr.filter(item => item !== null);
    }
    
    console.log(destroyer([1, 2, 3, 1, 2, 3], 2, 3)); // [ 1, 1 ]
    ```
    

- **Wherefore art thou**
    
    Making function that looks thrugh an array of objects (first argument) and returns an array of all objects that have matching name and value pairs (second argument).
    
    ```jsx
    function whatIsInAName(collection, source) {
      const arr = Object.keys(source);
    
      // filter through the collection
      return collection.filter(function(obj) {
        // compare every object inside the collection
        return arr.every(function(key){
          // return only similar properties
          return obj.hasOwnProperty(key) && obj[key] === source[key];
    
        });
      });
      
    }
    
    console.log(whatIsInAName([{ first: "Romeo", last: "Montague" }, { first: "Mercutio", last: null }, { first: "Tybalt", last: "Capulet" }], { last: "Capulet" }));
    
    // [{ first: 'Tybalt', last: 'Capulet' } ]
    ```
    
- **Spinal Tap Case**
    
    Convert a string into spinal case. 
    
    Spinal case is all-lowercase-words-joined-by-dashes.
    
    ```jsx
    function spinalCase(str) {
      // replace low-uppercase to low-space-uppercase
      str = str.replace(/([a-z])([A-Z])/g, "$1 $2")
      
      // split the whitespace and underscore and join them with dashes
      return str
      .toLowerCase()
      .split(/(?:_| )+/)
      .join("-");
    }
    
    console.log(spinalCase('This Is Spinal Tap')); // this-is-spinal-tap
    ```
    
- **Pig Latin**
    
    Pig Latin is a way of altering English Words.
    
    ```jsx
    // start at beginning and get longest match of everything not a vowel (consonants)
    // if regex pattern found, it saves the match; else, it returns null
    // if regex pattern found (starts with consonants), it deletes match, adds the match to the end, and adds “ay” to the end
    // if regex pattern not found (starts with vowels), it just adds “way” to the ending
    
    function translatePigLatin(str) {
      let consonantRegex = /^[^aiueo]+/;
      let myConsonants = str.match(consonantRegex);
      return myConsonants !== null ? str
        .replace(consonantRegex,"")
        .concat(myConsonants)
        .concat("ay")
        : str.concat("way");
    }
    
    console.log(translatePigLatin("consonant")); // onsonantway
    ```
    
Day 42 of #100DaysOfCode

- **Search and Replace**
    
    Search and replace using given arguments
    
    ```jsx
    function myReplace(str, before, after) {
      // find index of before on the string
      var index = str.indexOf(before);
      // check if the first letter is uppercase or otherwise
      if(str[index] === str[index].toUpperCase()) {
        // change the after word to capital
        after = after.charAt(0).toUpperCase() + after.slice(1);
      } else {
        // change the after word into uncapital
        after = after.charAt(0).toLowerCase() + after.slice(1);
      }
      // replace the str with new one
      str = str.replace(before, after);
      
      return str;
    }
    
    console.log(myReplace("A quick brown fox jumped over the lazy dog", "jumped", "leaped")); 
    // "A quick brown fox leaped over the lazy dog"
    ```
    
    
- **DNA Pairing**
    
    Finding the missing element. between two character
    
    ```jsx
    function pairElement(str) {
      var pairs = {
        A: "T",
        T: "A",
        C: "G",
        G: "C",
      };
      // split into array of character 
      var arr = str.split("");
      // map character to array of character & matching pair
      return arr.map(x => [x, pairs[x]]);
    }
    
    console.log(pairElement("GCG")); // [ [ 'G', 'C' ], [ 'C', 'G' ], [ 'G', 'C' ] ]
    ```
    
- **Missing letters**
    
    Finding the missing letter in the passed letter range
    
    ```jsx
    function fearNotLetter(str) {
      // loop through the item in array
      for (var i = 0; i < str.length; i++) {
        // ASCII code for current character
        var code = str.charCodeAt(i);
    
        // if the currrent item not match with the first, and no iteration, means the item has escape
        if (code !== str.charCodeAt(0) + i) {
          // if current item has escape on character, find prev char and return it
          return String.fromCharCode(code-1);
        }
      }
    
      return undefined;
    }
    
    console.log(fearNotLetter("abce")); // d
    ```
    
- **Sorted Union**
    
    ```jsx
    function uniteUnique(arr) {
      // Creates an empty array to store our final result.
      var finalArray = [];
    
      // Loop through the arguments object to truly make the program work with two or more arrays
      // instead of 3.
      for (var i = 0; i < arguments.length; i++) {
        var arrayArguments = arguments[i];
    
        // Loops through the array at hand
        for (var j = 0; j < arrayArguments.length; j++) {
          var indexValue = arrayArguments[j];
    
          // Checks if the value is already on the final array.
          if (finalArray.indexOf(indexValue) < 0) {
            finalArray.push(indexValue);
          }
        }
      }
    
      return finalArray;
    }
    
    console.log(uniteUnique([1, 3, 2], [5, 2, 1, 4], [2, 1])); // [ 1, 3, 2, 5, 4 ]
    ```
    
- **Convert HTML Entities**
    
    converting the characters `&`, `<` , `>`, `"` (double quote) and `'` (apostrophe), in a string to their corresponding HTML entities.
    
    ```jsx
    function convertHTML(str) {
      // split all charcter into stand alone item
      let temp = str.split("");
      // use switch to replace HTML Entities
      for (let i = 0; i < temp.length; i++){
        switch(temp[i]) {
          case "<":
            temp[i] = "&lt;";
            break;
          case "&":
            temp[i] = "&amp;";
            break;
          case ">":
            temp[i] = "&gt;";
            break;
          case '"':
            temp[i] = "&quot;";
            break;
          case "'":
            temp[i] = "&apos;";
            break;
    
        }
      }
      temp = temp.join("");
      return temp;
    }
    
    console.log(convertHTML("Dolce & Gabbana")); // Dolce &amp; Gabbana
    ```
    
 
