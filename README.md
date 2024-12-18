# javascript2

Reverse a String: Write a function that reverses a given string.
function reverseString(str) {
    var splitStr = str.split("");
 console.log(splitStr);
 var revereStr = splitStr.reverse();
 console.log(revereStr);
 var joinStr = revereStr.join("")
 console.log(joinStr);
}
reverseString("Ayo");
reverseString("Hello");

Count Characters: Create a function that counts the number of characters in a string

function countChar(str) {
    var strLen = str.length;
    console.log(strLen);

}

countChar("hello");
countChar("My name is Ayomide");

Capitalize Words: Implement a function that capitalizes the first letter of each word in a sentence.

function capFirstChar(str) {
      var firstletterCap = str.charAt(0).toUpperCase();
      console.log(firstletterCap)
      var remainingletter = str.slice(1);
      console.log(remainingletter)
      var letters = firstletterCap + remainingletter;
      console.log(letters)
      return letters

}

capFirstChar("Michael");

Find Maximum and Minimum: Write functions to find the maximum and minimum values in an array of numbers.

const num1 = [8, 2, 14, 1, 28, 20]

function maxNum() {
    console.log (Math.max(...num1))
    return Math.max(...num1);
}

maxNum()

function minNum() {
    console.log (Math.min(...num1))
    return Math.min(...num1);
}

minNum()

Sum of Array: Create a function that calculates the sum of all elements in an array.

const num1 = [8, 2, 14, 1, 28, 20]

let sumNum = num1.reduce((total, currentValue) => total + currentValue)

console.log(sumNum);

Filter Array: Implement a function that filters out elements from an array based on a given condition.

const num1 = [8, 2, 14, 1, 28, 20]

let filteredNum = num1.filter((num)=> num >= 8)

console.log(filteredNum);

Factorial: Write a function to calculate the factorial of a given number.

function factorials(num) {
    let result = num;
    if (num === 0 || num === 1) {
        return 1
    }

    while( num > 1) {
        num--
        result*=num;
    }
}

factorials(5)

Prime Number Check: Create a function to check if a number is prime or not.
function checkPrime(num){
   for (let i = 2; i < num; i++){
     if(num % i === 0){
       }
     }
  }
  function detectPrime(arr){
      if (checkPrime){
          return true;
           }else{
             return false;
        }
}

Fibonacci Sequence: Implement a function to generate the Fibonacci sequence up to a given number of terms.

const number = Number(prompt('Enter the number of terms: '));
let n1 = 0, n2 = 1, nextTerm;

console.log('Fibonacci Series:');

for (let i = 1; i <= number; i++) {
    console.log(n1);
    nextTerm = n1 + n2;
    n1 = n2;
    n2 = nextTerm;
}



