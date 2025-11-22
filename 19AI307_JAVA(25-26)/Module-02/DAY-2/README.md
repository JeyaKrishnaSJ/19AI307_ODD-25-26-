# Ex.No:2(B) METHODS

## QUESTION:
Write a method int cube(int x) that calls a method int square(int x) internally to calculate the cube as x * square(x).

## AIM:
To write a method that calls a method internally to calculate the cube.



## ALGORITHM :
1.	Start the program.
2.	Start the program and read an integer input n from the user.
3.	Create an object of the Calc class.
4.	Call the cube() method using the object and pass n as the argument.
5.	Inside cube(), compute the cube using x * square(x) where square(x) returns x*x.

## PROGRAM:
 ```
/*
Program to implement a Methods using Java
Developed by: JEYA KRISHNA SJ
RegisterNumber:  212222040064
*/
```

## SOURCE CODE:
```
import java.util.*;
public class Calc{
    public int square(int x){
        return x*x;
    }
    public int cube(int x){
        return x*(square(x));
    }
    public static void main(String[] arg){
        Scanner scan=new Scanner(System.in);
        Calc obj=new Calc();
        int n=scan.nextInt();
        int res=obj.cube(n);
        System.out.print(res);
        
    }
}
```


## OUTPUT:
<img width="489" height="264" alt="Screenshot 2025-11-22 205808" src="https://github.com/user-attachments/assets/2b326a30-8960-4dfd-bf1e-dce753eee564" />



## RESULT:
Program to implement a Methods using Java is executed
