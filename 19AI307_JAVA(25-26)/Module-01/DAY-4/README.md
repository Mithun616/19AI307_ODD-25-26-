# Ex.No:1(D) ARRAYS

## QUESTION:
Write a Java program to reverse an array

## AIM:
To write a java program to reverse an array

## ALGORITHM :
- Start the program.

- Import the java.util.Scanner package.

- Read the integer n representing the size of the array from the user.

- Declare an integer array arr of size n.

- Loop through 0 to n - 1 to accept and store n array elements.

- Loop backwards from n - 1 down to 0 and print each element of the array.

- Stop the program.





## PROGRAM:
 ```
Program to implement a Array concept using Java
Developed by: MITHUN KUMAR G
Register Number: 212224230160
```

## SOURCE CODE:

```java
import java.util.Scanner;
public class Main{
    public static void main(String args[]){
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        int[] arr=new int[n];
        float sum=0;
        for(int i=0;i<n;i++){
            arr[i]=sc.nextInt();
        }
        for(int i=n-1;i>=0;i--){
            System.out.print(arr[i]+" ");
        }
    }
}
```

## OUTPUT:
<img width="721" height="639" alt="image" src="https://github.com/user-attachments/assets/33087eb3-ac3f-4c43-9e9c-a783664e58b1" />


## RESULT:
Therefore the program successfully reverse an array.
