# Ex.No:5(C)  FILE HANDLING USING JAVA
## QUESTION:

Write a Java program to create a new file named example.txt.


## AIM:

To write a Java program that creates a new file named example.txt using the File class and handles any possible I/O exceptions.


## ALGORITHM :

Create a File object pointing to "example.txt".

Call the createNewFile() method to attempt creating the file.

If the method returns true, print that the file was created.

If it returns false, print that the file already exists.

Surround the file-creation logic with a try–catch block to handle IOException



## PROGRAM:
 ```
/*
Program to implement a File Handling using Java
Developed by: MITHUN KUMAR G
RegisterNumber: 212224230160
*/
```

## SOURCE CODE:


    import java.io.File;
    import java.io.IOException;
    
    public class CreateNewFileExample {
        public static void main(String[] args) {
            try {
                File file = new File("example.txt");
                if (file.createNewFile()) {
                    System.out.println("File created: " + file.getName());
                } else {
                    System.out.println("File already exists.");
                }
            } catch (IOException e) {
                System.out.println("An error occurred: " + e.getMessage());
            }
        }
    }




## OUTPUT:

<img width="735" height="206" alt="image" src="https://github.com/user-attachments/assets/8994030d-3d7a-4a19-b9a2-9a9478bdd0ec" />


## RESULT:
Therefore the program successfully creates a new file named example.txt if it does not already exist.

