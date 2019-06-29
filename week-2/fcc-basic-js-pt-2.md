> complete the rest of [basic JS exercises](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/basic-javascript) on FCC and paste each of your solutions into this file.  This will allow you to use your FCC exercises as a study reference later on  
> [completed example](https://github.com/AlfiYusrina/hyf-javascript1/blob/master/week1/freecode_camp_solutions.MD) 





73.Selecting from Many Options with Switch Statements
function caseInSwitch(val) {
  var answer = "";
  
  switch(val){
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
74.Adding a Default Option in Switch Statements
function switchOfStuff(val) {
  var answer = "";
 switch(val){
    case 'a': answer = 'apple'; 
    break;
    case 'b': answer = 'bird'; 
    break;
    case 'c': answer = 'cat'; 
    break;
    default: answer = 'stuff';
  }
  return answer;  
}
75.Multiple Identical Options in Switch Statements
function sequentialSizes(val) {
  var answer = "";
  switch(val){
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
76.Replacing If Else Chains with Switch
function chainToSwitch(val) {
  var answer = "";
  
  switch (val) {
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
    case 7 :
      answer = "Ate Nine";
      break;
  }
  
  return answer;  
}
77.Returning Boolean Values from Functions
function isLess(a, b) {
  return a<=b;
}
isLess(9, 15);
78.Return Early Pattern for Functions
function abTest(a, b) {

    if (a < 0 || b < 0) {
    return;
    }

  return Math.round(Math.pow(Math.sqrt(a) + Math.sqrt(b), 2));
}
