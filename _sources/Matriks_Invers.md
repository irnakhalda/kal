---
title: MATRIKS INVERS

---

---
title: MATRIKS INVERS

---

# MATRIKS INVERS
### Definisi Matriks Invers

Matriks invers adalah matriks yang jika dikalikan dengan matriks aslinya, menghasilkan matriks identitas. Dengan kata lain, matriks invers berfungsi sebagai kebalikan dari suatu matriks dalam operasi perkalian matriks.

Secara matematis, jika ${A}$ adalah sebuah matriks persegi, maka inversnya, yang ditulis sebagai $A^{-1}$, memenuhi persamaan:

$$
A \times A^{-1}=A^{-1} \times A=I
$$

di mana $I$ adalah matriks identitas, yaitu matriks dengan angka 1 di diagonal utama dan $\mathbf{0}$ di tempat lainnya. Tidak semua matriks memiliki invers; hanya matriks persegi yang determinannya tidak nol yang memiliki invers.
Contoh matriks identitas untuk ukuran $3 \times 3$ : 


$$
I=\left[\begin{array}{lll}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{array}\right]
$$
### Syarat Suatu Matriks Memiliki Invers

Suatu matriks $A$ bisa memiliki invers $A^{-1}$ jika memenuhi dua syarat berikut:
1. Matriks harus berbentuk persegi $\rightarrow$ jumlah baris harus sama dengan jumlah kolom.
2. Determinan tidak boleh nol $\rightarrow|A| \neq 0$. Jika determinannya nol $(|A|=0)$, maka matriks disebut singular dan tidak memiliki invers.
## MATRIKS 3 PERSAMAAN

$$
\begin{array}{r}2 x_1+3 x_2-x_3=2 \\ x_1-x_2+4 x_3=1 \\ 3 x_1+2 x_2+5 x_3=3\end{array}
$$

### 1. Diketahui Matriks ${A}$

Kita memiliki matriks $A$ : 

$$
A=\left[\begin{array}{ccc}2 & 3 & -1 \\ 
1 & -1 & 4 \\ 
3 & 2 & 5\end{array}\right]
$$

### 2. Membentuk Matriks Augmented [A | I]

$$
[A \mid I]=\left[\begin{array}{ccc|ccc}2 & 3 & -1 & \mid 1 & 0 & 0 \\ 1 & -1 & 4 & \mid 0 & 1 & 0 \\ 3 & 2 & 5 & \mid 0 & 0 & 1\end{array}\right]
$$

Tujuan: Kita harus mengubah bagian kiri menjadi identitas $I$, dan bagian kanan akan menjadi invers $A^{-1}$.

### 3. Membuat Elemen $(1,1)$ Menjadi 1

Saat ini, elemen pertama $(1,1)$ adalah 2, jadi kita bagi seluruh baris 1 dengan 2:

$$
\begin{gathered}R_1 \rightarrow \frac{1}{2} R_1 \\ {\left[\begin{array}{cccccc}1 & \frac{3}{2} & -\frac{1}{2} & \left\lvert\, \frac{1}{2}\right. & 0 & 0 \\ 1 & -1 & 4 & \mid 0 & 1 & 0 \\ 3 & 2 & 5 & \mid 0 & 0 & 1\end{array}\right]}\end{gathered}
$$

### 4. Membuat Elemen di Kolom 1 (Baris 2 dan 3) Menjadi 0

Kita buat elemen $(2,1)$ dan $(3,1)$ menjadi 0.

- Baris $2 \rightarrow R_2=R_2-R_1$
- Baris $3 \rightarrow R_3=R_3-3 R_1$


#### Langkah 1: Menjadikan Elemen (2,1) 
Elemen ( 2,1 ) saat ini adalah 1.
Untuk mengubahnya menjadi 0, kita lakukan operasi baris:

$$
R_2=R_2-R_1
$$

Perhitungan Baris 2 Baru ( $\mathbf{R}_{\mathbf{2}}$ )
Penjelasan:
Ambil baris kedua dikurangi baris pertama.


