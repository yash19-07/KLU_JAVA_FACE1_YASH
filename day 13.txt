// //Private Access modifier

//Example 1

// package P2;
// public class Day14{
//     private int x=10;
//     public static void main(String[] args){
//         Main obj = new Main();
//         System.out.println(obj.x);
//     }
// }


// Output

// Exception in thread "main" java.lang.Error: Unresolved compilation problem: 
//         x cannot be resolved or is not a field


//==========================================================================================

//Example 2


// public class Day14{
//     public static void main(String[] args){
//         Class108 obj = new Class108();
//         System.out.println(obj.x);

//     }
// }
// public class Class108{
//     private int x=12;
// }


// Output
// Exception in thread "main" java.lang.Error: Unresolved compilation problem: 
//         The field class108.x is not visible


//==========================================================================================


//Default Access Modifier



// package C1;

// public class A {
//     public static void main(String[] args) {
//         B obj = new B();
//         obj.display();
//     }
// }

// public class B {
//     void display() {
//         System.out.println("Default Access Modifier");
//     }
// }


//==========================================================================================

// import java.util.*;
// import java.lang.*;
// import java.io.*;

// class Codechef{
//     void display(int a){
//         System.out.println("Integer data: "+a);
//     }
//     void display(float b){
//         System.out.println("Float data: "+b);
//     }
//     public static void main(String[] args){
//         Scanner sc = new Scanner(System.in);
//         Codechef c= new Codechef();
//         int a = sc.nextInt();
//         float b = sc.nextFloat();
//         c.display(a);
//         c.display(b);
//     }
// }


// Output
// Integer data: 10
// Float data: 2.5


//==========================================================================================

//Method Overloading with different order of parameters 


// import java.util.*;
// import java.lang.*;
// import java.io.*;

// class Codechef{
//     void display(int a,float b){
//         System.out.println(a+" "+b);
//     }
//     void display(float b,char c){
//         System.out.println(b+" "+c);
//     }
//     public static void main(String[] args){
//         Scanner sc = new Scanner(System.in);
//         System.out.print("Enter the data: ");
//         Codechef cf= new Codechef();
//         int a;
//         float b;
//         char c;
//         a=sc.nextInt();
//         b=sc.nextFloat();
//         c=sc.next().charAt(0);
//         cf.display(a,b);
//         cf.display(b, c);
//     }
// }

// Output
// Enter the data: 10 20.5 d
// 10 20.5
// 20.5 d


//==========================================================================================

// Copy Constructor 

// import java.util.*;
// import java.lang.*;
// import java.io.*;

// class Student {
//     int rollno;
//     String name;
//     Student(int r,String n)
//     {
//         this.rollno=r;
//         this.name=n;

//     }
//     Student(Student s){
//         s.rollno=46;
//     }
//     void display(){
//         System.out.print(rollno+" "+name );
//     }
//     public static void main(String[] args){
//         System.out.print("The Details are : ");
//         Student s1=new Student(11,"Benny  ");
//         Student s2=new Student(s1);
//         s1.display();
//     }
// }

// output
// The Details are : 46 Benny  


//==========================================================================================


// Runtime Polymorphism/Method Over Riding


// class Shape{
//     void area(){
//         System.out.println("DISPLAY DIFFERENT SHAPES FORMULA");

//     }
// }
// class Rectangle extends Shape{
//     void area(){
//         System.out.println("L*B");
        
//     }
// }

// class Circle extends Shape{
//     void area(){
//         System.out.println("3.14*r*r");
        
//     }
// }
// class Main{
//     public static void main(String[] args){
//        Shape r= new Rectangle();
//        Shape c=new Circle();
//        r.area();
//        c.area();

//     }
// }

// Output
// L*B
// 3.14*r*r