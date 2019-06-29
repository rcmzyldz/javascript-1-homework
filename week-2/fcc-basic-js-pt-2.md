> complete the rest of [basic JS exercises](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/basic-javascript) on FCC and paste each of your solutions into this file.  This will allow you to use your FCC exercises as a study reference later on  
> [completed example](https://github.com/AlfiYusrina/hyf-javascript1/blob/master/week1/freecode_camp_solutions.MD) 





## Selecting from Many Options with Switch Statements
```js
function caseInSwitch(val) {
  var answer = "";
  switch(val) {
  case 1:
    return "alpha";
    break;
  case 2:
    return "beta";
    break;
  case 3:
    return "gamma";
    break;
     case 4:
   return "delta";
    break;
}

  return answer;
}

caseInSwitch(1);
caseInSwitch(2);
caseInSwitch(3);
caseInSwitch(4);
```

## Adding a Default Option in Switch Statements
```js
function switchOfStuff(val) {
  var answer = "";
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
}

  return answer;
}

switchOfStuff(1);
```

## Multiple Identical Options in Switch Statements
```js
function sequentialSizes(val) {
  var answer = "";
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
}
  return answer;
}

sequentialSizes(1);

```

## Replacing If Else Chains with Switch
```js
function chainToSwitch(val) {
  var answer = "";

  switch(val) {
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
  default:
    answer = "";
    break;
}

  return answer;
}

chainToSwitch(7);

```

## Returning Boolean Values from Functions
```js
function isLess(a, b) {
  return a < b;
}

isLess(10, 15);
```

## Return Early Pattern for Functions
```js
function abTest(a, b) {
 if (a < 0 || b < 0) {
   return undefined;
 }else{
  return Math.round(Math.pow(Math.sqrt(a) + Math.sqrt(b), 2));
}

}
abTest(2,2);
```

## Counting Cards
```js
var count = 0;

function cc(card) {
switch(card){
    case 2:
    case 3:
    case 4:
    case 5:
    case 6:
      count++;
      break;
    case 10:
    case "J":
    case "Q":
    case "K":
    case "A":
      count--;
      break;
  }
  if (count > 0){
    return count + " Bet";
  } else {
    return count + " Hold";
  }
}

cc(2); cc(3); cc(7); cc('K'); cc('A');
```

## Build JavaScript Objects
```js
var myDog = {
    "name": "Brownie",
  "legs": 4,
  "tails": 1,
  "friends": ["me"]
};
```

## Accessing Object Properties with Dot Notation
```js

var testObj = {
  "hat": "ballcap",
  "shirt": "jersey",
  "shoes": "cleats"
};

var hatValue = testObj.hat;
var shirtValue = testObj.shirt;
```
## Accessing Object Properties with Bracket Notation
```js
var testObj = {
  "an entree": "hamburger",
  "my side": "veggies",
  "the drink": "water"
};
var entreeValue = testObj["an entree"];
var drinkValue = testObj["the drink"];
```

## Accessing Object Properties with Variables
```js
var testObj = {
  12: "Namath",
  16: "Montana",
  19: "Unitas"
};
var playerNumber = 16;
var player = testObj[playerNumber];
```

## Updating Object Properties
```js
var myDog = {
  "name": "Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"]
};
myDog.name = "Happy Coder";
```

## Add New Properties to a JavaScript Object
```js
var myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"]
};


myDog["bark"] = "woof";
```

## Delete Properties from a JavaScript Object
```js
// Example
var ourDog = {
  "name": "Camper",
  "legs": 4,
  "tails": 1,
  "friends": ["everything!"],
  "bark": "bow-wow"
};

delete ourDog.bark;

// Setup
var myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"],
  "bark": "woof"
};

// Only change code below this line.
delete myDog.tails;

```

## Using Objects for Lookups
```js

function phoneticLookup(val) {
  var result = "";

  var lookup = {
 "alpha": "Adams",
  "bravo": "Boston",
  "charlie": "Chicago",
  "delta": "Denver",
  "echo": "Easy",
  "foxtrot": "Frank"
  };
  result = lookup[val];
  return result;
}

phoneticLookup("charlie");
```

## Testing Objects for Properties
```js
var myObj = {
  gift: "pony",
  pet: "kitten",
  bed: "sleigh"
};

function checkObj(checkProp) {
 return myObj.hasOwnProperty(checkProp) ? myObj[checkProp]: "Not Found";
}

checkObj("gift");
```

## Manipulating Complex Objects
```js
var myMusic = [
  {
    "artist": "Billy Joel",
    "title": "Piano Man",
    "release_year": 1973,
    "formats": [
      "CD",
      "8T",
      "LP"
    ],
    "gold": true
  },
  {

   "artist": "JLO",
    "title": "Girl",
    "release_year": 1999,
    "formats": [
      "Vinnyl",
      "8T",
      "LP"
    ]
  }
];
```

## Accessing Nested Objects
```js
var myStorage = {
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

var gloveBoxContents = myStorage.car.inside["glove box"];

```

## Accessing Nested Arrays
```js
// Setup
var myPlants = [
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

var secondTree = myPlants[1].list[1];
```

## Record Collection
```js
var collection = {
    "2548": {
      "album": "Slippery When Wet",
      "artist": "Bon Jovi",
      "tracks": [
        "Let It Rock",
        "You Give Love a Bad Name"
      ]
    },
    "2468": {
      "album": "1999",
      "artist": "Prince",
      "tracks": [
        "1999",
        "Little Red Corvette"
      ]
    },
    "1245": {
      "artist": "Robert Palmer",
      "tracks": [ ]
    },
    "5439": {
      "album": "ABBA Gold"
    }
};
// Keep a copy of the collection for tests
var collectionCopy = JSON.parse(JSON.stringify(collection));


function updateRecords(id, prop, value) {
  if (prop === "tracks" && value !== ""){
    if (collection[id][prop]){
      collection[id][prop].push(value);
    }else{
      collection[id][prop] = [value];
    }
  } else if (value !== "") {
     collection[id][prop] = value;
  } else {
    delete collection[id][prop];
  }
  return collection;
}
updateRecords(5439, "artist", "ABBA");
```

## Iterate with JavaScript While Loops
```js

var myArray = [];
var i = 0;
while(i <= 4) {
  myArray.push(i);
  i++;
}

```

## Iterate with JavaScript For Loops
```js
var myArray = [];
for (var i = 1; i <= 5; i++) {
    myArray.push(i);
}
```

## Iterate Odd Numbers With a For Loop
```js
var myArray = [];
for (var i = 1; i <= 9; i += 2){
  myArray.push(i);
}
```

## Count Backwards With a For Loop
```js
var myArray = [];
for (var i = 9; i > 0; i -= 2){
  myArray.push(i);
}
```

## Iterate Through an Array with a For Loop
```js
var myArr = [ 2, 3, 4, 5, 6];
var total = 0;
for(var i = 0; i < myArr.length; i++){
  total += myArr[i];
}
```

## Nesting For Loops
```js
function multiplyAll(arr) {
  var product = 1;
  for (var i=0; i < arr.length; i++) {
    for (var j=0; j < arr[i].length; j++) {
    product = product * arr[i][j];
    }
  }
  return product;
}
multiplyAll([[1,2],[3,4],[5,6,7]]);
```

## Iterate with JavaScript Do While Loops
```js
var myArray = [];
var i = 10;

do {
 myArray.push(i);
  i++;
} while (i < 5);
```

## Profile Lookup
```js
var contacts = [
    {
        "firstName": "Akira",
        "lastName": "Laine",
        "number": "0543236543",
        "likes": ["Pizza", "Coding", "Brownie Points"]
    },
    {
        "firstName": "Harry",
        "lastName": "Potter",
        "number": "0994372684",
        "likes": ["Hogwarts", "Magic", "Hagrid"]
    },
    {
        "firstName": "Sherlock",
        "lastName": "Holmes",
        "number": "0487345643",
        "likes": ["Intriguing Cases", "Violin"]
    },
    {
        "firstName": "Kristian",
        "lastName": "Vos",
        "number": "unknown",
        "likes": ["JavaScript", "Gaming", "Foxes"]
    }
];


function lookUpProfile(name, prop){
for(var i = 0; i < contacts.length; i++){
  var contact = contacts[i];
  if (contact.firstName === name){
    if(contact.hasOwnProperty(prop)){
      return contact[prop];
    }else {
      return "No such property";
    }
  }
}
return "No such contact";
}

lookUpProfile("Akira", "likes");
```

## Generate Random Fractions with JavaScript
```js
function randomFraction() {

  return Math.random();
}
```

## Generate Random Whole Numbers with JavaScript
```js
var randomNumberBetween0and19 = Math.floor(Math.random() * 20);
function randomWholeNum() {
  return Math.floor(Math.random() * 10);
}
```

## Generate Random Whole Numbers within a Range
```js
function randomRange(myMin, myMax) {
  return Math.floor(Math.random() * (myMax - myMin + 1)) + myMin;
}
var myRandom = randomRange(5, 15);
```

## Use the parseInt Function
```js
function convertToInteger(str) {
  return parseInt(str);
}

convertToInteger("56");
```

## Use the parseInt Function with a Radix
```js
function convertToInteger(str) {
  return parseInt(str, 2);
}

convertToInteger("10011");
```

## Use the Conditional Ternary Operator
```js
function checkEqual(a, b) {
  return a === b ? true : false;
}

checkEqual(1, 2);
```

## Use Multiple Conditional Ternary Operators
```js
function checkSign(num) {
  return num === 0 ? "zero" : num > 0 ? "positive" : "negative";
}

checkSign(10);
```
