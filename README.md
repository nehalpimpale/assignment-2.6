# assignment-2.6


1)Write a program to accepts two numbers from stdin and find all the odd as well as even numbers present in between them.


import java.util.ArrayList; import java.util.Scanner;

public class acad { public static void main(String[] args) { Scanner sc=new Scanner(System.in); int a=sc.nextInt();
int b=sc.nextInt();
ArrayList odd=new ArrayList(); //ArrayList preferred over array as the size is dynamic ArrayList even=new ArrayList(); //ArrayList preferred over array as the size is dynamic for(int i=a;i<=b;i++) { if(i%2==0) even.add(i); //adding even numbers in ArrayList else odd.add(i); //adding odd numbers in ArrayList } System.out.println(); System.out.println("Odd numbers are:"); for(int i:odd) System.out.print(i+" "); System.out.println(); System.out.println("\nEven numbers are:"); for(int i:even) System.out.print(i+" "); sc.close(); } }

2)Joe is scared to go to school. When her dad asked the reason, joe said she is unable to complete the task given by her teacher. The task was to find the “first 10 multiples” of the number entered from stdin.


3)Write a program consisting method sum() and demonstrate the concept of method overloading using this method.
