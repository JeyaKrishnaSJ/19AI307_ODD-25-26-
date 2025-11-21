# Ex.No:1(C) LOOPING STATEMENT

## QUESTION:
Check for Palindrome Number

## AIM:
To write a program to check for Palindrome Number

## ALGORITHM :
1.	Start the program.
2.	Start and read the number from the user.
3.	Store the original number in a separate variable and initialize a variable
4.	Repeat while the number is not zero: extract the last digit, add it to reverse, and remove the last digit from the number
5.	After the loop, compare the reversed number with the original number.
6.	If both are equal, output "Palindrome"; otherwise output "Not a Palindrome".

## PROGRAM:
 ```
/*
Program to implement a Looping Statement using Java
Developed by: JEYA KRISHNA SJ 
RegisterNumber:  212222040064
*/
```

## SOURCE CODE:
```
import java.util.*;
public class Main{
    public static void main(String[] arg){
        Scanner scan=new Scanner(System.in);
        int num=scan.nextInt();
        int reverse=0;
        int og=num;
        while(num!=0){
            int digi=num%10;
            reverse=reverse*10+digi;
            num=num/10;
        }
        if(og==reverse){
            System.out.print(og+" is a Palindrome.");
        }
        else{
            System.out.print(og+" is not a Palindrome.");
        }
    }
}
```

## OUTPUT:
<img width="1209" height="343" alt="Screenshot 2025-11-21 102650" src="https://github.com/user-attachments/assets/8bc56c62-5ecf-47a9-84fd-5097b1804980" />


## RESULT:
Program to implement a Looping Statement using Java is executed
