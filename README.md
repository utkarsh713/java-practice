   # java-practice.                                                     
                                                              
import java.util.Scanner;                                           
class EvenOdd                                    
{                                                        
                                      
   public static void main(String args[])        
    {           
        Scanner sc = new Scanner(System.in)     
        System.out.print("Enter a number: ");
        int num = sc.nextInt();  
        if(num % 2 == 0)
        {   
            System.out.println("Number is Even"); 
        }
        else 
        {
            System.out.println("Number is Odd");
        }
    } 

    
class Palindrome {
    public static void main(String[] args) {
        int n=121,r,sum=0,temp=n;
        while(n>0){
            r=n%10;
            sum=sum*10+r;
            n/=10;
        }
        System.out.println(temp==sum ? "Palindrome":"Not");
    }
}

Calculator

import java.util.Scanner;

class Calculator
{
    public static void main(String args[])
    {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter first number: ");
        int a = sc.nextInt();

        System.out.print("Enter second number: ");
        int b = sc.nextInt();

        System.out.println("1. Addition");
        System.out.println("2. Subtraction");
        System.out.println("3. Multiplication");
        System.out.println("4. Division");

        System.out.print("Enter your choice: ");
        int choice = sc.nextInt();

        switch(choice)
        {
            case 1:
                System.out.println("Sum = " + (a + b));
                break;

            case 2:
                System.out.println("Difference = " + (a - b));
                break;

            case 3:
                System.out.println("Product = " + (a * b));
                break;

            case 4:
                if(b != 0)
                    System.out.println("Quotient = " + (a / b));
                else
                    System.out.println("Division by zero not possible");
                break;

            default:
                System.out.println("Invalid Choice");
        }
    }
}


class Pattern
{
    public static void main(String args[])
    {
        for(int i = 9; i >= 1; i = i - 2)
        {
            for(int j = 1; j <= i; j++)
            {
                System.out.print("* ");
            }
            System.out.println();
        }
    }
}


import java.util.Scanner;

class Matrix
{
    public static void main(String args[])
    {
        Scanner sc = new Scanner(System.in);

        int a[][] = new int[2][2];

        for(int i=0;i<2;i++)
        {
            for(int j=0;j<2;j++)
            {
                a[i][j] = sc.nextInt();
            }
        }

        for(int i=0;i<2;i++)
        {
            for(int j=0;j<2;j++)
            {
                System.out.print(a[i][j]+" ");
            }
            System.out.println();
        }
    }
}
