# udacity-lesson-14
All the answers of Quiz in lesson 14 Udacity.

Directions:
Declare a function called laugh() that returns "hahahahahahahahahaha!". Print the value returned from the laugh() function to the console.
SOLUTION :-

*
 * Programming Quiz: Laugh it Off 1 (5-1)
 */

// your code goes here
function laugh() {
    var message = "hahahahahahahahahaha!";
    return message ;
    
}

console.log(laugh());



Write a function called laugh() that takes one parameter, num that represents the number of "ha"s to return.

TIP: You might need a loop to solve this!

Here's an example of the output and how to call the function that you will write:

console.log(laugh(3));
Prints: "hahaha!"

solution :-
/*
 * Programming Quiz: Laugh it Off 2 (5-2)
 *
 * Write a function called `laugh` with a parameter named `num` that represents the number of "ha"s to return.
 *
 * Note:
 *  - make sure your the final character is an exclamation mark ("!")
 *  - make sure that your function produces the correct results when it is called multiple times
 */

function laugh(num) {
  var ha="";
  for (var i=0; i<num; i++) {
    ha = ha + "ha";
  }
  return ha + "!";
}

console.log(laugh(3));


Write an anonymous function expression that stores a function in a variable called "laugh" and outputs the number of "ha"s that you pass in as an argument.

laugh(3);
Returns: hahaha!

/*
 * Programming Quiz: Laugh (5-4)
 */

var laugh = function (laugh) {
    var catLaugh = "";
    for (var i = 0; i < laugh ; i++) {
        catLaugh += "ha" ;
    }
    return catLaugh + "!";
};

console.log(laugh(3));

Write a named function expression that stores the function in a variable called cry and returns "boohoo!". Don't forget to call the function using the variable name, not the function name:

cry();
Returns: boohoo!

/*
 * Programming Quiz: Cry (5-5)
 */

// your code goes here
/*
 * Programming Quiz: Cry (5-5)
 */

// your code goes here
var cry = function human (boohoo) {
    return "boohoo!"; };
console.log(cry());



Call the emotions() function so that it prints the output you see below, but instead of passing the laugh() function as an argument, pass an inline function expression instead.

emotions("happy", laugh(2)); // you can use your laugh function from the previous quizzes
Prints: "I am happy, haha!"

/*
 * Programming Quiz: Inline Functions (5-6)
 */

// don't change this code
function emotions(myString, myFunc) {
    console.log("I am " + myString + ", " + myFunc(2));
}
emotions("happy", function laugh(num) {
	var laughter = "";
    for (var i = 0; i < num; i++) {
      laughter += "ha";
    }
    return laughter + "!";
});

// your code goes here
// call the emotions function here and pass in an
// inline function expression