$$
\begin{array}{|l|l|l|l|}
\hline Elemen & Nilai Lama \left(R_2\right) & Nilai R_1 & Hasil Baru \left(R_2-R_1\right) \\
\hline(2,1) & 1 & 1 & 1-1=0 \\
\hline(2,2) & -1 & \frac{3}{2} & -1-\frac{3}{2}=-\frac{2}{2}-\frac{3}{2}=-\frac{5}{2} \\
\hline(2,3) & 4 & -\frac{1}{2} & 4-\left(-\frac{1}{2}\right)=4+\frac{1}{2}=\frac{8}{2}+\frac{1}{2}=\frac{9}{2} \\
\hline(2,4) & 0 & \frac{1}{2} & 0-\frac{1}{2}=-\frac{1}{2} \\
\hline(2,5) & 1 & 0 & 1-0=1 \\
\hline(2,6) & 0 & 0 & 0-0=0 \\
\hline
\end{array}
$$


Hasil baris 2 baru:
$
\left(0,-\frac{5}{2}, \frac{9}{2},-\frac{1}{2}, 1,0\right)
$

#### Langkah 2: Menjadikan Elemen (3,1) = 0
Elemen ( 3,1 ) saat ini adalah 3.
Untuk mengubahnya menjadi 0, kita lakukan operasi baris:

$$
R_3=R_3-3 R_1
$$

Perhitungan Baris 3 Baru ( $\mathbf{R}_3$ )
Setiap elemen baris $\mathbf{3}$ dikurangi $\mathbf{3 \times}$ baris 1 .

$$
\begin{array}{|l|l|l|l|}
\hline Elemen & Nilai Lama \left(R_3\right) & 3 \times R_1 & Hasil Baru \left(R_3-3 R_1\right) \\
\hline(3,1) & 3 & 3 \times 1=3 & 3-3=0 \\
\hline(3,2) & 2 & 3 \times \frac{3}{2}=\frac{9}{2}& 2-\frac{9}{2}=\frac{4}{2}-\frac{9}{2}=-\frac{5}{2}\\
\hline(3,3) & 5 & 3 \times-\frac{1}{2}=-\frac{3}{2}& 5-\left(-\frac{3}{2}\right)=5+\frac{3}{2}=\frac{10}{2}+\frac{3}{2}=\frac{13}{2}\\
\hline(3,4) & 0 & 3 \times \frac{1}{2}=\frac{3}{2}& 0-\frac{3}{2}=-\frac{3}{2}\\
\hline(3,5) & 0 & 3 \times 0=0 & 0-0=0 \\
\hline(3,6) & 1 & 3 \times 0=0 & 1-0=1 \\
\hline
\end{array}
$$

Hasil baris 3 baru:
$
\left(0,-\frac{5}{2}, \frac{13}{2},-\frac{3}{2}, 0,1\right)
$

 Hasil matriks setelah eliminasi:

$$
\left[\begin{array}{ccc|ccc}1 & \frac{3}{2} & -\frac{1}{2} & \frac{1}{2} & 0 & 0 \\ 0 & -\frac{5}{2} & \frac{9}{2} & -\frac{1}{2} & 1 & 0 \\ 0 & -\frac{5}{2} & \frac{13}{2} & -\frac{3}{2} & 0 & 1\end{array}\right]
$$

### 5. Membuat Elemen $(2,2)$ Menjadi 1

Saat ini, elemen $(2,2)$ adalah $-\frac{5}{2}$. Untuk menjadikannya 1 , kita bagi baris 2 dengan $-\frac{5}{2}$ : 

$$
R_2 \rightarrow \frac{2}{-5} R_2
$$

Perhitungan Baris 2 Baru

Kita lakukan pembagian untuk setiap elemen di baris 2:


$$
\begin{array}{|l|l|l|l|}
\hline Elemen & Nilai Lama \left(R_2\right) & Dibagi -5 / 2 & Hasil Baru \\
\hline(2,1) & 0 & 0 \div(-5 / 2) & 0 \\
\hline(2,2) & -\frac{5}{2} & \left(-\frac{5}{2}\right) \div\left(-\frac{5}{2}\right) & 1 \\
\hline(2,3) & \frac{9}{2} & \frac{9}{2} \div(-5 / 2) & -\frac{9}{5} \\
\hline(2,4) & -\frac{1}{2} & -\frac{1}{2} \div(-5 / 2) & \frac{1}{5} \\
\hline(2,5) & 1 & 1 \div(-5 / 2) & -\frac{2}{5} \\
\hline(2,6) & 0 & 0 \div(-5 / 2) & 0 \\
\hline
\end{array}
$$


Hasil baris 2 setelah pembagian:

