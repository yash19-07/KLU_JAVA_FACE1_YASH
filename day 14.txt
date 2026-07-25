
//Single Linked List

// import java.util.*;

// class Node {
//     int data;
//     Node next;

//     Node(int d) {
//         this.data = d;
//         this.next = null;
//     }
// }

// class Main {
//     Node first;

//     void insert(int d) {
//         Node n = new Node(d);

//         if (first == null) {
//             first = n;
//             return;
//         }

//         Node temp = first;
//         while (temp.next != null) {
//             temp = temp.next;
//         }
//         temp.next = n;
//     }

//     void display() {
//         if (first == null) {
//             System.out.println("Linked List is Empty");
//             return;
//         }

//         Node temp = first;

//         while (temp != null) {
//             System.out.print(temp.data + " ");
//             temp = temp.next;
//         }
//     }

//     public static void main(String[] args) {
//         Scanner sc = new Scanner(System.in);
//         System.out.print("Enter the numbers: ");
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
// Enter the numbers: 10 20 30 40 50 -1
// 10 20 30 40 50 


//==========================================================================================


// Sum of the Elements in the Single Linked List 


// import java.util.*;

// class Node {
//     int data;
//     Node next;

//     Node(int d) {
//         this.data = d;
//         this.next = null;
//     }
// }

// class Main {
//     Node first;

//     void insert(int d) {
//         Node n = new Node(d);

//         if (first == null) {
//             first = n;
//             return;
//         }

//         Node temp = first;
//         while (temp.next != null) {
//             temp = temp.next;
//         }
//         temp.next = n;
//     }

//     void sumelements() {
//         int sum=0;
//         if (first == null) {
//             System.out.println("Linked List is Empty");
//             return;
//         }

//         Node temp = first;

//         while (temp != null) {
//             sum+=temp.data;
//             temp = temp.next;
//         }
//          System.out.print(sum+" ");
//     }

//     public static void main(String[] args) {
//         Scanner sc = new Scanner(System.in);
//         System.out.print("Enter the numbers: ");
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

// Enter the numbers: 1 2 3 4 5 -1
// 15

//==========================================================================================


//Write a java program to find the maximum element in the linked list

// import java.util.*;

// class Node {
//     int data;
//     Node next;

//     Node(int d) {
//         this.data = d;
//         this.next = null;
//     }
// }

// class Main {
//     Node first;

//     void insert(int d) {
//         Node n = new Node(d);

//         if (first == null) {
//             first = n;
//             return;
//         }

//         Node temp = first;
//         while (temp.next != null) {
//             temp = temp.next;
//         }
//         temp.next = n;
//     }

//     void maxelements() {
//         int max = Integer.MIN_VALUE;
//         if (first == null) {
//             System.out.println("Linked List is Empty");
//             return;
//         }

//         Node temp = first;

//         while (temp != null) {
//             if(temp.data>max)
//                 max=temp.data;
//             temp = temp.next;
//         }
//          System.out.print(max+" ");
//     }

//     public static void main(String[] args) {
//         Scanner sc = new Scanner(System.in);
//         System.out.print("Enter the numbers: ");
//         Main m = new Main();

//         int d = sc.nextInt();

//         while (d != -1) {
//             m.insert(d);
//             d = sc.nextInt();
//         }

//         m.maxelements();
//     }
// }


// //output

// Enter the numbers: 1 5 9 40 23 -1
// 40 



//==========================================================================================

//Write a java program to find the minimum element in the linked list



//  import java.util.*;

// class Node {
//     int data;
//     Node next;

//     Node(int d) {
//         this.data = d;
//         this.next = null;
//     }
// }

// class Main {
//     Node first;

//     void insert(int d) {
//         Node n = new Node(d);

//         if (first == null) {
//             first = n;
//             return;
//         }

//         Node temp = first;
//         while (temp.next != null) {
//             temp = temp.next;
//         }
//         temp.next = n;
//     }

//     void maxelements() {
//         int min = Integer.MAX_VALUE;
//         if (first == null) {
//             System.out.println("Linked List is Empty");
//             return;
//         }

//         Node temp = first;

//         while (temp != null) {
//             if(temp.data<min)
//                 min=temp.data;
//             temp = temp.next;
//         }
//          System.out.print(min+" ");
//     }

//     public static void main(String[] args) {
//         Scanner sc = new Scanner(System.in);
//         System.out.print("Enter the numbers: ");
//         Main m = new Main();

//         int d = sc.nextInt();

