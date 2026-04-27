# java-practice. 

import java.util.Scanner;

class EvenOdd
{
    public static void main(String args[])
    {
        Scanner sc = new Scanner(System.in);
        


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
