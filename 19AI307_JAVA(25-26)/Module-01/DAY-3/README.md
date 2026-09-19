# Ex.No:1(C) LOOPING STATEMENT

## QUESTION:
Write a Java program that prompts the user to enter a non-negative integer and then calculates and displays the factorial of the given number.

- Use a for loop to perform the calculation.

- Make sure to handle the case when the user enters 0.

- Display the result in a clear and user-friendly way.

## AIM:
To write a java program to calculate and display the factorial of the given number.

## ALGORITHM :
- Start the program and prompt the user to enter a non-negative integer n.
- Read the integer n.
- Check if n < 0.
- If true, display an error message for invalid input.
- If n = 0 or n = 1, set the result/factorial to 1.
- If n > 1, initialize fact = 1 and loop i from 1 to n, multiplying fact by i in each iteration.
- Print the resulting factorial value.
- End the program.

## PROGRAM:
 ```
Program to implement a Looping Statement using Java
Developed by: MITHUN KUMAR G
Register Number:  212224230160
```

## SOURCE CODE:


```java
import java.util.Scanner;
public class Main{
    public static void main(String args[]){
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        int fact=1;
        if(n==0){
            System.out.println("Factorial of 0 is: "+fact);
        }
        else{
            for(int i=1;i<=n;i++){
                fact=fact*i;
            }
            System.out.println("Factorial of "+n+" is: "+fact);
        }
    }
}
```




## OUTPUT:

<img width="796" height="338" alt="image" src="https://github.com/user-attachments/assets/524c0133-a9fb-43c0-84d0-f6a28bd09283" />


## RESULT:
Therefore, the program successfully reads a number from the user and computes its factorial.
