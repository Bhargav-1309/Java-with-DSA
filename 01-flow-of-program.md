1. Input a year and find whether it is a leap year or not.
Program:

import java.util.Scanner;

class Main {
public static void main(String[] args) {
    Scanner sc = new Scanner(System.in);

    System.out.print("Enter a year: ");
    int year = sc.nextInt();

    if ((year % 400 == 0) || (year % 4 == 0 && year % 100 != 0)) {
        System.out.println(year + " is a leap year.");
    } else {
        System.out.println(year + " is not a leap year.");
      }
  }
}
Output: Enter year: 2024 2024 is a leap year.

=== Code Execution Successful ===

2. Take two numbers and print the sum of both. Program:

  class Main {
     public static void main(String[] args) {
         int a = 4;
         int b = 5;
         System.out.println(a+b);
     }
 }
Output: 9

=== Code Execution Successful ===

3. Take a number as input and print the multiplication table for it. Program:

class Main {
 public static void main(String[] args) {
 int n = 8;

     System.out.println(n + " x 1 = " + (n * 1));
     System.out.println(n + " x 2 = " + (n * 2));
     System.out.println(n + " x 3 = " + (n * 3));
     System.out.println(n + " x 4 = " + (n * 4));
     System.out.println(n + " x 5 = " + (n * 5));
     System.out.println(n + " x 6 = " + (n * 6));
     System.out.println(n + " x 7 = " + (n * 7));
     System.out.println(n + " x 8 = " + (n * 8));
     System.out.println(n + " x 9 = " + (n * 9));
     System.out.println(n + " x 10 = " + (n * 10));
  }
}
Output: 8 x 1 = 8 8 x 2 = 16 8 x 3 = 24 8 x 4 = 32 8 x 5 = 40 8 x 6 = 48 8 x 7 = 56 8 x 8 = 64 8 x 9 = 72 8 x 10 = 80

=== Code Execution Successful ===

4. Take 2 numbers as inputs and find their HCF and LCM. Program:

 import java.util.Scanner;
   class Main {
     public static void main(String[] args) {
     Scanner sc = new Scanner(System.in);

 System.out.print("Enter first number: ");
 int a = sc.nextInt();

 System.out.print("Enter second number: ");
 int b = sc.nextInt();

 int hcf = 1;

 for (int i = 1; i <= a && i <= b; i++) {
     if (a % i == 0 && b % i == 0) {
         hcf = i;
     }
 }

 int lcm = (a * b) / hcf;

 System.out.println("HCF = " + hcf);
 System.out.println("LCM = " + lcm);
   }
 }
Output: Enter first number: 4 Enter second number: 8 HCF = 4 LCM = 8

=== Code Execution Successful ===

5. Keep taking numbers as inputs till the user enters ‘x’, after that print sum of all. Program:

 import java.util.Scanner;
   class Main {
     public static void main(String[] args) {
     Scanner sc = new Scanner(System.in);

 int sum = 0;

 while (true) {
     System.out.print("Enter a number or x to stop: ");
     String input = sc.next();

     if (input.equals("x")) {
         break;
     }

     int num = Integer.parseInt(input);
     sum = sum + num;
 }

 System.out.println("Sum = " + sum);
 }
 }
Output: Enter a number or x to stop: 25 Enter a number or x to stop: 25 Enter a number or x to stop: 35 Enter a number or x to stop: x Sum = 85

=== Code Execution Successful ===
