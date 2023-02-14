# test-javascript-platzi 🚀

### 1️⃣ Answer the following questions in the comments section:

- What is a variable and how to work it?
  It is an element that stores information, it can be a number, a string, a boolean, an array, an object, etc.
  It is declared with the keyword var, let or const.
  It works with the following syntax:

```javascript
var name = "Aldo";
var age = 25;
var isDeveloper = true;
```

- What is difference between declaring and initiating a variable?
  Declaring a variable is to create it, while initializing it is to assign it a value.
  It works with the following syntax:

```javascript
var name; // Declaring
name = "Aldo"; // Initializing
```

- What is difference between adding numbers and concatenating strings?
  When adding numbers, the result is the sum of the numbers, while when concatenating strings, the result is the union of the strings.
  It works with the following syntax:

```javascript
var number = 1 + 1; // 2
var string = "Hello" + "World"; // HelloWorld
```

- Which operators allow us to add or concatenate?
  The operators that allow us to add are + and +=, while the operators that allow us to concatenate are + and +=.
  It works with the following syntax:

```javascript
var number = 1 + 1; // 2
number += 1; // 3
var string = "Hello" + "World"; // HelloWorld
string += "!!"; // HelloWorld!!
```

### 2️⃣ Determine the name and data type to store the following information in variables:

- Name "String"
- Last name "String"
- Username at platzi "String"
- Age "Number"
- Email "String"
- IsAdult "Boolean"
- SavedMoney "Number"
- Debt "Number"

### 3️⃣ Translate the variables in the previous example to JavaScript code and leave your code in the comments.

```javascript
var name = "Aldo";
var lastName = "Balderrama";
var username = "abalderrama";
var age = 25;
var email = "abalderrama@platzi.com";
var isAdult = true;
var savedMoney = 0;
var debt = 0;
```

### 4️⃣ Calculate and print the following variables from the variables in the previous example:

- Full name

```javascript
let name = "Aldo";
let lastName = "Balderrama";
console.log(`Full name: ${name}  ${lastName}`); // Aldo Balderrama
```

- Total money

```javascript
let savedMoney = 2000;
let debt = 400;
console.log(`Total money: $${savedMoney - debt}`); // 0
```

## Functions

### 1️⃣ Answer the following questions in the comments section:

- What is a function?
  It is a block of code that is executed when it is called.
  It works with the following syntax:

```javascript
function myFunction() {
  // Code to be executed
}
```

- When is it useful for me to use a function in my code?
  It is useful when you want to reuse the same code several times, or when you want to separate the code into different parts.

- What is difference between parameters and arguments?
  Parameters are the variables that are declared in the function, while arguments are the values that are passed to the function when it is called.
  It works with the following syntax:

```javascript
function myFunction(parameter1, parameter2) {
  // Code to be executed
}
myFunction(argument1, argument2);
```

2️⃣ Convert the following code into a function, but changing when necessary the constant variables for parameters and arguments in a function:

```javascript
const name = "Aldo";
const lastName = "Balderrama";
const fullName = name + lastName;
const nickname = "abalderrama";

console.log(
  "My name is " + fullName + ", but I prefer that you tell me " + nickname + "."
);
```

```javascript
function myFunction(name, lastName, nickname) {
  const fullName = name + lastName;
  console.log(
    `My name is ${fullName}, but I prefer that you tell me ${nickname}.`
  );
}
myFunction("Aldo", "Balderrama", "abalderrama");
```

## Conditionals

### 1️⃣ Answer the following questions in the comments section:

- What is a conditional?
  It is a block of code that is executed when a condition is met.
  It works with the following syntax:

```javascript
if (condition) {
  // Code to be executed
}
```

- What kind of conditions exist in JavaScript and What are differences between them?
  There are two types of conditions, the if and the if-else.
  The if condition is executed when the condition is true, while the if-else condition is executed when the condition is true, and if it is false, it is executed the else condition.
  Also it has switch condition, which is executed when the condition is equal to the case.
  Ternary condition is a short way to write an if-else condition.
  It works with the following syntax:

```javascript
// If condition
if (condition) {
  // Code to be executed
} else {
  // Code to be executed
}

// Multiple conditions
if (condition) {
  // Code to be executed
} else if (condition) {
  // Code to be executed
} else {
  // Code to be executed
}

// Switch condition
switch (condition) {
  case value1:
    // Code to be executed
    break;
  case value2:
    // Code to be executed
    break;
  default:
  // Code to be executed
}

// Ternary condition
condition ? code1 : code2;
```

- Can I combine functions and conditionals?
  Yes, you can combine functions and conditionals.

### 2️⃣ Replicate the behavior of the following code that uses the switch statement using if, else and else if:

```javascript
const tipoDeSuscripcion = "Basic";

switch (tipoDeSuscripcion) {
  case "Free":
    console.log("Solo puedes tomar los cursos gratis");
    break;
  case "Basic":
    console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
    break;
  case "Expert":
    console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
    break;
  case "ExpertPlus":
    console.log(
      "Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año"
    );
    break;
}
```

My Solution:

```javascript
const tipoDeSuscripcion = "Basic";
if (tipoDeSuscripcion === "Free") {
  console.log("Solo puedes tomar los cursos gratis");
} else if (tipoDeSuscripcion === "Basic") {
  console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
} else if (tipoDeSuscripcion === "Expert") {
  console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
} else if (tipoDeSuscripcion === "ExpertPlus") {
  console.log(
    "Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año"
  );
}
```