$$
\left(0,1,-\frac{9}{5}, \frac{1}{5},-\frac{2}{5}, 0\right)
$$
Hasilnya menjadi:

$$
\left[\begin{array}{ccc|ccc}
1 & \frac{3}{2} & -\frac{1}{2} & \frac{1}{2} & 0 & 0 \\
0 & 1 & -\frac{9}{5} & \frac{1}{5} & -\frac{2}{5} & 0 \\
0 & -\frac{5}{2} & \frac{13}{2} & -\frac{3}{2} & 0 & 1
\end{array}\right]
$$

### 6. Menghilangkan Elemen di Kolom 2 (Baris 1 dan 3)
- Baris $1 \rightarrow R_1=R_1-\frac{3}{2} R_2$
- Baris $3 \rightarrow R_3=R_3+\frac{5}{2} R_2$



#### Langkah 1: Menghitung Baris 1 Baru
Setiap elemen di baris 1 dikurangi $\frac{3}{2} \times$ baris 2 .

$$
\begin{array}{|l|l|l|l|}
\hline Elemen & Nilai Lama \left(R_1\right) & \frac{3}{2} \times R_2 & Hasil Baru \left(R_1-\frac{3}{2} R_2\right) \\
\hline(1,1) & 1 & \frac{3}{2} \times 0=0 & 1-0=1 \\
\hline(1,2) & \frac{3}{2} & \frac{3}{2} \times 1=\frac{3}{2} & \frac{3}{2}-\frac{3}{2}=0 \\
\hline(1,3) & -\frac{1}{2} & \frac{3}{2} \times-\frac{9}{5}=-\frac{27}{10} & -\frac{1}{2}-\left(-\frac{27}{10}\right)=-\frac{5}{10}+\frac{27}{10}=\frac{22}{10}=\frac{11}{5} \\
\hline(1,4) & \frac{1}{2} & \frac{3}{2} \times \frac{1}{5}=\frac{3}{10} & \frac{1}{2}-\frac{3}{10}=\frac{5}{10}-\frac{3}{10}=\frac{2}{10}=\frac{1}{5} \\
\hline(1,5) & 0 & \frac{3}{2} \times-\frac{2}{5}=-\frac{6}{10} & $0-\left(-\frac{6}{10}\right)=\frac{6}{10}=\frac{3}{5} \\
\hline(1,6) & 0 & \frac{3}{2} \times 0=0 & 0-0=0 \\
\hline
\end{array}
$$

Hasil baris 1 baru:

$$
\left(1,0, \frac{11}{5}, \frac{1}{5}, \frac{3}{5}, 0\right)
$$

#### Langkah 2: Perhitungan Baris 3 Baru

Setiap elemen di baris 3 ditambah $\frac{5}{2} \times$ baris 2 .

$$
\begin{array}{|l|l|l|l|}
\hline Elemen & Nilai Lama \left(R_3\right) & \frac{5}{2} \times R_2 & Hasil Baru \left(R_3+\frac{5}{2} R_2\right) \\
\hline(3,1) & 0 & \frac{5}{2} \times 0=0 & 0+0=0 \\
\hline(3,2) & -\frac{5}{2} & \frac{5}{2} \times 1=\frac{5}{2} & -\frac{5}{2}+\frac{5}{2}=0 \\
\hline(3,3) & \frac{13}{2} & \frac{5}{2} \times-\frac{9}{5}=-\frac{45}{10}=-\frac{9}{2} & \frac{13}{2}-\frac{9}{2}=\frac{4}{2}=2 \\
\hline(3,4) & -\frac{3}{2} & \frac{5}{2} \times \frac{1}{5}=\frac{5}{10}=\frac{1}{2} & -\frac{3}{2}+\frac{1}{2}=-\frac{2}{2}=-1 \\
\hline(3,5) & 0 & \frac{5}{2} \times-\frac{2}{5}=-\frac{10}{10}=-1 & 0-1=-1 \\
\hline(3,6) & 1 & \frac{5}{2} \times 0=0 & 1+0=1 \\
\hline
\end{array}
$$

Hasil baris 3 baru:
$
(0,0,2 \mid-1,-1,1)
$

Hasil matriks:

$$
\left[\begin{array}{ccc|ccc}1 & 0 & \frac{11}{5} & \frac{1}{5} & \frac{3}{5} & 0 \\ 0 & 1 & -\frac{9}{5} & \frac{1}{5} & -\frac{2}{5} & 0 \\ 0 & 0 & 2 & -1 & -1 & 1\end{array}\right]
$$
### 7. Membuat Elemen (3,3) Menjadi 1 

