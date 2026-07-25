
//Circular Singly Linked List

// import java.util.*;
// class Node {
//     int data;
//     Node next;

//     Node(int d) {
//         this.data = d;
//         this.next = null;
//     }
// }

// public class Main {
//     Node first;

//     void insert(int d) {
//         Node n = new Node(d);

//         if (first == null) {
//             first = n;
//             n.next = first;
//         } else {
//             Node temp = first;

//             while (temp.next != first) {
//                 temp = temp.next;
//             }

//             temp.next = n;
//             n.next = first;
//         }
//     }

//     void display() {
//         if (first == null) {
//             System.out.println("Linked List is Empty");
//             return;
//         }

//         Node temp = first;

//         do {
//             System.out.print(temp.data + " ");
//             temp = temp.next;
//         } while (temp != first);
//     }

//     public static void main(String[] args) {
//         Scanner sc = new Scanner(System.in);

//         System.out.print("Enter the Data: ");

//         Main m = new Main();

//         int d = sc.nextInt();

//         while (d != -1) {
//             m.insert(d);
//             d = sc.nextInt();
//         }

//         m.display();
//     }
// }



// Output
// Enter the Data: 10 20 40 50 -1
// 10 20 40 50 

//==========================================================================================


// Sum of Elements in Circular Singly Linked List


// import java.util.*;

// class Node {
//     int data;
//     Node next;

//     Node(int d) {
//         this.data = d;
//         this.next = null;
//     }
// }

// public class Main {
//     Node first;

//     void insert(int d) {
//         Node n = new Node(d);

//         if (first == null) {
//             first = n;
//             n.next = first;
//         } else {
//             Node temp = first;

//             while (temp.next != first) {
//                 temp = temp.next;
//             }

//             temp.next = n;
//             n.next = first;
//         }
//     }

//     void sumelements() {
//         if (first == null) {
//             System.out.println("Linked List is Empty");
//             return;
//         }

//         Node temp = first;
//         int sum=0;
//         do{
//             sum=sum+temp.data;
//             temp=temp.next;
//         }
//         while (temp != first);
    
//          System.out.print(sum+" ");
//     }

//     public static void main(String[] args) {
//         Scanner sc = new Scanner(System.in);

//         System.out.print("Enter the Data: ");

//         Main m = new Main();

//         int d = sc.nextInt();

//         while (d != -1) {
//             m.insert(d);
//             d = sc.nextInt();
//         }

//         m.sumelements();
//     }
// }


// Output

// Enter the Data: 10 20 30 40 50 -1
// 150


//==========================================================================================


//task

// import java.util.*;

// class Node {
//     int data;
//     Node next;

//     Node(int d) {
//         data = d;
//         next = null;
//     }
// }

// public class Main {
//     Node first;

//     void insert(int d) {
//         Node n = new Node(d);

//         if (first == null) {
//             first = n;
//             n.next = first;
//         } else {
//             Node temp = first;

//             while (temp.next != first) {
//                 temp = temp.next;
//             }

//             temp.next = n;
//             n.next = first;
//         }
//     }

//     void playSongs(int k) {
//         if (first == null) {
//             System.out.println("Playlist is Empty");
//             return;
//         }

//         Node temp = first;

//         System.out.println("Songs Played:");
//         for (int i = 1; i <= k; i++) {
//             System.out.println(temp.data);
//             temp = temp.next;
//         }
//     }

//     public static void main(String[] args) {
//         Scanner sc = new Scanner(System.in);

//         Main m = new Main();

//         System.out.print("Enter number of songs: ");
//         int n = sc.nextInt();

//         System.out.println("Enter Song IDs:");
//         for (int i = 0; i < n; i++) {
//             m.insert(sc.nextInt());
//         }

//         System.out.print("Enter number of songs to play: ");
//         int k = sc.nextInt();

//         m.playSongs(k);
//     }
// }