### 3️⃣ Replicate the behavior of your previous conditional with if, else and else if, but now only with if (without else or else if).

💡 Bonus: If you are already an expert in the language, I challenge you to comment on how to replicate this behavior with arrays or objects and a single conditional. 😏

```javascript
const typeSubscription = "Basic";
const subscriptions = [
  {
    type: "Free",
    message: "Solo puedes tomar los cursos gratis",
  },
  {
    type: "Basic",
    message: "Puedes tomar casi todos los cursos de Platzi durante un mes",
  },
  {
    type: "Expert",
    message: "Puedes tomar casi todos los cursos de Platzi durante un año",
  },
  {
    type: "ExpertPlus",
    message:
      "Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año",
  },
];

// Option 1
subscriptions.forEach((subscription) => {
  if (typeSubscription === subscription.type) {
    console.log(subscription.message);
  }
});

// Option 2
console.log(
  subscriptions.find((subcription) => subcription.type === typeSubscription)
    .message
);
```

## Loops

### 1️⃣ Answer the following questions in the comments section:

- What is a loop?
  It is a block of code that is executed repeatedly until a condition is met.
  It works with the following syntax:

```javascript
for (initialization; condition; final - expression) {
  // Code to be executed
}
```

- What kind of loops exist in JavaScript?
  There are three types of loops, the for, the while and the do-while.
  The for loop is executed when the condition is true, while the while loop is executed when the condition is true, and if it is false, it is executed the else condition.
  Also it has switch condition, which is executed when the condition is equal to the case.
  Ternary condition is a short way to write an if-else condition.
  It works with the following syntax:

  ```javascript
  // For loop
  for (initialization; condition; final - expression) {
    // Code to be executed
  }
  // While loop
  while (condition) {
    // Code to be executed
  }
  // Do-while loop
  do {
    // Code to be executed
  } while (condition);
  ```

  ### 2️⃣ Replicates the behavior of the following for loops using while loops:

```javascript
for (let i = 0; i < 5; i++) {
  console.log("El valor de i es: " + i);
}

for (let i = 10; i >= 2; i--) {
  console.log("El valor de i es: " + i);
}
```

My Solution:

```javascript
let i = 0;
while (i < 5) {
  console.log("El valor de i es: " + i);
  i++;
}
i = 10;
while (i >= 2) {
  console.log("El valor de i es: " + i);
  i--;
}
```

### 3️⃣ Write a JavaScript code that asks users how much 2 + 2 is. If they answer correctly, we show a congratulations message, but if they answer wrong, we start over. 💡 Hint: you can use the JavaScript prompt function.

```javascript
let answer = prompt("How much is 2 + 2?");
while (answer != 4) {
  answer = prompt("How much is 2 + 2?");
}
alert("Congratulations!");
```

## List

### 1️⃣ Answer the following questions in the comments section:

- What is an array?
  It is an ordered collection of data(either primitive or object depending upon the language). Array are used to store multiple values in a single variable. It is a collection of elements.
  Example:

```javascript
const array = [element1, element2, element3];
```

- What is an object?
  It is is an standalone entity, with properties and type.
  Example:

```javascript
const object = {
  key1: value1,
  key2: value2,
  key3: value3,
};
```

- When is better use objects or arrays?
  It depends on the situation, if you need to store a list of values, you can use an array, but if you need to store a list of values with a key, you can use an object.
  Example:

```javascript
// Array
const array = ["element1", "element2", "element3"];
// Object
const object = {
  key1: "value1",
  key2: "value2",
  key3: "value3",
};
```

- Can I mix objects and arrays?
  Yes, you can mix objects and arrays.
  Example:

```javascript
const array = [
  "element1",
  "element2",
  "element3",
  {
    key1: "value1",
    key2: "value2",
    key3: "value3",
  },
];
```

### 2️⃣ Create a function that can receive any array as a parameter and print its first element.

```javascript
const array = ["element1", "element2", "element3"];
const printFirstElement = (array) => {
  console.log(array[0]);
};
printFirstElement(array);

// Or
const printFirstElement = (array) => {
  console.log(array.shift());
};
printFirstElement(array);
```

### 3️⃣ Create a function that can receive any array as a parameter and print all its elements one by one (printing the entire array is not valid).

```javascript
const array = ["element1", "element2", "element3"];
const printAllElements = (array) => {
  array.forEach((element) => {
    console.log(element);
  });
};
printAllElements(array);
// Or
const printAllElements = (array) => {
  for (let i = 0; i < array.length; i++) {
    console.log(array[i]);
  }
};
printAllElements(array);
// Or
const printAllElements = (array) => {
  for (const element of array) {
    console.log(element);
  }
};
printAllElements(array);
```

### 4️⃣ Create a function that can receive any object as a parameter and print all its elements one by one (printing the entire object is not valid).

```javascript
const object = {
  key1: "value1",
  key2: "value2",
  key3: "value3",
};
const printAllElements = (object) => {
  for (const key in object) {
    console.log(object[key]);
  }
};
printAllElements(object);
// Or
const printAllElements = (object) => {
  Object.values(object).forEach((value) => {
    console.log(value);
  });
};
printAllElements(object);
```
