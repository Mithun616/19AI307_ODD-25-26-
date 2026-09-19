# Ex.No:1(E) STRINGS AND MATH FUNCTION

## QUESTION:
Write a Java program to calculate the power of a given number.

## AIM:
To write a java program to calculate the power of a given number.

## ALGORITHM :
- Start the program.

- Import the necessary packages (java.util.Scanner and java.lang.Math).

- Create a Scanner object to accept input from the user.

- Read two numerical values, n (base) and m (exponent), from the user using sc.nextInt().

- Calculate the power using the predefined function Math.pow(n, m) and store the result in the variable pow.

- Print the calculated power using formatted output (System.printf).

- Stop the program.



## PROGRAM:
 ```
Program to implement a Strings and Math Function using Java
Developed by: MITHUN KUMAR G
RegisterNumber: 212224230160
```

## SOURCE CODE:

```java
import java.util.Scanner;
import java.lang.Math;
public class Main{
    public static void main(String args[]){
        Scanner sc=new Scanner(System.in);
        double n=sc.nextInt();
        double m=sc.nextInt();
        double pow=Math.pow(n,m);
        System.out.printf(n+" raised to the power of "+m+" is: "+pow);
    }
}
```





## OUTPUT:

<img width="970" height="340" alt="image" src="https://github.com/user-attachments/assets/6a12f552-19ef-4aab-af71-19801c15e3d1" />


## RESULT:
Therefore the program successfully reads a number and calculates the power of a given number.
