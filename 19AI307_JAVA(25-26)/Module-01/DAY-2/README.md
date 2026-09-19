# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION:
- A pirate ship has a code lock that only opens if:
-   The input code is even, and
-      If it is less than 100, say "Weak Code".
-      If it is between 100 and 999, say "Strong Code".
-   If the code is odd, deny access -"Access Denied".

## AIM:
To write a Java program that accepts a code number and determines the security level based on the given conditions:

- If the code is even and less than 100 → Display "Weak Code"
- If the code is even and between 100 and 999 → Display "Strong Code"
- Otherwise → Display "Access Denied"

## ALGORITHM :
- Start the program.
- Create a Scanner object to read input from the user.
- Read an integer value from the user and store it in variable 'code'.
- Check if 'code' is even (code % 2 == 0): a. If 'code' is less than 100: - Print "Weak Code". b. Else if 'code' is between 100 and 999 (inclusive): - Print "Strong Code". c. Else: - Print "Access Denied".
- If 'code' is odd: Print "Access Denied".
- End the program.

## PROGRAM:
 ```
Program to implement a conditional statement using Java
Developed by: MITHUN KUMAR G
Register Number:  212224230160
```

## SOURCE CODE:


```java
import java.util.Scanner;
public class Main{
    public static void main(String args[]){
        Scanner sc=new Scanner(System.in);
        int num=sc.nextInt();
        if(num%2==0){
            if(num<100){
                System.out.println("Weak Code");
            }
            else if(num>=100 & num<=999){
                System.out.println("Strong Code");
            }
            else{
                System.out.println("Access Denied");
            }
        }
        else{
            System.out.println("Access Denied");
        }
        
    }
}
```


## OUTPUT:
<img width="919" height="396" alt="image" src="https://github.com/user-attachments/assets/ccc0b281-ac3a-4018-81c7-536c9e6db51f" />



## RESULT:
Therefore,the program has been executed successfully.
