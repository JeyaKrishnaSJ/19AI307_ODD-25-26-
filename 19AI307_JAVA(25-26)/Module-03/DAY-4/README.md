# Ex.No:3(D)    INTERFACE 

## QUESTION:
You are programming bots that analyze weather data. Each bot must implement a common interface and give a prediction.
SunBot: Predicts "HOT" if temperature > 30, else "MODERATE".
RainBot: Predicts "COLD" if temperature < 20, else "WARM".

## AIM:
To implement a Interface using Java


## ALGORITHM :
1.	Start the program.
2.	Based on the bot type, create an object of SunBot or RainBot, both implementing the WeatherBot interface.
3.	Call the predict(temperature) method on the selected bot object.
4.	Inside predict(), apply the respective temperature rules and return the weather condition.
5.	Display the predicted weather condition to the user.

## PROGRAM:
 ```
/*
Program to implement a Interface using Java
Developed by: JEYA KRISHNA SJ
RegisterNumber:  212222040064
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

interface WeatherBot {
    String predict(int temperature);
}

class SunBot implements WeatherBot {
    public String predict(int temperature) {
        if (temperature > 30)
            return "HOT";
        else
            return "MODERATE";
    }
}

class RainBot implements WeatherBot {
    public String predict(int temperature) {
        if (temperature < 20)
            return "COLD";
        else
            return "WARM";
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int temperature = sc.nextInt();
        int botType = sc.nextInt();

        WeatherBot bot;

        if (botType == 1)
            bot = new SunBot();
        else if (botType == 2)
            bot = new RainBot();
        else {
            System.out.println("Invalid bot type!");
            sc.close();
            return;
        }

        System.out.println(bot.predict(temperature));

    }
}
```

## OUTPUT:
<img width="653" height="180" alt="image" src="https://github.com/user-attachments/assets/45a07a90-57e8-4405-a2d9-32ed3f56cd95" />



## RESULT:
Program to implement a Interface using Java is executed
