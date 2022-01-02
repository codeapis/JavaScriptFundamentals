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
