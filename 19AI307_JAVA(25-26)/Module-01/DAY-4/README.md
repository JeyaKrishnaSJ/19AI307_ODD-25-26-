# Ex.No:1(D) ARRAYS

## QUESTION:
Write a Java program to check if an element is present more than once in an array

## AIM:
To write a program to check if an element is present more than once in an array


## ALGORITHM :
1.	Start the program.
2.	Start and read the value of n, then read n elements into an array.
3.	Sort the array so that any duplicate values become adjacent.
4.	Initialize a flag variable to 0 (indicating no duplicates found yet).
5.	Traverse the array from index 0 to n−2 and compare each element with the next one; if any pair is equal, set the flag to 1.
6.	If the flag is 1, print "Yes" (duplicates exist), otherwise print "No".

## PROGRAM:
 ```
/*
Program to implement a Array concept using Java
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
        int n=scan.nextInt();
        int[] arr=new int[n];
        for(int i=0;i<n;i++){
            arr[i]=scan.nextInt();
        }
        int flag=0;
        Arrays.sort(arr);
        for(int i=0;i<n-1;i++){
            if(arr[i]==arr[i+1]){
                flag=1;
            }
            }
            if(flag==1){
                System.out.print("Yes");
            }
            else{
                System.out.print("No");
            
        }
    }
}
```

## OUTPUT:
<img width="1396" height="733" alt="Screenshot 2025-11-21 103107" src="https://github.com/user-attachments/assets/1a06c69e-ace6-4a35-a203-0e11b40b0025" />



## RESULT:
Program to implement a Array concept using Java is executed.
