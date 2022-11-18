### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

```Javascript code
const whatToDoForLunch = function(hungry, availableTime) {
  let output = ``;
  if (hungry === true) {
    output += `I am hungry and I have ${availableTime} minutes for lunch.`;
  } else {
    output += `I am not hungry and I have ${availableTime} minutes for lunch.`;
  }
  console.log(output);
  output = ""; // resetting the output value to use on new availableTime conditionals
  if (availableTime > 30) {
    output +=
      "This is an intense program after all and I should probably reconsider.";
  } else if (availableTime >= 20 || availableTime <= 30) {
    output += "I deserve a break and should take time to cook a tasty meal.";
  } else {
    output += "Pick up a snack or grab something I have ready at home";
  }
  console.log(output + "\n");
};
```
