# Alur kerja Program #
1. Package
package ProjectUTS;
Menentukan lokasi penyimpanan class dalam project.

2. Deklarasi Class
public class SortingArray
Merupakan nama class utama yang digunakan untuk menjalankan program.

3. Main Method
public static void main(String[] args)
Method utama yang pertama kali dijalankan saat program dieksekusi.

4. Deklarasi Array
int[] A = {200, 50, 10, 4, 300, 1};
Menyimpan data angka dalam bentuk array satu dimensi.

5. Variabel Sementara
int temp;
Digunakan untuk menyimpan nilai sementara saat proses penukaran (swap).

6. Proses Sorting Ascending
-Loop Luar
for (int i = 0; i < A.length - 1; i++)
Mengatur jumlah pengulangan proses sorting.

-Loop Dalam
for (int j = 0; j < A.length - i - 1; j++)

Digunakan untuk membandingkan elemen array satu per satu.

-Kondisi Perbandingan
if (A[j] > A[j + 1])

Jika elemen kiri lebih besar dari kanan, maka dilakukan penukaran.

-Proses Swap
temp = A[j];
A[j] = A[j + 1];
A[j + 1] = temp;
Menukar posisi dua elemen.

-Output Ascending
System.out.println("Ascending:");
System.out.print(A[i] + " ");
Menampilkan hasil pengurutan dari kecil ke besar.

7. Proses Sorting Descending
-Reset Array
int[] B = {200, 50, 10, 4, 300, 1};
Membuat ulang array agar tidak menggunakan hasil sorting sebelumnya.

-Kondisi Descending
if (B[j] < B[j + 1])
Jika elemen kiri lebih kecil dari kanan, maka ditukar.

-Output Descending
System.out.println("Descending:");
System.out.print(B[i] + " ");
Menampilkan hasil pengurutan dari besar ke kecil.

8. Hasil Output
Ascending:
1 4 10 50 200 300

Descending:
300 200 50 10 4 1

