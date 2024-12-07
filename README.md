# Search-in-Array
Search in Array
import java.util.Scanner;

public class searchinArray {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the dimensions of Array:");
        int n = sc.nextInt();
        int m = sc.nextInt();
        System.out.println("Enter the element to be searched: ");
        int x = sc.nextInt();
        int arr[][] = new int[n][m];
        for (int i = 0; i < n; i++) {
            for (int j = 0; j < m; j++) {
                arr[i][j] = sc.nextInt();
            }
        }
        for (int i = 0; i < n; i++) {
            for (int j = 0; j < m; j++) {
                if (arr[i][j] == x) {
                    System.out.println("Row: " + i);
                    System.out.println("Column: " + j);
                    return;
                }
            }
        }
        System.out.println(-1);

    }
}
