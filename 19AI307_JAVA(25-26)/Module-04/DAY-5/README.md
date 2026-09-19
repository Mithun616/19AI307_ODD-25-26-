# Ex.No:4(E) DESIGN PATTERN  ---- BEHAVIOUR PATTERN

## QUESTION:

Design a program where a Product model stores item info, and the view displays it. Implement a controller to update product price and refresh the view automatically.

## AIM:

To design and implement the Model-View-Controller (MVC) pattern in Java, where the Product model stores item information, the View displays the product details, and the Controller updates the product price and refreshes the View automatically.

## ALGORITHM :
Start the program.
Import the required java.util package.
Create the Product Model with name, price, and code.
Initialize the product details using a constructor.
Create getter and setter methods to access and update the product information.
Create the Product View to display the product details.
Create the Product Controller to connect the Model and View.
Implement updateView() to display the current product details.
Implement updatePrice() to change the price and refresh the View automatically.
Get the product details and new price from the user.
Create the Model, View, and Controller objects.
Display the initial product details.
Update the product price and refresh the View.
Stop the program.

## PROGRAM:
 ```
/*
Program to implement a Behaviour Pattern using Java
Developed by: MITHUN KUMAR G
RegisterNumber: 212224230160
*/
import java.util.Scanner;

public class ProductManagementSystem {

    // ===== Model =====
    static class Product {
        private String name;
        private double price;
        private String code;

        Product(String name, double price, String code) {
            this.name = name;
            this.price = price;
            this.code = code;
        }

        public String getName() {
            return name;
        }

        public double getPrice() {
            return price;
        }

        public String getCode() {
            return code;
        }

        public void setPrice(double price) {
            this.price = price;
        }
    }

    // ===== View =====
    static class ProductView {
        public void displayProduct(String name, double price, String code) {
            System.out.println("--- Product Details ---");
            System.out.println("Name : " + name);
            System.out.println("Price: " + price);
            System.out.println("Code : " + code);
        }
    }

    // ===== Controller =====
    static class ProductController {
        private Product product;
        private ProductView view;

        ProductController(Product product, ProductView view) {
            this.product = product;
            this.view = view;
        }

        public void updateView() {
            view.displayProduct(
                product.getName(),
                product.getPrice(),
                product.getCode()
            );
        }

        public void updatePrice(double newPrice) {
            product.setPrice(newPrice);
            updateView();
        }
    }

    // ===== Main Method =====
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        String name = sc.nextLine();
        double price = sc.nextDouble();
        sc.nextLine();
        String code = sc.nextLine();
        double newPrice = sc.nextDouble();

        Product product = new Product(name, price, code);
        ProductView view = new ProductView();
        ProductController controller = new ProductController(product, view);

        controller.updateView();
        controller.updatePrice(newPrice);

        sc.close();
    }
}
```

## OUTPUT:

<img width="561" height="294" alt="image" src="https://github.com/user-attachments/assets/0100780f-a3ee-4db0-96a2-3ce000e26a9a" />

## RESULT:

Thus, the MVC (Model-View-Controller) design pattern was successfully implemented in Java. The Product model stores item information, the View displays the details, and the Controller updates the product price and automatically refreshes the View.
