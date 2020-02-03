### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.
```javascript
const whatToDoForLunch = function(hungry, availableTime) {
  if (hungry === false) {
    console.log("Wait until you're hungry, only then will you know.");
  } else if (hungry === true && availableTime < 20) {
    console.log("Pick something up and eat it in the office. Get to know your cohort!");
  } else if (hungry === true && (availableTime >= 20 && availableTime < 30)) {
    console.log("You deserve a break. Go check out somewhere in Gastown!");
  } else if (hungry === true && availableTime > 30) {
    console.log("A " + availableTime + " minute break? You know this is bootcamp... right?");
  } else
    console.log("I don't know what to do!");
};
```