// Output
// Enter number of songs: 2
// Enter Song IDs:
// 10 20 
// Enter number of songs to play: 3
// Songs Played:
// 10
// 20
// 10



//==========================================================================================



//Circular Double Linked list 


// import java.util.*;

// class Node 
// {
//     int data;
//     Node next;
//     Node prev;

//     Node(int d) 
//     {
//         data = d;
//         next = null;
//         prev = null;
//     }
// }

// class Main 
// {

//     Node first;

    
//     void insert(int d) 
//     {
//         Node n = new Node(d);

//         if (first == null) 
//             {
//             first = n;
//             first.next = first;
//             first.prev = first;
//         } 
//         else 
//             {
//             Node last = first.prev;

//             last.next = n;
//             n.prev = last;
//             n.next = first;
//             first.prev = n;
//         }
//     }

    
//     void display()
//     {
//         if (first == null) 
//             {
//             System.out.println("Linked List is empty");
//             return;
//         }

//         Node temp = first;
//         do 
//         {
//             System.out.print(temp.data + " ");
//             temp = temp.next;
//         } 
//         while (temp != first);

//         System.out.println();
//     }

//     public static void main(String[] args) 
//     {
//         Scanner sc = new Scanner(System.in);

//         Main list = new Main();

//         System.out.print("Enter number of nodes: ");
//         int n = sc.nextInt();

//         System.out.println("Enter elements:");

//         for (int i = 0; i < n; i++) 
//             {
//             list.insert(sc.nextInt());
//         }

//         System.out.print("Circular Doubly Linked List: ");
//         list.display();
//     }
// }


// Output
// Enter number of nodes: 2
// Enter elements:
// 10 20 
// Circular Doubly Linked List: 10 20 


//==========================================================================================


// Stack


// import java.util.Scanner;

// class Stack {
//     int top;
//     int arr[];
//     int size;

//     Stack(int n) {
//         top = -1;
//         size = n;
//         arr = new int[n];
//     }

//     void push(int d) {
//         if (top == size - 1) {
//             System.out.println("Stack Overflow");
//         } else {
//             arr[++top] = d;
//             System.out.println(d + " pushed into stack");
//         }
//     }

//     void pop() {
//         if (top == -1) {
//             System.out.println("Stack Underflow");
//         } else {
//             System.out.println(arr[top]);
//             top--;
//         }
//     }

//     void peek() {
//         if (top == -1) {
//             System.out.println("Stack Underflow");
//         } else {
//             System.out.println(arr[top]);
//         }
//     }

//     void display() {
//         if (top == -1) {
//             System.out.println("Stack is Empty");
//             return;
//         }

//         System.out.print("Stack Elements: ");
//         for (int i=top;i>=0;i--) {
//             System.out.print(arr[i] + " ");
//         }
//         System.out.println();
//     }
// }

//==========================================================================================


// public class Day16 {
//     public static void main(String[] args) {
//         Scanner sc = new Scanner(System.in);

//         System.out.print("Enter stack size: ");
//         int n=sc.nextInt();
//         Stack s = new Stack(n);
//         while(true){
//                 System.out.println("1.push");
//                 System.out.println("2.pop");
//                 System.out.println("3.peek");
//                 System.out.println("4.display");
//                 System.out.println("Enter the choice ");
//                 int choice = sc.nextInt();
//                 switch(choice)
//                 {
//                     case 1:
//                         System.out.print("Enter value to Push: ");
//                         int d=sc.nextInt();
//                         s.push(d);
//                         break;
//                     case 2:
//                         s.pop();
//                         break;
//                     case 3:
//                         s.peek();
//                         break;
//                     case 4:
//                         s.display();
//                         break;
//                     case 5:
//                         return;
//                     default:
//                         System.out.print("Invalid");


//                 }

//             }
//         }

        
//     }




// Output
// Enter stack size: 4 
// 1.push
// 2.pop
// 3.peek
// 4.display
// Enter the choice 
// 3
// Stack Underflow



//==========================================================================================