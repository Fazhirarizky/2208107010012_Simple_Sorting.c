Fazhira Rizky Harmayani
2208107010012_Simple_Sorting.c

# Sorting Algorithma Benchmark

## Deskripsi
Program ini mengimplementasikan beberapa algoritma pengurutan (Bubble Sort, Selection Sort, dan Insertion Sort) dan membandingkan kinerjanya untuk ukuran masukan yang berbeda. Kinerja algoritma diukur dengan mencatat waktu eksekusi untuk setiap algoritma pada setiap ukuran masukan.

## Kompilasi dan Eksekusi
Untuk mengompilasi program, jalankan perintah berikut di terminal atau command prompt:
```
gcc sorting.c -o sorting -Wall
```

Untuk menjalankan program, gunakan perintah:

```
./sorting
```

Hasil dari benchmarking akan disimpan dalam file "sortingResults.txt".

## Algoritma Pengurutan
Program ini menggunakan tiga algoritma pengurutan berikut:

### Bubble Sort
Bubble Sort adalah algoritma sederhana yang berulang kali membandingkan setiap pasangan elemen dalam daftar dan menukar mereka jika berada dalam urutan yang salah. Algoritma ini memiliki kompleksitas waktu O(n^2), di mana n adalah jumlah elemen dalam array.

### Selection Sort
Selection Sort adalah algoritma pengurutan yang berulang kali mencari elemen terkecil dari sisa array dan menukarnya dengan elemen pertama. Algoritma ini juga memiliki kompleksitas waktu O(n^2).

### Insertion Sort
Insertion Sort adalah algoritma pengurutan yang membagi array menjadi bagian terurut dan tidak terurut. Pada setiap iterasi, algoritma memindahkan satu elemen dari bagian tidak terurut ke bagian terurut dan memastikan bahwa elemen tersebut ditempatkan pada posisi yang benar. Kompleksitas waktu Insertion Sort adalah O(n^2).

## Fungsi Utama

### generateRandomNumbers
```c
void generateRandomNumbers(int *array, int size);
```
Fungsi ini digunakan untuk mengisi array dengan angka acak.

### bubbleSort
```c
void bubbleSort(int *array, int size);
```
Fungsi ini mengimplementasikan algoritma Bubble Sort untuk mengurutkan array.

### selectionSort
```c
void selectionSort(int *array, int size);
```
Fungsi ini mengimplementasikan algoritma Selection Sort untuk mengurutkan array.

### insertionSort
```c
void insertionSort(int *array, int size);
```
Fungsi ini mengimplementasikan algoritma Insertion Sort untuk mengurutkan array.

### copyArray
```c
void copyArray(int *source, int *destination, int size);
```
Fungsi ini menyalin isi array sumber ke array tujuan.

### performSort
```c
void performSort(const char *sortName, void (*sortFunction)(int*, int), int *data, int size, FILE *file);
```
Fungsi ini melakukan sorting menggunakan algoritma yang diberikan, mencatat waktu eksekusi, dan menyimpan hasil sorting dalam file.

---

