
//Queue With Linked List



// import java.util.*;

// class Queue {
//     int front, rear;
//     int n;
//     int arr[];

//     Queue(int n) {
//         this.n = n;
//         arr = new int[n];
//         front = 0;
//         rear = -1;
//     }

//     void enqueue(int data) {
//         if (rear == n - 1) {
//             System.out.println("Queue is Full");
//             return;
//         }
//         arr[++rear] = data;
//         System.out.println(data + " Enqueued");
//     }

//     void dequeue() {
//         if (front > rear) {
//             System.out.println("Queue is Empty");
//             return;
//         }
//         System.out.println("Dequeued: " + arr[front++]);
//     }

//     void display() {
//         if (front > rear) {
//             System.out.println("Queue is Empty");
//             return;
//         }

//         System.out.print("Queue: ");
//         for (int i = front; i <= rear; i++) {
//             System.out.print(arr[i] + " ");
//         }
//         System.out.println();
//     }
// }

// public class Main {
//     public static void main(String[] args) {

//         Scanner sc = new Scanner(System.in);

//         System.out.print("Enter Queue Size: ");
//         int n = sc.nextInt();

//         Queue q = new Queue(n);

//         while (true) {
//             System.out.println("\n1. Enqueue");
//             System.out.println("2. Dequeue");
//             System.out.println("3. Display");
//             System.out.println("4. Exit");
//             System.out.print("Enter your choice: ");

//             int choice = sc.nextInt();

//             switch (choice) {
//                 case 1:
//                     System.out.print("Enter value: ");
//                     int val = sc.nextInt();
//                     q.enqueue(val);
//                     break;

//                 case 2:
//                     q.dequeue();
//                     break;

//                 case 3:
//                     q.display();
//                     break;

//                 case 4:
//                     System.out.println("Exiting...");
//                     sc.close();
//                     return;

//                 default:
//                     System.out.println("Invalid Choice");
//             }
//         }
//     }
// }

// Output




// Enter Queue Size: 5

// 1. Enqueue
// 2. Dequeue
// 3. Display
// 4. Exit
// Enter your choice: 1
// Enter value: 10
// 10 Enqueued

// 1. Enqueue
// 2. Dequeue
// 3. Display
// 4. Exit
// Enter your choice: 3 
// Queue: 10 

// 1. Enqueue
// 2. Dequeue
// 3. Display
// 4. Exit
// Enter your choice: 1
// Enter value: 27
// 27 Enqueued

// 1. Enqueue
// 2. Dequeue
// 3. Display
// 4. Exit
// Enter your choice: 3
// Queue: 10 27 

// 1. Enqueue
// 2. Dequeue
// 3. Display
// 4. Exit
// Enter your choice: 

//==========================================================================================

//Stack with Linked List 


import java.util.Scanner;

class Node {
    int data;
    Node next;

    Node(int data) {
        this.data = data;
        this.next = null;
    }
}

class Stack {
    Node top;

    
    void push(int data) {
        Node newNode = new Node(data);
        newNode.next = top;
        top = newNode;
        System.out.println(data + " pushed into stack");
    }

    
    void pop() {
        if (top == null) {
            System.out.println("Stack Underflow");
        } else {
            System.out.println(top.data + " popped from stack");
            top = top.next;
        }
    }

    
    void peek() {
        if (top == null) {
            System.out.println("Stack is Empty");
        } else {
            System.out.println("Top Element: " + top.data);
        }
    }

    
    void display() {
        if (top == null) {
            System.out.println("Stack is Empty");
        } else {
            System.out.println("Stack Elements:");
            Node temp = top;
            while (temp != null) {
                System.out.print(temp.data + " ");
                temp = temp.next;
            }
            System.out.println();
        }
    }

   
    boolean isEmpty() {
        return top == null;
    }
}

public class Day17 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Stack s = new Stack();

        while (true) {
            System.out.println("\n1. Push");
            System.out.println("2. Pop");
            System.out.println("3. Peek");
            System.out.println("4. Display");
            System.out.println("5. Exit");
            System.out.print("Enter your choice: ");

            int choice = sc.nextInt();

            switch (choice) {
                case 1:
                    System.out.print("Enter element: ");
                    int data = sc.nextInt();
                    s.push(data);
                    break;

                case 2:
                    s.pop();
                    break;

                case 3:
                    s.peek();
                    break;

                case 4:
                    s.display();
                    break;

                case 5:
                    System.out.println("Program Ended");
                    sc.close();
                    return;

                default:
                    System.out.println("Invalid Choice");
            }
        }
    }
}