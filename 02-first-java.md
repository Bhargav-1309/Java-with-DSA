1.Write a program to print whether a number is even or odd, also take input from the user.
Program:

import java.util.Scanner;

 public class EvenOdd {
       public static void main(String[] args) {
         Scanner sc = new Scanner(System.in);

         System.out.print("Enter a number: ");
         int num = sc.nextInt();

         System.out.println((num % 2 == 0) ? "Even" : "Odd");

         sc.close();
   }
 }
Output:

Enter a number: 8
Even
=== Code Execution Successful ===

2. Take name as input and print a greeting message for that particular name.
   Program:

  import java.util.Scanner;

  public class Greeting {
    public static void main(String[] args) {
      Scanner sc = new Scanner(System.in);
      System.out.print("Enter your name: ");
      String name = sc.nextLine();
      System.out.println("Hello, " + name + "! Welcome!");
      sc.close();
    }
  }
Output:

      Enter your name: Abhinav
      Hello, Abhinav! Welcome!
    === Code Execution Successful ===
    
3. Write a program to input principal, time, and rate (P, T, R) from the user and find Simple Interest.
   Program:

  import java.util.Scanner;

 public class SimpleInterest {
   public static void main(String[] args) {
     Scanner sc = new Scanner(System.in);
     System.out.print("Enter principal (P): ");
     double p = sc.nextDouble();
     System.out.print("Enter time in years (T): ");
     double t = sc.nextDouble();
     System.out.print("Enter rate (R) as percent: ");
     double r = sc.nextDouble();
     double si = (p * t * r) / 100.0;
     System.out.println("Simple Interest = " + si);
     sc.close();
  }
}
Output:

 Enter principal (P): 12
 Enter time in years (T): 2
 Enter rate (R) as percent: 3
 Simple Interest = 0.72
=== Code Execution Successful ===

4. Take in two numbers and an operator (+, -, *, /) and calculate the value. (Use if conditions)
   Program:

import java.util.Scanner;

public class Calculator {
  public static void main(String[] args) {
   Scanner sc = new Scanner(System.in);

    System.out.print("Enter first number: ");
    int a = sc.nextInt();

    System.out.print("Enter second number: ");
    int b = sc.nextInt();

    System.out.print("Enter operator (+, -, *, /): ");
    char op = sc.next().charAt(0);

    if (op == '+')
        System.out.println("Answer = " + (a + b));

    else if (op == '-')
        System.out.println("Answer = " + (a - b));

    else if (op == '*')
        System.out.println("Answer = " + (a * b));

    else if (op == '/')
        System.out.println("Answer = " + (a / b));

    else
        System.out.println("Invalid Operator");

    sc.close();
  }
}
Output:

  Enter first number: 4
  Enter second number: 7
  Enter operator (+, -, *, /): *
  Answer = 28
=== Code Execution Successful ===

5. Take 2 numbers as input and print the largest number.
Program:

import java.util.Scanner;  
public class LargestNumber {
   public static void main(String[] args) {
      Scanner sc = new Scanner(System.in);

      System.out.print("Enter first number: ");
       int a = sc.nextInt();

       System.out.print("Enter second number: ");
       int b = sc.nextInt();

       if (a > b)
           System.out.println(a + " is the largest");
       else
           System.out.println(b + " is the largest");

       sc.close();
   }
 }
Output:

Enter first number: 4
 Enter second number: 6
 6 is the largest
 === Code Execution Successful ===
 
6. Input currency in rupees and output in USD.
Program:

import java.util.Scanner;

public class RupeesToUSD {
  public static void main(String[] args) {
    Scanner sc = new Scanner(System.in);

    System.out.print("Enter amount in Rupees: ");
    double rupees = sc.nextDouble();

    double dollars = rupees * 0.012;

    System.out.println("Dollars = " + dollars);

    sc.close();
  }
}
Output:

Enter amount in Rupees: 500
Dollars = 6.0
 === Code Execution Successful ===
 
7. To calculate Fibonacci Series up to n numbers.
Program:

import java.util.Scanner;
public class Fibonacci {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("How many Fibonacci numbers to print? ");
        int n = sc.nextInt();
        int a = 0, b = 1;
        if (n <= 0) {
            System.out.println("Enter a positive integer.");
        } else if (n == 1) {
            System.out.println(a);
        } else {
            System.out.print(a + " " + b);
            for (int i = 3; i <= n; i++) {
                int c = a + b;
                System.out.print(" " + c);
                a = b;
                b = c;
            }
            System.out.println();
        }
        sc.close();
    }
}
Output:

How many Fibonacci numbers to print? 5
0 1 1 2 3
=== Code Execution Successful ===

8. To find out whether the given String is Palindrome or not. Program:

import java.util.Scanner;

public class Palindrome {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a string: ");
        String s = sc.nextLine();
        String rev = new StringBuilder(s).reverse().toString();
        if (s.equals(rev)) {
            System.out.println("\"" + s + "\" is a palindrome.");
        } else {
            System.out.println("\"" + s + "\" is not a palindrome.");
        }
        sc.close();
    }
}
Output:

Enter a string: 3
"3" is a palindrome.
=== Code Execution Successful ===

9. To find Armstrong Number between two given number.
Program:

import java.util.Scanner;

public class ArmstrongRange {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter start of range: ");
        int start = sc.nextInt();
        System.out.print("Enter end of range: ");
        int end = sc.nextInt();
        System.out.println("Armstrong numbers between " + start + " and " + end + ":");
        for (int num = Math.max(0, start); num <= end; num++) {
            if (isArmstrong(num)) {
                System.out.println(num);
            }
        }
        sc.close();
    }

    private static boolean isArmstrong(int n) {
        int original = n;
        int digits = String.valueOf(n).length();
        int sum = 0;
        while (n > 0) {
            int d = n % 10;
            sum += Math.pow(d, digits);
            n /= 10;
        }
        return sum == original;
    }
}
Output:

Enter start of range: 1
Enter end of range: 67
Armstrong numbers between 1 and 67:
1
2
3
4
5
6
7
8
9
=== Code Execution Successful ===