Agar elemen $(3,3)$ menjadi 1. kita bagi baris ketiga dengan ${2}$ : 

$$
R_3 \rightarrow \frac{1}{2} R_3
$$

Sekarang kita bagi setiap elemen di baris 3 dengan 2:

$$
\begin{array}{|l|l|l|l|}
\hline Elemen & Nilai Lama \left(R_3\right) & Dibagi 2 & Hasil Baru \\
\hline(3,1) & 0 & 0 \div 2 & 0 \\
\hline(3,2) & 0 & 0 \div 2 & 0 \\
\hline(3,3) & 2 & 2 \div 2 & 1 \\
\hline(3,4) & -1 & -1 \div 2 & -\frac{1}{2} \\
\hline(3,5) & -1 & -1 \div 2 & -\frac{1}{2} \\
\hline(3,6) & 1 & 1 \div 2 & \frac{1}{2} \\
\hline
\end{array}
$$

Hasil baris 3 baru:
$
\left(0,0,1,-\frac{1}{2},-\frac{1}{2}, \frac{1}{2}\right)
$

Hasil matriks:
$
\left[\begin{array}{ccc|ccc}1 & 0 & \frac{11}{5} & \frac{1}{5} & \frac{3}{5} & 0 \\ 0 & 1 & -\frac{9}{5} & \frac{1}{5} & -\frac{2}{5} & 0 \\ 0 & 0 & 1 & -\frac{1}{2} & -\frac{1}{2} & \frac{1}{2}\end{array}\right]
$

### 8. Menghilangkan Elemen di Kolom 3 (Baris 1 dan 2)

Sekarang kita ingin **mengubah elemen (1,3) dan (2,3) menjadi 0**, yaitu:
- **(1,3) = $\frac{11}{5}$ → harus menjadi 0**
- **(2,3) = $-\frac{9}{5}$ → harus menjadi 0**


#### Langkah 1: Menghitung Baris 1 Baru
Operasi yang dilakukan:
$R_1=R_1-\frac{11}{5} R_3$

Sekarang kita hitung **elemen-elemen baru pada $( R_1)$**:

$$
\begin{array}{|l|l|l|l|}
\hline Elemen & Nilai Lama \left(R_1\right) & \frac{11}{5} \times R_3 & Hasil Baru \left(R_1-\frac{11}{5} R_3\right) \\
\hline(1,1) & 1 & \frac{11}{5} \times 0=0 & 1-0=1 \\
\hline(1,2) & 0 & \frac{11}{5} \times 0=0 & 0-0=0 \\
\hline(1,3) & \frac{11}{5} & \frac{11}{5} \times 1=\frac{11}{5} & \frac{11}{5}-\frac{11}{5}=0 \\
\hline(1,4) & \frac{1}{5} & \frac{11}{5} \times-\frac{1}{2}=-\frac{11}{10} & \frac{1}{5}-\left(-\frac{11}{10}\right)=\frac{2}{10}+\frac{11}{10}=\frac{13}{10} \\
\hline(1,5) & \frac{3}{5} & \frac{11}{5} \times-\frac{1}{2}=-\frac{11}{10} & \frac{3}{5}-\left(-\frac{11}{10}\right)=\frac{6}{10}+\frac{11}{10}=\frac{17}{10} \\
\hline(1,6) & 0 & \frac{11}{5} \times \frac{1}{2}=\frac{11}{10} & $0-\frac{11}{10}=-\frac{11}{10} \\
\hline
\end{array}
$$

Jadi, **baris 1 baru** menjadi:

$$
\left( 1, 0, 0, \frac{13}{10}, \frac{17}{10}, -\frac{11}{10} \right)
$$


#### Langkah 2: Menghitung Baris 2 Baru
Operasi yang dilakukan:  
$
R_2 = R_2 + \frac{9}{5} R_3
$

Sekarang kita hitung **elemen-elemen baru pada $( R_2 )$**:

