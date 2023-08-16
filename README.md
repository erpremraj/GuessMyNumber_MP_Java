//GuessMyNumber_MP_Java
//Guess my number Mini Project Java
//package com.project; //my file but not required

import java.util.*;

public class GuessNoMP {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int userNumber = (int) (Math.random() * 100);
        int myNumber = 0;
        do {
            System.out.print("Guess my number : ");
            myNumber = sc.nextInt();
            if (myNumber == userNumber) {
                System.out.println("Yooohoo... You guessed it correctly!");

                break;
            } else if (myNumber > userNumber) {
                System.out.println("Your number is too large...");
            } else {
                System.out.println("Your number is too short...");
            }
        } while (myNumber >= 0);
        System.out.print("My number was : ");
        System.out.println(myNumber);
    }

}

