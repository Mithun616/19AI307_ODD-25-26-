# Ex.No:5(D) THREAD PRIORITY

## QUESTION:

Write a Java program to implement a extending thread class


## AIM:

To write a Java program that demonstrates multithreading by creating a user-defined thread class that extends Thread and executes its own run() method.


## ALGORITHM :

Create a class MyThread that extends the Thread class.

Override the run() method to print numbers from 1 to 5.

In the main() method: Print a message indicating the main thread execution.

Create an instance of MyThread.

Call the start() method to begin execution in a separate thread.

Allow the thread to run independently from the main thread.



## PROGRAM:
 ```
/*
Program to implement a Thread Priority Concept using Java
Developed by: MITHUN KUMAR G
RegisterNumber: 212224230160
*/
```

## SOURCE CODE:

    
    public class MyThread extends Thread {
        public void run() {
            for (int i = 1; i <= 5; i++) {
                System.out.println("Thread: " + i);
            }
           
        }
    
        public static void main(String[] args) {
            System.out.println("Main thread finished");
            MyThread t = new MyThread();
            t.start();
        }
    }



## OUTPUT:

<img width="650" height="326" alt="image" src="https://github.com/user-attachments/assets/6b27cb65-42b3-4e0f-9015-3157ad58816c" />


## RESULT:
Therefore the program successfully creates a separate thread by extending Thread and executes the overridden run() method.

