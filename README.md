# ADDITION-OF-ELEMENTS
import java.util.*;
class Main {
    public static void main(String[] args) {
        int c=0;
        Scanner sc= new Scanner(System.in);
          System.out.println("Enter array length: ");
        int n=sc.nextInt();// Array length
         int [][]a=new int[n][n];
         int [][]b=new int[n][n];
          System.out.println("Enter array1 elements: ");
        for(int i=0;i<n;i++){
            for(int j=0;j<n;j++){
            int k=sc.nextInt();
            a[i][j]=k;
            }
        }
         System.out.println("Enter second matrix elements: ");
        for (int i=0;i<n;i++){
            for(int j=0;j<n;j++){
            int k=sc.nextInt();
            b[i][j]=k;
            }
        }
        for (int i=0;i<n;i++){
            for(int j=0;j<n;j++){
            int k=sc.nextInt();
            a[i][j]+=b[i][j];
            }
        }
         System.out.println("After addition matrix: ");
        for (int i=0;i<n;i++){
            for(int j=0;j<n;j++){
             System.out.print(b[i][j]+" ");
            }
            System.out.println();
        }
    }
}
