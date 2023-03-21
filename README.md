# Oasis-Game
import java.lang.Math;
import java.util.Random;
import java.util.*;
public class Game{
public static void main(String[] args){
int ch=1;
int c=1;
Scanner sc=new Scanner(System.in);
while(ch>0){
c=1;
System.out.println("Enter low limit value:");
int min=sc.nextInt();
System.out.println("Enter high limit value:");
int max=sc.nextInt();
int R=(int)(Math.random()*(max-min)+min);
System.out.println("Enter positive number:");
int N=sc.nextInt();
while(N!=R)
{
c++;
if(N<R){
System.out.println( "   "+N+"    "+"is smaller");}
if(N>R){
System.out.println( "   "+N+"    "+"is greater");}
System.out.println( "Enter another num: ");
N=sc.nextInt();
}
System.out.println( "\n");
if(c==1)
System.out.println( "     * * * * * \n Congrats!!!");
else if(c==2)
System.out.println( "     * * *  \n Congrats!!!");
else if(c==3)
System.out.println( "     * \n Congrats!!!");
else
System.out.println("     Won");
System.out.println("You guessed the number in  "  +c+"  chances");
System.out.println("Do you want to continue!!!");
System.out.println("If yes enter a positive number. \n Else enter a negative number.");
ch=sc.nextInt();
}
}
}


