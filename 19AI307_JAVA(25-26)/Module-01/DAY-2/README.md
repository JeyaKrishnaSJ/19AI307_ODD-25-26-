# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION:
A dragon wakes based on temperature:
If temperature < 0, it hibernates.
If 0 ≤ temp ≤ 20, it snoozes.
If 21 ≤ temp ≤ 35, it wakes.
If temp > 35, it gets angry.
Write a java program to get the user input for temperature and display appropriate output.

## AIM:
To write a java program to get the user input for temperature and display appropriate output.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Identify the first condition to check
4.	If the first condition is false, move to the next condition and evaluate it
5.	Continue checking conditions one by one, and when a condition becomes true, select the corresponding action
6.	End the program

## PROGRAM:
 ```
/*
Program to get the user input for temperature and display appropriate output using Java
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
        int t=scan.nextInt();
        if(t<0){
            System.out.print("Hibernating");
        }
        else if((t>=0) && (t<=20)){
                    System.out.print("Snoozing");
        } 
        else if((t>=21) && (t<=35)){
                    System.out.print("Awake"); 
        }
        else if(t>35){
                    System.out.print("Angry"); 
        }
    }
} 
```
## OUTPUT:
<img width="890" height="369" alt="Screenshot 2025-11-21 102213" src="https://github.com/user-attachments/assets/85e35b9b-b421-4b8d-a738-3995ab8c3940" />



## RESULT:
Program to get the user input for temperature and display appropriate output using Java is executed
