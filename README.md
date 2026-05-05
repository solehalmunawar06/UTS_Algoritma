# UTS_Algoritma

package ProjectUTS;
public class SortingArray {
    public static void main(String[] args) {
        int[] A = {200, 50, 10, 4, 300, 1};
        int temp;

        // ASCENDING
        for (int i = 0; i < A.length - 1; i++) {
            for (int j = 0; j < A.length - i - 1; j++) {
                if (A[j] > A[j + 1]) {
                    temp = A[j];
                    A[j] = A[j + 1];
                    A[j + 1] = temp;
                }
            }
        }

        System.out.println("Ascending:");
        for (int i = 0; i < A.length; i++) {
            System.out.print(A[i] + " ");
        }

        // Reset array
        int[] B = {200, 50, 10, 4, 300, 1};

        // DESCENDING
        for (int i = 0; i < B.length - 1; i++) {
            for (int j = 0; j < B.length - i - 1; j++) {
                if (B[j] < B[j + 1]) {
                    temp = B[j];
                    B[j] = B[j + 1];
                    B[j + 1] = temp;
                }
            }
        }

        System.out.println("\nDescending:");
        for (int i = 0; i < B.length; i++) {
            System.out.print(B[i] + " ");
        }
    }
}

