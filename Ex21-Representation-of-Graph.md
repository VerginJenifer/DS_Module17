# Ex21 Representation of Graph
## DATE:
## AIM:
To write a C program to display the adjacency matrix of the given graph by supplying the edges and the number of vertices.

## Algorithm
1. Initialize the adjacency matrix with all zeros.
2. Read the number of vertices (V).
3. Loop up to maximum edges (V*(V-1)) or until input (-1, -1) is encountered:
   - Read edge endpoints (e1, e2).
   - Add edge to adjacency matrix by setting adjMatrix[e1][e2] = 1.
4. After input ends, print the adjacency matrix.
5. End program. 

## Program:
```

Program to display the adjacency matrix of the given graph
Developed by: D VERGIN JENIFER
RegisterNumber: 212223240174
/*#include<stdio.h>
int V;

//init matrix to 0
void init(int arr[][V])
{
    int i,j;
    for(i = 0; i < V; i++)
        for(j = 0; j < V; j++)
            arr[i][j] = 0;
}
*/
int main()
{  int e1,e2,me,n,i;
    scanf("%d",&V);
    int adjMatrix[V][V];
    init(adjMatrix);
    n=V;
    me=n*(n-1);
    for(i=1;i<=me;i++){
        scanf("%d%d",&e1,&e2);
        addEdge(adjMatrix,e1,e2);
        if((e1==-1)&&(e2==-1))
            break;
        
    }
    printAdjMatrix(adjMatrix);
 //type your code here...
 
}

```

## Output:

![output](img/adjmat.png)

## Result:
Thus, the C program to print the adjacency matrix of the given graph is implemented successfully.
