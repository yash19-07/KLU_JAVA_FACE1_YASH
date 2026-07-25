
//Preorder Traversal

// import java.util.*;
// class Node
// {
//     int data;
//     Node left, right;

//     Node(int data)
//     {
//         this.data = data;
//         left = right = null;
//     }
// }
// class Main
// {
//     static void preorder(Node node)
//     {
//         if(node != null)
//         {
//             System.out.print(node.data + " ");
//             preorder(node.left);
//             preorder(node.right);
//         }
//     }
//     public static void main(String[] args)
//     {
//         Scanner sc = new Scanner(System.in);
//         System.out.println("Enter 5 Values");
//         Node root = new Node(sc.nextInt());
//         root.left = new Node(sc.nextInt());
//         root.right = new Node(sc.nextInt());
//         root.left.left = new Node(sc.nextInt());
//         root.left.right = new Node(sc.nextInt());
//         System.out.println("Preorder Traversal");
//         preorder(root);

//         sc.close();
//     }
// }


//==========================================================================================


//postorder Traversal



// import java.util.*;
// class Node
// {
//     int data;
//     Node left, right;

//     Node(int data)
//     {
//         this.data = data;
//         left = right = null;
//     }
// }
// class Main
// {
//     static void postorder(Node node)
//     {
//         if(node != null)
//         {
//             
//             postorder(node.left);
//             postrder(node.right);
//             System.out.print(node.data + " ");
//         }
//     }
//     public static void main(String[] args)
//     {
//         Scanner sc = new Scanner(System.in);
//         System.out.println("Enter 5 Values");
//         Node root = new Node(sc.nextInt());
//         root.left = new Node(sc.nextInt());
//         root.right = new Node(sc.nextInt());
//         root.left.left = new Node(sc.nextInt());
//         root.left.right = new Node(sc.nextInt());
//         System.out.println("Postorder Traversal");
//         postorder(root);

//         
//     }
// }



//==========================================================================================


//Inorder Traversal



// import java.util.*;
// class Node
// {
//     int data;
//     Node left, right;

//     Node(int data)
//     {
//         this.data = data;
//         left = right = null;
//     }
// }
// class Main
// {
//     static void inorder(Node node)
//     {
//         if(node != null)
//         {
//             inorder(node.left);
//             System.out.print(node.data + " ");
//             inorder(node.right);
//         }
//     }
//     public static void main(String[] args)
//     {
//         Scanner sc = new Scanner(System.in);
//         System.out.println("Enter 5 Values");
//         Node root = new Node(sc.nextInt());
//         root.left = new Node(sc.nextInt());
//         root.right = new Node(sc.nextInt());
//         root.left.left = new Node(sc.nextInt());
//         root.left.right = new Node(sc.nextInt());
//         System.out.println("Inorder Traversal");
//         inorder(root);

//     }
// }



