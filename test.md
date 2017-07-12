var lastWord = 'welcome';
console.log(lastWord);
lastWord = 'goodbye';



var message = "Up here!";
  function shout() {
    console.log(message);
  }
shout();



var message = "Up here!";
function shout(message) {
  console.log(message);
}
shout("Down below!")



var muffins = 'two dozen';
var purchasedMuffins;

function getMuffins() {
  return muffins;
}
purchasedMuffins = getMuffins();
console.log(purchasedMuffins);
