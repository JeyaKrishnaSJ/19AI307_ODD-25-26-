# Ex.No:1(E) STRINGS AND MATH FUNCTION

## QUESTION:
Write a java program to find the index of the last occurrence of a character in a string.

## AIM:
To write a java program to find the index of the last occurrence of a character in a string.

## ALGORITHM :
1.	Start the program.
2.	Initialize an index variable to store the last found position (default −1).
3.	Traverse the string from the beginning to the end, checking each character.
4.	If the current character matches the given character, update the index variable with the current position.
5.	After the traversal, if the index is not −1, display the last occurrence position; otherwise, print “Not found”.
   
## PROGRAM:
 ```
/*
Program to implement a Strings and Math Function using Java
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
        String str=scan.next();
        char ch=scan.next().charAt(0);
        int index=str.lastIndexOf(ch);
        
        if(index!=-1){
            System.out.print("Last occurrence of '"+ch+"' is at index: "+index);
        }
        else{
            System.out.print("Not found");
        }
    }
}
```


## OUTPUT:

<img width="1103" height="329" alt="Screenshot 2025-11-21 103742" src="https://github.com/user-attachments/assets/f74017ec-2be8-4fd9-92af-8491bfac3d23" />

## RESULT:
Program to implement a Strings and Math Function using Java is executed
