# Test-Vagrant-Manasa
# ManasaTestVagrant
import java.util.*;
import java.io.*;

class Expenses{
  public static void main(String args[]){
    Scanner sc=new Scanner(System.in);
    //array for subscriptions
    String[] subArray = new String[]{"TOI","BM","HT","Hindu"}; 
    System.out.println("Enter the prices  of subscriptions");
    int price=sc.nextInt();
    
    if(price==40){
      System.out.print(subArray[0]);
      System.out.println(","+subArray[1]);
     }
     else if(price==50){
       System.out.println(subArray[1]);
       System.out.println(","+subArray[2]);
       }
      else if(price==80){
        System.out.println(subArray[2]);
        System.out.println(","+subArray[3]);
       }
      }
   }
      