$$
\begin{array}{|l|l|l|l|}
\hline Elemen & Nilai Lama \left(R_2\right) & \frac{9}{5} \times R_3 & Hasil Baru \left(R_2+\frac{9}{5} R_3\right) \\
\hline(2,1) & 0 & \frac{9}{5} \times 0=0 & 0+0=0 \\
\hline(2,2) & 1 & \frac{9}{5} \times 0=0 & 1+0=1 \\
\hline(2,3) & -\frac{9}{5} & \frac{9}{5} \times 1=\frac{9}{5} & -\frac{9}{5}+\frac{9}{5}=0 \\
\hline(2,4) & \frac{1}{5} & \frac{9}{5} \times-\frac{1}{2}=-\frac{9}{10} & \frac{1}{5}-\frac{9}{10}=\frac{2}{10}-\frac{9}{10}=-\frac{7}{10} \\
\hline(2,5) & -\frac{2}{5} & \frac{9}{5} \times-\frac{1}{2}=-\frac{9}{10} & -\frac{2}{5}-\left(-\frac{9}{10}\right)=-\frac{4}{10}+\frac{9}{10}=\frac{5}{10}=\frac{1}{2} \\
\hline(2,6) & 0 & \frac{9}{5} \times \frac{1}{2}=\frac{9}{10} & $0+\frac{9}{10}=\frac{9}{10} \\
\hline
\end{array}
$$
Jadi, **baris 2 baru** menjadi:

$$
\left( 0, 1, 0, -\frac{7}{10}, \frac{1}{2}, \frac{9}{10} \right)
$$

Hasil akhir matriks:

$$
\left[
\begin{array}{ccc|ccc}
1 & 0 & 0 & \frac{13}{10} & \frac{17}{10} & -\frac{11}{10} \\
0 & 1 & 0 & -\frac{7}{10} & \frac{1}{2} & \frac{9}{10} \\
0 & 0 & 1 & -\frac{1}{2} & -\frac{1}{2} & \frac{1}{2}
\end{array}
\right]
$$

solusi dari sistem persamaan linear
$ AX = B $$
$$ A^{-1} AX = A^{-1} B$$
$$ IX = A^{-1} B$$
$$ X = A^{-1} B$

## MATRIKS 4 PERSAMAAN

Sistem persamaannya adalah:
$
\begin{cases}
2x_1 - x_2 + 3x_3 + 4x_4 = 2 \\
x_1 - 2x_3 + 5x_4 = 1 \\
4x_1 + 2x_2 + x_3 - 3x_4 = 4 \\
3x_2 - x_3 + 2x_4 = 0
\end{cases}
$

---

### 1. Diketahui matriks \( A \):

$$
A =
\begin{bmatrix} 
2 & -1 & 3 & 4 \\ 
1 & 0 & -2 & 5 \\ 
4 & 2 & 1 & -3 \\ 
0 & 3 & -1 & 2 
\end{bmatrix}
$$

Untuk mencari invers, kita buat **matriks augmented** dengan menyisipkan **matriks identitas \( I \) di sebelah kanan \( A \)**:

$$
(A | I) =
\begin{bmatrix} 
2 & -1 & 3 & 4 & | 1 & 0 & 0 & 0 \\ 
1 & 0 & -2 & 5 & | 0 & 1 & 0 & 0 \\ 
4 & 2 & 1 & -3 & | 0 & 0 & 1 & 0 \\ 
0 & 3 & -1 & 2 & | 0 & 0 & 0 & 1 
\end{bmatrix}
$$

**Tujuan:**  
Ubah $A$ menjadi **matriks identitas** menggunakan **operasi baris**, dan perubahan yang sama diterapkan ke bagian kanan agar kita mendapatkan $A^{-1}$


---

### 2. Buat Elemen (1,1) Menjadi 1
Saat ini elemen $(1,1)$ adalah **2**, maka kita bagi seluruh **baris pertama** dengan **2** supaya menjadi **1**.

$$
R_1 \leftarrow \frac{1}{2} R_1
$$

$$
\begin{bmatrix} 
1 & -0.5 & 1.5 & 2 & | 0.5 & 0 & 0 & 0 \\ 
1 & 0 & -2 & 5 & | 0 & 1 & 0 & 0 \\ 
4 & 2 & 1 & -3 & | 0 & 0 & 1 & 0 \\ 
0 & 3 & -1 & 2 & | 0 & 0 & 0 & 1 
\end{bmatrix}
$$

---

### 3. Buat Elemen di Kolom Pertama (Kecuali (1,1)) Menjadi Nol
Kita ingin membuat elemen di bawah **1** di kolom pertama menjadi **nol**.

