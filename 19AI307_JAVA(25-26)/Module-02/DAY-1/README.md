# Ex.No:2(A) CLASS AND OBJECT
## QUESTION:
Define a class Teacher with attributes: name (String), subject (String), and experience (int, years). 

## AIM:
To define a class Teacher with attributes

## ALGORITHM :
1.	Start the program.
2.	Read the teacher’s name, subject, and years of experience from the user.
3.	Create an object of the Teacher class.
4.	Assign the input values to the object's variables (name, subject, experience).
5.	Invoke the printMessage() method of the object.


## PROGRAM:
 ```
/*
Program to implement a Class and Objects using Java
Developed by: JEYA KRISHNA SJ
RegisterNumber:  212222040064
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class Teacher {
    String name;
    String subject;
    int experience;

    void printMessage() {
        System.out.println("Mr. " + name + " teaches " + subject + " and has " + experience + " years experience.");
    }
}

class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String name = sc.nextLine();
        String subject = sc.nextLine();
        int experience = sc.nextInt();
        Teacher t = new Teacher();
        t.name = name;
        t.subject = subject;
        t.experience = experience;
        t.printMessage();
    }
}
```

## OUTPUT:
<img width="1219" height="434" alt="Screenshot 2025-11-22 205253" src="https://github.com/user-attachments/assets/d116727e-4ba2-45f0-82e6-162876863e96" />



## RESULT:
Program to implement a Class and Objects using Java is executed

