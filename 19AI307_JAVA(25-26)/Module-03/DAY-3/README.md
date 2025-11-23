# Ex.No:3(C) ABSTRACTION

## QUESTION:
Create abstract class GameScore with method finalScore().
Subclasses:
ArcadeGame: score = baseScore + (level × 100)
PuzzleGame: score = (attempts ≤ 3) ? 1000 - (attempts × 100) : 500

## AIM:
To Program to implement a Abstraction using Java 

## ALGORITHM :
1.	Start the program.
2.	Based on the choice, read the required inputs.
3.	Create the appropriate object that extends the abstract class GameScore.
4.	Call the overridden finalScore() method of the selected game object to compute the score.
5.	Display the computed final score to the user.

## PROGRAM:
 ```
/*
Program to implement a Abstraction using Java
Developed by: JEYA KRISHNA SJ
RegisterNumber:  212222040064
*/
```

## SOURCE CODE:
```
import java.util.Scanner;
abstract class GameScore {
    abstract int finalScore();
}
class ArcadeGame extends GameScore {
    private int baseScore;
    private int level;

    ArcadeGame(int baseScore, int level) {
        this.baseScore = baseScore;
        this.level = level;
    }

    @Override
    int finalScore() {
        return baseScore + (level * 100);
    }
}
class PuzzleGame extends GameScore {
    private int attempts;

    PuzzleGame(int attempts) {
        this.attempts = attempts;
    }

    @Override
    int finalScore() {
        if (attempts <= 3)
            return 1000 - (attempts * 100);
        else
            return 500;
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int choice = sc.nextInt();

        GameScore game;

        if (choice == 1) { 
            int base = sc.nextInt();
            int level = sc.nextInt();
            game = new ArcadeGame(base, level);
        } else if (choice == 2) { 
            int attempts = sc.nextInt();
            game = new PuzzleGame(attempts);
        } else {
            return;
        }

        System.out.println(game.finalScore());
    }
}
```


## OUTPUT:
<img width="647" height="218" alt="Screenshot 2025-11-23 090955" src="https://github.com/user-attachments/assets/b98714ad-ddbe-48be-ac98-f3ed64fac6ea" />

## RESULT:
Program to implement a Abstraction using Java is executed
