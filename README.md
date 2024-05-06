# Amazing Numbers

Java Project @JetBrains Academy

A program focusing on analyzing and categorizing numbers based on various mathematical properties. allows users to explore a wide range of unique and interesting properties of numbers, offering insights into their characteristics.

The application can identify the following properties of a given number:

- Even Numbers: Divisible by 2.
- Odd Numbers: Not divisible by 2.
- Buzz Numbers: Divisible by 7 or ending in 7.
- Duck Numbers: Contain at least one '0' in their decimal representation.
- Palindromic Numbers: The number is the same when read forwards and backwards.
- Gapful Numbers: Divisible by the number formed by its first and last digits.
- Spy Numbers: The sum of its digits equals the product of its digits.
- Sunny Numbers: The number n such that n+1 is a perfect square.
- Square Numbers: A number that is the square of an integer.
- Jumping Numbers: Digits of the number differ by 1 when compared with adjacent digits.
- Happy Numbers: A number that eventually equals 1 when replaced by the sum of the squares of its digits repeatedly.
- Sad Numbers: A number that does not converge to 1 using the same process as Happy Numbers.

## Prerequisites

This program requires Java to compile and run.

## Installation

- Download this repository and unzip the .zip file in your desired location.
- Open a terminal, then navigate to the project root.
- Compile the program using the command ```javac "Amazing Numbers\task\src\numbers\Main.java"```.
- Run the program using the command ```java -cp "Amazing Numbers\task\src" numbers.Main```.

## Example of use

- Input: The user inputs a number to analyze.
- Output: The program outputs the number's properties, indicating which of the above it meets.
- Multiple Checks: Users can check multiple numbers in a single run and get results for each property.

The symbol > represents the user input. Notice that it's not the part of the input.

```
> java -cp "Amazing Numbers\task\src" numbers.Main
Welcome to Amazing Numbers!
Supported requests:
- enter a natural number to know its properties;
- enter two natural numbers to obtain the properties of the list:
  * the first parameter represents a starting number;
  * the second parameter shows how many consecutive numbers are to be printed;
- two natural numbers and a property to search for;
- two natural numbers and properties to search for;
- a property preceded by minus must not be present in numbers;
- separate the parameters with one space;
- enter 0 to exit.

Enter a request: > 51 5 even sunny happy -duck 

       3,968 is even, happy, sunny
      15,624 is buzz, even, gapful, happy, sunny
      34,224 is even, happy, sunny
      75,624 is even, happy, sunny
     117,648 is even, gapful, happy, sunny


```


```

Enter a request: > 879654 5 sad

     879,654 is even, sad
     879,657 is buzz, gapful, odd, sad
     879,659 is odd, sad
     879,660 is duck, even, sad
     879,661 is odd, sad

```