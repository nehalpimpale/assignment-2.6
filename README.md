# assignment-2.6


1)Write a program to accepts two numbers from stdin and find all the odd as well as even numbers present in between them.


   import java.util.ArrayList; import java.util.Scanner;
   
   
    public class acad 
    
    
      {
      
        public static void main(String[] args) 
          { 
          
            Scanner sc=new Scanner(System.in); 
            int a=sc.nextInt();
            int b=sc.nextInt();
            ArrayList odd=new ArrayList(); //ArrayList preferred over array as the size is dynamic 
            ArrayList even=new ArrayList(); //ArrayList preferred over array as the size is dynamic \
            for(int i=a;i<=b;i++) 
            { 
            
              if(i%2==0) 
                even.add(i); //adding even numbers in ArrayList 
              else 
                odd.add(i); //adding odd numbers in ArrayList 
                
            } 
            System.out.println(); 
            System.out.println("Odd numbers are:"); 
            for(int i:odd) 
            System.out.print(i+" "); 
            System.out.println(); 
            System.out.println("\nEven numbers are:"); 
            for(int i:even) System.out.print(i+" "); 
            sc.close(); 
            
          } 
          
     }

2)Joe is scared to go to school. When her dad asked the reason, joe said she is unable to complete the task given by her teacher. The task was to find the “first 10 multiples” of the number entered from stdin.


import java.util.Scanner;

public class acad 
{ 

   public static void main(String[] args) 
      { 
      
         Scanner sc=new Scanner(System.in); 
         int n=sc.nextInt(); //accepting the number from console 
         System.out.println("Input: "+n); 
         System.out.println("O/p:"); 
         for(int i=1;i<=10;i++) 
         { 
         
            System.out.println(n+" * "+i+" = "+(n*i)); //displaying table of given number on console } 
            sc.close(); 
            
         } 
         
      }


3)Write a program consisting method sum() and demonstrate the concept of method overloading using this method.

import java.util.Scanner;

public class acad 
   { 
   
      public static void sum() //sum method with no arguments 
   { 
   
      int x=5; 
      int y=10; 
      System.out.println("Sum is (method with no arguments):"+(x+y)); 
   } 
     public static void sum(int a,int b) //sum method with 2 arguments
   { 
   
      System.out.println("Sum of first 2 numbers is (method with 2 arguments):"+(a+b)); 
   } 
   public static void sum(int a,int b,int d,int e) //sum method with 4 arguments
   { 
   
      System.out.println("Sum of all 3 numbers is (method with 4 arguments):"+(a+b+d+e)); 
   }

public static void main(String[] args)

{
     Scanner sc=new Scanner(System.in);
     int a=sc.nextInt();      
     int b=sc.nextInt();
     int d=sc.nextInt();
     int e=sc.nextInt();
     sum();
     sum(a,b);
     sum(a,b,d,e);
     sc.close();
} 

}
