
## QUESTION:
Write a Java program that calculates the area of different shapes using method overloading. Create a class AreaCalculator with:
area(int side) for square
area(int length, int breadth) for rectangle
area(double radius) for circle

## AIM:
To write a Java program that calculates the area of different shapes using method overloading.

## ALGORITHM :
1.	Start the program.
2.	Read the inputs from the user:side, length, breadth, and radius.
3.	Create an object of the AreaCalculator class.
4.	Call the overloaded area(int side) method to compute and display the area of a square.
5.	Call the overloaded area(int length, int breadth) method to compute and display the area of a rectangle.
6.	Call the overloaded area(double radius) method to compute and display the area of a circle using the formula πr².

## PROGRAM:
 ```
/*
Program to implement a Polymorphism using Java
Developed by: 
RegisterNumber:  
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class AreaCalculator {

    void area(int side) {
        System.out.println("Area of square: " + (side * side));
    }
    void area(int length, int breadth) {
        System.out.println("Area of rectangle: " + (length * breadth));
    }

    void area(double radius) {
        System.out.println("Area of circle: " + (Math.PI * radius * radius));
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        AreaCalculator calc = new AreaCalculator();

        int side = sc.nextInt();             
        int length = sc.nextInt();           
        int breadth = sc.nextInt();
        double radius = sc.nextDouble();

        calc.area(side);
        calc.area(length, breadth);
        calc.area(radius);

        sc.close();
    }
}


```


## OUTPUT:
<img width="1080" height="401" alt="image" src="https://github.com/user-attachments/assets/b60d691a-0c9d-4b48-abf7-afba9672bf74" />



## RESULT:

Program to implement a Polymorphism using Java is executed
