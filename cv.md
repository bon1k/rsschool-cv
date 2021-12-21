# **Gorshkov Mikhail**
## Contact info  
### Tel +7 965 841 1000  
### *mail: bon1k@bk.ru*

## About Me:
### A person who is trying to comprehend the profession of a programmer!

## Education:
* HTML and CSS Tutorials on the w3schools 
![htmlImg](.HTML.PNG "screen complete course html")
![CSSImg](.CSS.PNG "screen complete course CSS")
## Skills:
*Low Level
    + Python 
    +Java 2
    +JS 3
    +CSS3 4
    +HTML5 5
    +Git, Github 6

*High Level
    - teamwork
    - ability to learn

## Languages:
1. Russian
2. English (A1 level)

## Examples of my code
```
package ru.epam.izh.mikhail;

import java.io.BufferedReader;
import java.io.IOException;
import java.io.InputStreamReader;
import java.util.Objects;

public class ViewConsole {


    public static void sayCount(int getCountMatches) {
        System.out.println("На столе осталось " + getCountMatches +" спичек");
    }

    public static void sayComp(int getPutComp) {
        System.out.println(" - Компьютер взял спичек = " + getPutComp);
    }

    public static int sayUser() {
        int stepUser = 0;
        System.out.print(" - Ваш ход. Введите кол-во спичек: ");
        BufferedReader bufferedReader = new BufferedReader(new InputStreamReader(System.in));
        try {

            stepUser = Integer.parseInt(bufferedReader.readLine());
            if (stepUser > 3 || stepUser < 1){
                System.out.println("Некорректный ввод, выберете от 1 до 3 спичек");
                sayUser();
            }

        } catch (IOException e) {
            e.printStackTrace();
        }
        return stepUser;
    }
    public static void sayWinner() {
        System.out.println("Для игрока осталась последняя спичка. Игрок проиграл");
    }
}
```