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
## MATRIK 3 PERSAMAAN

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


$$\begin{array}{|l|l|l|l|}
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

$$\begin{array}{|l|l|l|l|}
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

$$\begin{array}{|l|l|l|l|}
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

$$\begin{array}{|l|l|l|l|}
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

$$\begin{array}{|l|l|l|l|}
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


