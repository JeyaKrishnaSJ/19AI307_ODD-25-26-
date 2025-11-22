# Ex.No:2(C) ACCESS SPECIFIERS

## QUESTION:
Write a Java program to create a class called Person with private instance variables name, age. and country. Provide public getter and setter methods to access and modify these variables.

## AIM:
To write a Java program to create a class called Person with private instance variables. Provide public getter and setter methods to access and modify these variables.

## ALGORITHM :
1.	Start the program.
2.	Read the name, age, and country from the user using Scanner.
3.	Store these values in the object using setName(), setAge(), and setCountry().
4.	Retrieve the stored values using getName(), getAge(), and getCountry().
5.	Display the person's details in the required format.

## PROGRAM:
 ```
/*
Program to implement a Access Specifiers using Java
Developed by: JEYA KRISHNA SJ
RegisterNumber:  212222040064
*/
```

## SOURCE CODE:
```
import java.util.*;
public class Person {
    private String name;
    private int age;
    private String country;
    public String getName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }
    public int getAge() {
        return age;
    }
    public void setAge(int age) {
        this.age = age;
    }
    public String getCountry() {
        return country;
    }
    public void setCountry(String country) {
        this.country = country;
    }
    public static void main(String[] arg){
            Scanner sc=new Scanner(System.in);
            Person per=new Person();
            String name=sc.nextLine();
            per.setName(name);
            
            int age=sc.nextInt();
            sc.nextLine();
            
            per.setAge(age);
            String country=sc.nextLine();
            per.setCountry(country);
            System.out.println("Person 1");
            System.out.println("Name: "+per.getName());
            System.out.println("Age: "+per.getAge());
            System.out.println("Country: "+per.getCountry());
        }
    }

```

## OUTPUT:
<img width="867" height="475" alt="Screenshot 2025-11-22 210548" src="https://github.com/user-attachments/assets/32fd1a78-f407-4dd1-8ecb-c07850d7cbf3" />



## RESULT:
Program to implement a Access Specifiers using Java is executed

