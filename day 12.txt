
// Single Inheritance

// import java.util.*;
// public class Father {
//     void gen2(){
//         System.out.println("gold");
//     }
// }
// class son extends Father
// {
//     void gen3(){
//         System.out.println("Cash");
//     }
// }
// class Main{
//     public static void main(String[] args){
//         son sc=new son();
//         sc.gen3();
//         sc.gen2();
//     }
// }


// Output
// Cash
// gold


//==========================================================================================


//Multilevel Inheritance 

// import java.util.*;
// class GrandFather{
//     void gen1(){
//         System.out.println("Diamond");
//     }
// }
// class Father extends GrandFather{
//     void gen2(){
//         System.out.println("Gold");
//     }
// }
// class son extends Father{
//     void gen3(){
//         System.out.println("Cash");
//     }
// }
// class Main{
//     public static void main(String[] args){
//         son s = new son();
//         Father f = new Father();
//         GrandFather g = new GrandFather();
//         s.gen3();
//         s.gen2();
//         f.gen2();
//         f.gen1();
//         g.gen1();
//     }
// }


// Output

// Cash
// Gold
// Gold
// Diamond
// Diamond



//==========================================================================================

// Hierarchical Inheritance

// import java.util.*;
// class Father{
//     void gen2(){
//         System.out.println("Gold");
//     }
// }
// class son extends Father{
//     void gen31(){
//         System.out.println("Cash");
//     }
// }
// class Daughter extends Father{
//     void gen32(){
//         System.out.println("Platinium");
//     }
// }
// class Main{
//     public static void main(String[] args){
//         son s = new son();
//         Daughter d = new Daughter();
//         Father f = new Father();
//         s.gen31();
//         s.gen2();
//         d.gen32();
//         d.gen2();
//         f.gen2();
//     }
// }



// output
// Cash
// Gold
// Platinium
// Gold
// Gold


//==========================================================================================

//Hybrid Inheritance 

// import java.util.*;
// class GrandFather{
//     void gen1(){
//     System.out.println("Diamond");
// }
// }
// class Father extends GrandFather{
//     void gen2(){
//         System.out.println("Gold");
//     }
// }
// class Mother extends Father{
//     void gen21(){
//         System.out.println("Copper");
//     }
// }
// class son extends Father{
//     void gen3(){
//         System.out.println("Cash");
//     }
// }
// class Main{
//     public static void main(String[] args){
//         son s = new son();
//         s.gen3();
//         s.gen2();
//         s.gen1();
//         Mother m=new Mother();
//         m.gen21();
//         m.gen2();
//     }
// }


// Output


// Cash
// Gold
// Diamond
// Copper
// Gold



//==========================================================================================

//Parameterized Constructor 


// import java.util.*;
// class Student 
// {
//     int roll;
//     String name;
//     Student(int r,String n){
//         this.roll=r;
//         this.name=n;
//     }
//     void display(){
//         System.out.println(roll+" "+name);

//     }
//     public static void main(String[] args){
//         Student s1= new Student(12,"rider");
//         Student s2= new Student(46,"Benny");
//         s1.display();
//         s2.display();
//     }
// }


// Output
// 12 rider
// 46 Benny

//==========================================================================================

// Task
// class Vehicle{
//     void displayVehicleType(){
//         System.out.println("vehicle Type: ");
//     }
// }
// class Car extends Vehicle{
//     void c1(){
//         System.out.println("Number of Wheels: Four Wheels");
//     }
// }
// class Bike extends Vehicle{
//     void b1(){
//         System.out.println("Number of Wheels: Two Wheels");
//     }
// }
// class Auto extends Vehicle{
//     void a1(){
//         System.out.println("Number of Wheels: Three Wheels");
//     }
// }
// class Main{
//     public static void main(String[] args){
//         Vehicle v=new Vehicle();
//         Car c= new Car();
//         Bike b=new Bike();
//         Auto a=new Auto();
//        c.displayVehicleType();
//        c.c1();
//        b.displayVehicleType();
//        b.b1();
//        a.displayVehicleType();
//        a.a1();


//     }
// }


// Output
// vehicle Type: 
// Number of Wheels: Four Wheels
// vehicle Type: 
// Number of Wheels: Two Wheels
// vehicle Type: 
// Number of Wheels: Three Wheels