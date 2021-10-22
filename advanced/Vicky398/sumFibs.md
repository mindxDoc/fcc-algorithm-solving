//Sum of all odd fibonacci number

/*
We'll pass you a number as an argument to the function. 
return the sum of all odd Fibonacci numbers that are less than or equal to number.

For example, sumFibs(10) should return 10 because all odd Fibonacci numbers less than or equal to 10 are 1, 1, 3, and 5.
*/



function sumFibs(num) {
   let prevNumber = 0;
  let currNumber = 1;
  let result = 0;
  while (currNumber <= num) {
    if (currNumber % 2 !== 0) {
      result += currNumber;
    }
    currNumber += prevNumber;
    prevNumber = currNumber - prevNumber;
  }

  return result;
}

sumFibs(4);