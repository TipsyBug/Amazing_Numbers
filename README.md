# Amazing Numbers

Java Project @JetBrains Academy

This program focuses on analyzing and categorizing numbers based on various mathematical properties. It allows users to explore a wide range of unique and interesting characteristics of numbers, offering insights into their behavior.

The application can identify the following properties in a given number:

- Even Numbers: Divisible by 2.
- Odd Numbers: Not divisible by 2.
- Buzz Numbers: Divisible by 7 or ending in 7.
- Duck Numbers: Contains at least one '0' in its decimal representation.
- Palindromic Numbers: Reads the same forwards and backwards.
- Gapful Numbers: Divisible by the number formed by its first and last digits.
- Spy Numbers: The sum of its digits equals the product of its digits.
- Sunny Numbers: The number 𝑛 such that 𝑛 + 1 is a perfect square.
- Square Numbers: A number that is the square of an integer.
- Jumping Numbers: Each pair of adjacent digits differs by 1.
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

Enter a request: > 21012321012                     

Properties of 21,012,321,012
        buzz: false
        duck: true
        even: true
      gapful: false
       happy: false
     jumping: true
         odd: false
 palindromic: true
         sad: true
         spy: false
      square: false
       sunny: false
```
Get a list of numbers with their properties
```
Enter a request: > 21012321012 2

21,012,321,012 is duck, even, jumping, palindromic, sad
21,012,321,013 is duck, odd, sad
```
Find numbers with specific property
```
Enter a request: > 21012321012 2 spy

21,111,111,124 is even, happy, spy
21,111,111,142 is even, gapful, happy, spy
```
Find numbers with specific properties
```
Enter a request: > 21012321012 4 sunny odd        

21,012,821,763 is duck, odd, sad, sunny
21,013,401,599 is duck, happy, odd, sunny
21,013,981,443 is buzz, duck, odd, sad, sunny
21,014,561,295 is buzz, duck, odd, sad, sunny
```
Find numbers excluding specific properties
```
Enter a request: > 21012321012 4 sunny odd -sad

21,013,401,599 is duck, happy, odd, sunny
21,015,141,155 is duck, happy, odd, sunny
21,019,200,399 is duck, happy, odd, sunny
21,022,100,099 is buzz, duck, happy, odd, sunny
```
Error Handling                               
```                                                                  
Enter a request: > 21012321012 4 square sunny odd                    
                                                                     
The request contains mutually exclusive properties: sunny and square 
There are no numbers with these properties.                          
```                                                                  
Exit the program
```
Enter a request: > 0

Goodbye!
```