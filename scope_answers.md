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
