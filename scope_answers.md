1.
var lastWord = 'welcome';
console.log(lastWord);
lastWord = 'goodbye';

--->  O/P : welcome

      Value of lastWord variable is 'welcome' when console.log is being called.
      So, no matter what the value is after function is being called already


2.
var message = "Up here!";
  function shout() {
    console.log(message);
  }
shout();

--->  O/P: Up here!

      Value of message variable is 'Up here!' and console.log is printing value of message variable when function shout() is being called.


3.
var message = "Up here!";
function shout(message) {
  console.log(message);
}
shout("Down below!")

---> O/P: Down below!

          Value of message variable is 'Up here!' at the declaration section but when function shout() is being called it already have 'message' parameter value as 'Down below!' so console.log is printing value of message variable of function shout(parameter value)


4.
var muffins = 'two dozen';
var purchasedMuffins;

function getMuffins() {
  return muffins;
}
purchasedMuffins = getMuffins();
console.log(purchasedMuffins);

---> O/P: Two dozen

          getMuffins function returns the value of muffins as 'two dozen' and stored that returned value into purchasedMuffins variable and console.log prints the value of purchasedMuffins.


5.
var chore = 'laundry';

function doChores() {
  var chore = 'sneak out';
  function reportActivity() {
    console.log(chore);
  }
  reportActivity();
}

doChores(); // calling doChores(), which then calls reportActivity()

---> O/P: Sneak out

          value of chore variable is 'laundry' at the declaration but doChores function and nested reportActivity function returns its local variable value.


6.
var letter;
var contents = 'Looking for gold';

function getMail() {
  function changeContents() {
    var contents = 'Struck it rich!';
  }
  changeContents();
  return contents;
}

letter = getMail();
console.log(letter);

---> O/P: Looking for gold

          value of contents variable is 'Looking for gold' and letter has no value at the declaration but getMail function and nested changeContents function returns new value local to that function and the variable contents set at declaration remains unchanged.


7.
var decision;

function firstIdea() {
  var decision = 'Buy a new car';
  return decision;
}
function secondIdea() {
  console.log(decision);
}

firstIdea();
secondIdea();

---> O/P: undefined

          decision variable has no value at declaration so function firstIdea returns nothing and secondIdea function does not have anything to return so it prints the undefined variable decision to the screen
