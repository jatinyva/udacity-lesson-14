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