Gunakan operasi:

- $ R_2 \leftarrow R_2 - R_1 $ (Nol pada (2,1))
- $ R_3 \leftarrow R_3 - 4R_1 $ (Nol pada (3,1))

$$\begin{bmatrix} 
1 & -0.5 & 1.5 & 2 & | 0.5 & 0 & 0 & 0 \\ 
0 & 0.5 & -3.5 & 3 & | -0.5 & 1 & 0 & 0 \\ 
0 & 4 & -5 & -11 & | -2 & 0 & 1 & 0 \\ 
0 & 3 & -1 & 2 & | 0 & 0 & 0 & 1 
\end{bmatrix}
$$


---

### 4. Buat Elemen $(2,2)$ Menjadi 1
Saat ini elemen (2,2) adalah **0.5**, maka kita bagi **baris kedua** dengan **0.5**.

$$
R_2 \leftarrow 2 R_2
$$

$$
\begin{bmatrix} 
1 & -0.5 & 1.5 & 2 & | 0.5 & 0 & 0 & 0 \\ 
0 & 1 & -7 & 6 & | -1 & 2 & 0 & 0 \\ 
0 & 4 & -5 & -11 & | -2 & 0 & 1 & 0 \\ 
0 & 3 & -1 & 2 & | 0 & 0 & 0 & 1 
\end{bmatrix}
$$

---

### 5. Buat Elemen di Kolom Kedua (Kecuali (2,2)) Menjadi Nol
Gunakan operasi:

- $ R_3 \leftarrow R_3 - 4 R_2 $ (Nol pada (3,2))
- $ R_4 \leftarrow R_4 - 3 R_2 $ (Nol pada (4,2))

$$
\begin{bmatrix} 
1 & 0 & -2 & 5 & | 0 & 1 & 0 & 0 \\ 
0 & 1 & -7 & 6 & | -1 & 2 & 0 & 0 \\ 
0 & 0 & 23 & -35 & | 2 & -8 & 1 & 0 \\ 
0 & 0 & 20 & -16 & | 3 & -6 & 0 & 1 
\end{bmatrix}
$$

---


### 6. Buat Elemen $(3,3)$ Menjadi 1
Saat ini elemen $(3,3)$ adalah **23**, maka kita bagi **baris ketiga** dengan **23**.

$$
R_3 \leftarrow \frac{1}{23} R_3
$$

$$
\begin{bmatrix} 
1 & 0 & -2 & 5 & | 0 & 1 & 0 & 0 \\ 
0 & 1 & -7 & 6 & | -1 & 2 & 0 & 0 \\ 
0 & 0 & 1 & -\frac{35}{23} & | \frac{2}{23} & -\frac{8}{23} & \frac{1}{23} & 0 \\ 
0 & 0 & 20 & -16 & | 3 & -6 & 0 & 1 
\end{bmatrix}
$$

---

### 7. Buat Elemen di Kolom Ketiga (Kecuali (3,3)) Menjadi Nol
Gunakan operasi:

- $ R_4 \leftarrow R_4 - 20 R_3 $ (Nol pada (4,3))

$$
\begin{bmatrix} 
1 & 0 & -2 & 5 & | 0 & 1 & 0 & 0 \\ 
0 & 1 & -7 & 6 & | -1 & 2 & 0 & 0 \\ 
0 & 0 & 1 & -\frac{35}{23} & | \frac{2}{23} & -\frac{8}{23} & \frac{1}{23} & 0 \\ 
0 & 0 & 0 & 13.57 & | 2.26 & -4.04 & -0.87 & 1 
\end{bmatrix}
$$

---

#### 8. Buat Elemen $(4,4)$ Menjadi 1
Saat ini elemen di posisi (4,4) adalah **13.57**.  
Agar menjadi **1**, kita bagi seluruh baris ke-4 dengan **13.57**.

$$
R_4 \leftarrow \frac{1}{13.57} R_4
$$

Setelah pembagian:

$$
\begin{bmatrix} 
1 & 0 & -2 & 5 & | 0 & 1 & 0 & 0 \\ 
0 & 1 & -7 & 6 & | -1 & 2 & 0 & 0 \\ 
0 & 0 & 1 & -\frac{35}{23} & | \frac{2}{23} & -\frac{8}{23} & \frac{1}{23} & 0 \\ 
0 & 0 & 0 & 1 & | 0.1665 & -0.2976 & -0.0641 & 0.0737 
\end{bmatrix}
$$

