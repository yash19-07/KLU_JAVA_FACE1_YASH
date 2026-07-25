// import java.util.*;
// public class Day19 {
//     public static void main(String[] args){
//         Scanner sc = new Scanner(System.in);
//         System.out.print("Enter the size of the Matrix: ");
//         int V = sc.nextInt();
//         int E = sc.nextInt();
//         int [][] matrix = new int[V][V];
//         for(int i=0;i<E;i++){
//             int u = sc.nextInt();
//             int v = sc.nextInt();
//             matrix[u][v]=1;
//             matrix[v][u]= 1;
//         }
//         for(int i=0;i<V;i++){
//             for(int j=0;j<V;j++){
//                 System.out.print(matrix[i][j]+" ");
//             }
//             System.out.println();

//         }
//     }
// }



// Output


// Enter the size of the Matrix: 5 4 
// 0 1 
// 0 2
// 1 3
// 3 4
// 0 1 1 0 0 
// 1 0 0 1 0 
// 1 0 0 0 0 
// 0 1 0 0 1 
// 0 0 0 1 0 


//==========================================================================================



// import java.util.*;
// public class Day19 {
//     public static void main(String[] args){
//         Scanner sc = new Scanner(System.in);
//         System.out.print("Enter the size of the Matrix: ");
//         int V = sc.nextInt();
//         int E = sc.nextInt();
//         int [][] adj = new int[V][V];
//         int [] deg = new int[V];
//         for(int i=0;i<E;i++){
//             int u = sc.nextInt();
//             int v = sc.nextInt();
//             adj[u][deg[u]++]=v;
//             adj[v][deg[v]++]=u;
//         }
//         for(int i=0;i<V;i++){
//             System.out.print(i+ " ");
//             for(int j=0;j<deg[i];j++){
//                 System.out.print(adj[i][j]+" ");
//             }
//             System.out.println();

//         }
//     }
// }






//==========================================================================================



import java.util.*;
class Main{
    static int[][]graph;
    static boolean[] visited;
    static void dfs(int n,int V){
        visited[n]=true;
        System.out.print(n+" ");
        for(int i=0;i<V;i++){
            if(graph[n][i]==1 && !visited[i]){
                dfs(i,V);
            }
        }
    }
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter the Numbers: ");
        int V = sc.nextInt();
        int E = sc.nextInt();
        graph = new int[V][V];
        visited = new boolean[V];
        for(int i=0;i<E;i++){
            int u = sc.nextInt();
            int v = sc.nextInt();
            graph[u][v]=1;
            graph[v][u]=1;
        }
        dfs(0,V);
    }
}
