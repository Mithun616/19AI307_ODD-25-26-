# Ex.No:1(A) INTRODUCTION TO JAVA PROGRAMMING, DATA TYPES, VARIABLES AND OPERATORS

## QUESTION:
Lovely has mastered printing in Java, and now she wants to learn how arithmetic operators work. She’s curious about how Java can add, subtract, multiply, divide, and find remainders of two numbers.

Write a Java program that:

Accepts two integer numbers from the user.

Demonstrates all 5 arithmetic operations:

Addition (+)

Subtraction (-)

Multiplication (*)

Division (/)

Modulus (%)

Displays the result of each operation in a separate line with a clear message.

## AIM:
To write a Java program that reads two integer numbers from the user and performs basic arithmetic operations such as addition, subtraction, multiplication, division, and modulus, and displays the results.

## ALGORITHM :
- Start the program.
- Create an object of the Scanner class to take input from the user.
- Read the first integer input from the user and store it in variable num1.
- Read the second integer input from the user and store it in variable num2.
- Calculate the sum of num1 and num2, and display the result.
- Calculate the difference (num1 - num2), and display the result.
- Calculate the product of num1 and num2, and display the result.
- Calculate the quotient of num1 divided by num2, and display the result.
- Calculate the remainder of num1 divided by num2, and display the result.
- Close the Scanner object.


## PROGRAM:
 ```
Program to implement variables and Operators using Java
Developed by: MITHUN KUMAR G
RegisterNumber: 212224230160
```

## Sourcecode.java:

```java
import java.util.Scanner;
public class Main{
    public static void main(String args[]){
        Scanner sc=new Scanner(System.in);
        int number1=sc.nextInt();
        int number2=sc.nextInt();
        int sum=number1+number2;
        int Difference=number1-number2;
        int Product=number1*number2;
        int Quotient=number1/number2;
        int Remainder=number1%number2;
        System.out.println("Sum = "+sum);
        System.out.println("Difference = "+Difference);
        System.out.println("Product = "+Product);
        System.out.println("Quotient = "+Quotient);
        System.out.println("Remainder = "+Remainder);
    }
}
```


## OUTPUT:

<img width="942" height="357" alt="image" src="https://github.com/user-attachments/assets/53c65599-7d7d-48e6-af4d-4d76a5db3258" />


## RESULT:
Therefore the program has been executed successfully.