---

#### 9. Buat Elemen $(1,4)$, $(2,4)$, dan $(3,4)$ Menjadi Nol
Agar elemen selain (4,4) di kolom ke-4 menjadi **0**, kita lakukan:

- $$ R_1 \leftarrow R_1 - 5 R_4 $$  
- $$ R_2 \leftarrow R_2 - 6 R_4 $$  
- $$ R_3 \leftarrow R_3 + \frac{35}{23} R_4 $$  

Setelah operasi ini:

$$
\begin{bmatrix} 
1 & 0 & -2 & 0 & | -0.8325 & 2.488 & 0.3205 & -0.3685 \\ 
0 & 1 & -7 & 0 & | 0.0006 & 3.7856 & 0.3846 & -0.4422 \\ 
0 & 0 & 1 & 0 & | 0.2475 & -0.1167 & -0.0591 & 0.1121 \\ 
0 & 0 & 0 & 1 & | 0.1665 & -0.2976 & -0.0641 & 0.0737 
\end{bmatrix}
$$

---

#### 10. Buat Elemen $(1,3)$ dan $(2,3)$ Menjadi Nol
Agar elemen selain (3,3) di kolom ke-3 menjadi **0**, kita lakukan:

- $$ R_1 \leftarrow R_1 + 2 R_3 $$  
- $$ R_2 \leftarrow R_2 + 7 R_3 $$  

Setelah operasi ini:

$$
\begin{bmatrix} 
1 & 0 & 0 & 0 & | -0.3375 & 2.2546 & 0.2023 & -0.1443 \\ 
0 & 1 & 0 & 0 & | 1.7314 & 3.9645 & 0.6353 & -0.6585 \\ 
0 & 0 & 1 & 0 & | 0.2475 & -0.1167 & -0.0591 & 0.1121 \\ 
0 & 0 & 0 & 1 & | 0.1665 & -0.2976 & -0.0641 & 0.0737 
\end{bmatrix}
$$

Sekarang **bagian kiri matriks sudah menjadi identitas**, sehingga **bagian kanan adalah invers**.
$
A^{-1} =
\begin{bmatrix} 
-0.3375 & 2.2546 & 0.2023 & -0.1443 \\ 
1.7314 & 3.9645 & 0.6353 & -0.6585 \\ 
0.2475 & -0.1167 & -0.0591 & 0.1121 \\ 
0.1665 & -0.2976 & -0.0641 & 0.0737 
\end{bmatrix}
$

---

### 11. Kalikan Baris $A^{-1}$ dengan  $B$
Perkalian matriks dilakukan sebagai berikut:

$$
X = A^{-1} \cdot B
$$

Maka komponennya adalah:

$$
x_1 = (-0.3375 \times 2) + (2.2546 \times 1) + (0.2023 \times 4) + (-0.1443 \times 0)
$$

$$
x_2 = (1.7314 \times 2) + (3.9645 \times 1) + (0.6353 \times 4) + (-0.6585 \times 0)
$$

$$
x_3 = (0.2475 \times 2) + (-0.1167 \times 1) + (-0.0591 \times 4) + (0.1121 \times 0)
$$

$$
x_4 = (0.1665 \times 2) + (-0.2976 \times 1) + (-0.0641 \times 4) + (0.0737 \times 0)
$$

---

#### 12. Hitung Setiap Komponen
Hitung nilai setiap $X_i$:

$$
x_1 = (-0.675) + (2.2546) + (0.8092) + (0) = 2.3888
$$

$$
x_2 = (3.4628) + (3.9645) + (2.5412) + (0) = 9.9685
$$

$$
x_3 = (0.495) + (-0.1167) + (-0.2364) + (0) = 0.1419
$$

$$
x_4 = (0.333) + (-0.2976) + (-0.2564) + (0) = -0.221
$$

---

### 13. Tuliskan hasil perkalian:

$$
X =
\begin{bmatrix} 
2.3888 \\ 
9.9685 \\ 
0.1419 \\ 
-0.221 
\end{bmatrix}
$$

Jadi, **hasil akhirnya adalah**:

$$
X =
\begin{bmatrix} 
2.39 \\ 
9.97 \\ 
0.14 \\ 
-0.22 
\end{bmatrix}
$$

