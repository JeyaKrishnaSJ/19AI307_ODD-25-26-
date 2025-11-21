# Ex.No:1(A) INTRODUCTION TO JAVA PROGRAMMING, DATA TYPES, VARIABLES AND OPERATORS

## QUESTION:
Lovely found a magic machine that tells her how two numbers relate to each other.
The machine supports all 6 relational operators
Lovely enters two numbers. The machine prints the result (true or false) for each operator.

## AIM:
To prints the result (true or false) for each operator.

## ALGORITHM :
1.	Read two numbers A and B from the user.
2. Check A == B and store/record the boolean result.
3. Check A != B and store/record the boolean result.
4. Check A > B, A < B, A >= B, and A <= B and store each boolean result.
5. Print the six results labeled for ==, !=, >, <, >=, <= (each as true or false).
## PROGRAM:
 ```
/*
Program to prints the result (true or false) for each operator.
Developed by: JEYA KRISHNA SJ
RegisterNumber:  212222040064
*/
```

## Sourcecode.java:
```
import java.util.*;
public class Main{
    public static void main(String[] args){ 
        Scanner scan=new Scanner(System.in);
        int a=scan.nextInt();
        int b=scan.nextInt(); 
        
        System.out.println("a == b: "+(a==b));
        System.out.println("a != b: "+(a!=b)); 
        System.out.println("a > b: "+(a>b)); 
        System.out.println("a < b: "+(a<b)); 
         System.out.println("a >= b: "+(a>=b)); 
         System.out.println("a <= b: "+(a<=b)); 
    }
}
```

## OUTPUT:
<img width="1234" height="378" alt="Screenshot 2025-11-21 101253" src="https://github.com/user-attachments/assets/e9d20c6e-ecfa-4365-b700-0bd6c831fcea" />



## RESULT:
Program to prints the result (true or false) for each operator is executed
