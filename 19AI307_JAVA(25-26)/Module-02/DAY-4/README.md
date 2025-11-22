# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION:
Write a class that uses a constructor to initialize variables and overrides toString() method.

## AIM:
To write a class that uses a constructor to initialize variables and overrides toString() method.

## ALGORITHM :
1.	Start the program.
2.	Create a Student object using the parameterized constructor.
3.	Inside the constructor, initialize the object's fields name and age.
4.	When printing the object, automatically call the overridden toString() method.
5.	Display the output in the format

## PROGRAM:
 ```
/*
Program to implement a Variable scope and Constructor using Java
Developed by: 
RegisterNumber:  
*/
```

## SOURCE CODE:
```
import java.util.*;
public class Student{
    private String name;
    private int age;
    
    public Student(String name,int age){
        this.name=name;
        this.age=age;
    }
    
    @Override
    public String toString(){
        return "Student{name='" +name+ "', age="+ age + "}";
    }
    public static void main(String[] arg){
        Scanner sc=new Scanner(System.in);
        String name=sc.nextLine();
        int age=sc.nextInt();
        
        Student s=new Student(name,age);
        System.out.print(s);
    }
}
```


## OUTPUT:

<img width="875" height="404" alt="Screenshot 2025-11-22 211624" src="https://github.com/user-attachments/assets/e82b4a27-f85c-46d8-96a5-36361d8b4bb2" />


## RESULT:
Program to implement a Variable scope and Constructor using Java is executed