//         while (d != -1) {
//             m.insert(d);
//             d = sc.nextInt();
//         }

//         m.maxelements();
//     }
// }


// Output

// Enter the numbers: 1 5 9 40 23 -1
// 1


//==========================================================================================


//Write a java program to find the Average element in the linked list


//  import java.util.*;

// class Node {
//     int data;
//     Node next;

//     Node(int d) {
//         this.data = d;
//         this.next = null;
//     }
// }

// class Main {
//     Node first;

//     void insert(int d) {
//         Node n = new Node(d);

//         if (first == null) {
//             first = n;
//             return;
//         }

//         Node temp = first;
//         while (temp.next != null) {
//             temp = temp.next;
//         }
//         temp.next = n;
//     }

//     void average() {
//         int count=0,sum=0;
//         if (first == null) {
//             System.out.println("Linked List is Empty");
//             return;
//         }

//         Node temp = first;

//         while (temp != null) {
//             count++;
//             sum+=temp.data;
//             temp = temp.next;
//         }
//          System.out.print("Average is : "+(float)(sum/count));
//     }

//     public static void main(String[] args) {
//         Scanner sc = new Scanner(System.in);
//         System.out.print("Enter the numbers: ");
//         Main m = new Main();

//         int d = sc.nextInt();

//         while (d != -1) {
//             m.insert(d);
//             d = sc.nextInt();
//         }

//         m.average();
//     }
// }




// Output


// Enter the numbers: 1 3 6 9 29 65 -1
// Average is : 18.0


//==========================================================================================


//Write a java program to insert the elements at any point in the single linked list

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
//             return;
//         }

//         Node temp = first;
//         while (temp.next != null) {
//             temp = temp.next;
//         }
//         temp.next = n;
//     }

  
//     void insert(int d, int pos) {
//         Node n = new Node(d);

//         if (pos == 1) {
//             n.next = first;
//             first = n;
//             return;
//         }

//         Node temp = first;

//         for (int i = 1; i < pos - 1 && temp != null; i++) {
//             temp = temp.next;
//         }

//         if (temp == null) {
//             System.out.println("Invalid Position");
//             return;
//         }

//         n.next = temp.next;
//         temp.next = n;
//     }

//     void display() {
//         if (first == null) {
//             System.out.println("Linked List is Empty");
//             return;
//         }

//         Node temp = first;
//         while (temp != null) {
//             System.out.print(temp.data + " ");
//             temp = temp.next;
//         }
//     }

//     public static void main(String[] args) {
//         Scanner sc = new Scanner(System.in);
//         Main m = new Main();

//         System.out.println("Enter elements (-1 to stop):");

//         int d = sc.nextInt();

//         while (d != -1) {
//             m.insert(d);
//             d = sc.nextInt();
//         }

//         System.out.print("Enter element to insert: ");
//         int data = sc.nextInt();

//         System.out.print("Enter position: ");
//         int pos = sc.nextInt();

//         m.insert(data, pos);

//         System.out.println("Linked List:");
//         m.display();
//     }
// }


// output

// Enter elements (-1 to stop):
// 1 3 59 33 49 -1
// Enter element to insert: 45
// Enter position: 2
// Linked List:
// 1 45 3 59 33 49 



//==========================================================================================


//DOUBLE Linked List


// import java.util.*;

// class Node {
//     int data;
//     Node next;
//     Node prev;

//     Node(int d) {
//         this.data = d;
//         this.next = null;
//         this.prev = null;
//     }
// }

// class Main {
//     Node first;

//     void insert(int d) {
//         Node n = new Node(d);

//         if (first == null) {
//             first = n;
//             return;
//         }

//         Node temp = first;

//         while (temp.next != null) {
//             temp = temp.next;
//         }

//         temp.next = n;
//         n.prev = temp;
//     }

//     void display() {
//         if (first == null) {
//             System.out.println("Linked List is Empty");
//             return;
//         }

//         Node temp = first;

//         while (temp != null) {
//             System.out.print(temp.data + " ");
//             temp = temp.next;
//         }
//     }

//     public static void main(String[] args) {
//         Scanner sc = new Scanner(System.in);
//         Main m = new Main();

//         System.out.print("Enter the numbers: ");

//         int d = sc.nextInt();

//         while (d != -1) {
//             m.insert(d);
//             d = sc.nextInt();
//         }

//         m.display();
//     }
// }



// Output
// Enter the numbers: 10 20 30 40 50 -1
// 10 20 30 40 50 