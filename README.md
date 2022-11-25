# 4.23-Find-the-Two-Largest-Numbers-Using-an-approach-similar-to-that-for-Exercise-4.21-find-the-tw
4.23 (Find the Two Largest Numbers) Using an approach similar to that for Exercise 4.21, find the two largest values of the 10 values entered. [Note: You may input each number only once.]

import java.util.Scanner;

public class Main {
    public static void main(String[] args){
    
        Scanner console = new Scanner(System.in);
        int counter =0;
        int num;
        int Largest = 0;
        int Largest1=0;
   
        while (counter<10){
            num = console.nextInt();

            if(num>Largest){
                Largest1 = Largest;
                Largest=num;
            }
            if (num<Largest){
                if (num>Largest1){
                    //Largest2=Largest1;
                    Largest1=num;
                }
            }
            counter++;
        }
        System.out.println(Largest +" is 1st largest numbers: ");
        System.out.println(Largest1 +" is 2nd largest numbers: ");

    }
}
