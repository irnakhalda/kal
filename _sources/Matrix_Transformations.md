---
title: Matrix_Transformations

---

---
title: Matrix_Transformations

---

# Matrix Transformations

Kombinasi bentuk perkalian dan translasi untuk transformasi geometri 2D ke
dalam suatu matriks dilakukan dengan mengubah matriks 2 x 2 menjadi
matriks 3 x 3.
Untuk itu maka koordinat cartesian (x,y) dinyatakan dalam bentuk koordinat
homogen (xh, yh, h), dimana :
x = xh / h y = yh / h
Dimana untuk geometri 2D parameter h ≠ 0 atau biasanya h = 1, sehingga
setiap posisi koordinat 2D dapat dinyatakan dengan (x, y, 1).
Untuk transformasi 3D biasanya parameter h ≠ 1.Dengan menyatakan posisi titik dalam koordinat homogen, semua transformasi geometri dinyatakan dalam bentuk matriks. Koordinat dinyatakan dalam tiga elemen vektor kolom dan operasi transformasi ditulis dengan matriks 3 x 3.

## A1. Matriks Translasi

$$
\left[\begin{array}{l}
x^{\prime} \\
y^{\prime} \\
1
\end{array}\right]=\left[\begin{array}{lll}
1 & 0 & t_x \\
0 & 1 & t_y \\
0 & 0 & 1
\end{array}\right] \cdot\left[\begin{array}{c}
x \\
y \\
1
\end{array}\right] \quad \text { atau } \quad P^{\prime}=T\left(t_x, t_y\right) \cdot P
$$

## A2. Matriks Rotasi

$$
\left[\begin{array}{c}
x^{\prime} \\
y^{\prime} \\
1
\end{array}\right]=\left[\begin{array}{ccc}
\cos \theta & -\sin \theta & 0 \\
\sin \theta & \cos \theta & 0 \\
0 & 0 & 1
\end{array}\right] \cdot\left[\begin{array}{l}
\mathrm{x} \\
\mathrm{y} \\
1
\end{array}\right] \quad \text { atau } \quad \mathbf{P}^{\prime}=\mathbf{R}({\theta}) \cdot \mathbf{P}
$$

## A3. Matriks Skala

$$
\left[\begin{array}{l}
x^{\prime} \\
y^{\prime} \\
1
\end{array}\right]=\left[\begin{array}{ccc}
s_x & 0 & 0 \\
0 & s_y & 0 \\
0 & 0 & 1
\end{array}\right] \cdot\left[\begin{array}{l}
x \\
y \\
1
\end{array}\right]
$$

atau $\quad P^{\prime}=\mathbf{S}\left(S_x, S_y\right) \cdot P$

## B. Matriks Transformasi Komposit (Gabungan)

Dengan bentuk matriks seperti yang telah dibahas sebelumnya, setiap urutan transformasi dapat dibuat sebagai matriks transformasi komposit dengan menghitung produk matriks transformasi individu.
Bentuk matriks transformasi komposit diperoleh dengan melakukan perkalian matriks dari kanan ke kiri :

### B1. Translasi
Bila dua vektor translasi masing-masing ( $\mathrm{t}_{x 1}, \mathrm{t}_{\mathrm{y} 1}$ ) dan ( $\mathrm{t}_{\mathrm{x} 2}, \mathrm{t}_{\mathrm{y} 2}$ ) digunakan pada posisi koordinat P , maka transformasi akhir $\mathrm{P}^{\prime}$ dapat dihitung dengan:

$$
\begin{aligned}
P^{\prime}= & T\left(t_x 2, t_y 2\right) \cdot\left\{T\left(t_x 1, t_y 1\right) \cdot P\right\} \\
& \left\{T\left(t_x, t_y\right) \cdot T\left(t_{x 1}, t_{y 1}\right)\right\} . P
\end{aligned}
$$

Dimana:
P dan P' : Vektor kolom koordinat homogen

Dalam bentuk matriks:

$$
\left[\begin{array}{ccc}
1 & 0 & t_{\mathrm{x} 2} \\
0 & 1 & \mathrm{t}_{\mathrm{y} 2} \\
0 & 0 & 1
\end{array}\right] \cdot\left[\begin{array}{ccc}
1 & 0 & \mathrm{t}_{\mathrm{x} 1} \\
0 & 1 & \mathrm{t}_{\mathrm{y} 1} \\
0 & 0 & 1
\end{array}\right]=\left[\begin{array}{ccc}
1 & 0 & \mathrm{t}_{\mathrm{x} 1}+\mathrm{t}_{\mathrm{x} 2} \\
0 & 1 & \mathrm{t}_{\mathrm{y} 1}+\mathrm{t}_{\mathrm{y} 2} \\
0 & 0 & 1
\end{array}\right]
$$

atau

$$
T\left(t_x, t_y\right) \cdot T\left(t_{x 1}, t_y\right)=T\left(t_{x 1}+t_{x 2}, t_{y 1}+t_y\right)
$$

### B2. Scaling
Bila operasi penskalaan dilakukan sebanyak dua kali, maka akan menghasilkan matriks skala komposit sebagai berikut:

$$
\left[\begin{array}{ccc}
\mathrm{s}_{\mathrm{x} 2} & 0 & 0 \\
0 & \mathrm{~s}_{\mathrm{y} 2} & 0 \\
0 & 0 & 1
\end{array}\right] \cdot\left[\begin{array}{ccc}
\mathrm{s}_{\mathrm{x} 1} & 0 & 0 \\
0 & \mathrm{~s}_{\mathrm{y} 1} & 0 \\
0 & 0 & 1
\end{array}\right]=\left[\begin{array}{ccc}
\mathrm{s}_{\mathrm{x} 1} \cdot \mathrm{~s}_{\mathrm{x} 2} & 0 & 0 \\
0 & \mathrm{~s}_{\mathrm{y} 1} \cdot \mathrm{~s}_{\mathrm{y} 2} & 0 \\
0 & 0 & 1
\end{array}\right]
$$

atau

$$
\mathbf{S}\left(S_{x 2}, S_{y 2}\right) \cdot S\left(S_{x 1}, S_{y 1}\right)=S\left(S_{x 1} \cdot S_{x 2}, S_{y 1} \cdot S_{y 2}\right)
$$

### B3. Rotasi
Bila rotasi dilakukan sebanyak dua kali terhadap titik P, maka posisi transformasi akhir P' dapat dinyatakan dengan:

$$
\begin{aligned}
P^{\prime}= & R\left(\theta_2\right) \cdot\left\{R\left(\theta_1\right) \cdot P\right\} \\
& \left\{R\left(\theta_2\right) \cdot R\left(\theta_1\right)\right\} \cdot P \quad \operatorname{dimana} \quad R\left(\theta_2\right) \cdot R\left(\theta_1\right)=R\left(\theta_1+\theta_2\right)
\end{aligned}
$$

Sehingga

$$
P^{\prime}=R\left(\theta_1+\theta_2\right) \cdot P
$$

### B4. Rotasi Terhadap Pivot Point
Pada paket aplikasi grafika yang hanya mampu memutar objek menurut koordinat asal, yaitu terhadap titik pusat koordinat, dapat dibuat rotasi yang dilakukan dari titik tertentu, pivot point ( $\mathrm{X} p, \mathrm{y}_{\mathrm{p}}$ ) maka proses transformasi dilakukan dengan cara translasi-rotasi-translasi, prosedurnya adalah:
1. Pindahkan objek sedemikian sehingga posisi pivot point berada pada titik pusat (0, 0).
2. Putar objek pada titik pusat.
3. Pindahkan objek dari titik pusat ke posisi semula.

![image](https://hackmd.io/_uploads/r1m6fUSCyg.png)


### B5. Scaling Terhadap Fixed Point
Proses penskalaan (scaling) terhadap sebuat titik tertentu, fixed point ( $\mathrm{x}_{\mathrm{f}}, \mathrm{y}_{\mathrm{f}}$ ) menggunakan fungsi skala adalah sebagai berikut:
1. Pindahkan objek sedemikian sehingga posisi fixed point berhimpit dengan titik pusat (0, 0).
2. Ubah skala objek pada titik pusat.
3. Pindahkan objek dari titik pusat ke posisi semula.
Bentuk matriksnya adalah:

$$
\left[\begin{array}{ccc}
1 & 0 & x_f \\
0 & 1 & y_f \\
0 & 0 & 1
\end{array}\right] \cdot\left[\begin{array}{ccc}
s_x & 0 & 0 \\
0 & s_y & 0 \\
0 & 0 & 1
\end{array}\right] \cdot\left[\begin{array}{ccc}
1 & 0 & -x_f \\
0 & 1 & -y_f \\
0 & 0 & 1
\end{array}\right]=\left[\begin{array}{ccc}
s_x & 0 & x_f\left(1-s_x\right) \\
0 & s_y & y_f\left(1-s_y\right) \\
0 & 0 & 1
\end{array}\right]
$$

atau dapat ditulis:

$$
T\left(X_f, y_f\right) \cdot S\left(S_x, S_y\right) \cdot T\left(-x_f,-y_f\right)=S\left(x_f, y_f, S_x, S_y\right)
$$

![image](https://hackmd.io/_uploads/rJ7vzLSAJe.png)

## 7. Transformasi Lain
Transformasi dasar seperti translasi, penskalaan dan rotasi merupakan
fasilitas yang dimiliki setiap Aplikasi Grafika. Beberapa paket biasanya juga
dilengkapi dengan beberapa tambahan transformasi yang berguna untuk
aplikasi tertentu.

### A. Refleksi
Refleksi adalah transformasi yang menghasilkan pencerminan citra dari suatu
objek. Citra hasil pencerminan untuk refleksi 2D dibuat relatif terhadap sumbu
refleksi dengan cara memutar objek 180 terhadap sumbu refleksi.
Sumbu refleksi dapat dipilih sembarang garis pada bidang xy.

## A1. Refleksi Terhadap Sumbu X
Refleksi terhadap sumbu $x$ (horizontal), $\mathrm{y}=0$ dinyatakan dengan matriks:

$$
\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & -1 & 0 \\
0 & 0 & 1
\end{array}\right]
$$

![image](https://hackmd.io/_uploads/rkI4fLSCyl.png)

llustrasi refleksi terhadap sumbu x

## A2. Refleksi Terhadap Sumbu y
Refleksi terhadap sumbu y (vertikal), $\mathrm{x}=0$ dinyatakan dengan matriks:

$$
\left[\begin{array}{ccc}
-1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{array}\right]
$$

![image](https://hackmd.io/_uploads/SJw4Q8HRkx.png)

## A3. Refleksi Terhadap Sumbu Tegak Lurus Bidang XY
Refleksi terhadap sumbu yang tegak lurus bidang xy dan melalui titik pusat dinyatakan dengan matriks:

$$
\left[\begin{array}{ccc}
-1 & 0 & 0 \\
0 & -1 & 0 \\
0 & 0 & 1
\end{array}\right]
$$

![image](https://hackmd.io/_uploads/HJ75QUSRkl.png)

## A4. Refleksi Terhadap Garis Diagonal Y = X
Refleksi terhadap garis diagonal, y = x dinyatakan dengan matriks:

$$
\left[\begin{array}{ccc}
0 & 1 & 0 \\
1 & 0 & 0 \\
0 & 0 & 1
\end{array}\right]
$$

![image](https://hackmd.io/_uploads/H13-VIBAyg.png)

Terhadap sumbu x
• X’ = X
• Y’ = -Y
Terhadap sumbu y
• X’ = -X
• Y’ = Y
Terhadap sumbu y = x
• X’ = Y
• Y’ = X
Terhadap sumbu y = -x
• X’ = -Y
• Y’ = -X
## SOAL LATIHAN

### **Kelompok Latihan**  
Diberikan sebuah matriks **A**. Buatlah sketsa dari **𝑥⃗**, **𝑦⃗**, **𝐴𝑥⃗**, dan **𝐴𝑦⃗** pada sumbu Kartesius yang sama, dengan:

$$
\vec{x} = \begin{bmatrix} 1 \\ 1 \end{bmatrix} \quad \text{dan} \quad \vec{y} = \begin{bmatrix} -1 \\ 2 \end{bmatrix}
$$

#### 1. 
$$
A = \begin{bmatrix} 1 & -1 \\ 2 & 3 \end{bmatrix}
$$

#### 2. 
$$
A = \begin{bmatrix} 2 & 0 \\ -1 & 3 \end{bmatrix}
$$

---

### **Langkah Pengerjaan:**

#### Soal 1:

Hitung $A\vec{x}$ dan $A\vec{y}$:

$$
A\vec{x} = \begin{bmatrix} 1 & -1 \\ 2 & 3 \end{bmatrix} \begin{bmatrix} 1 \\ 1 \end{bmatrix} = \begin{bmatrix} 1 - 1 \\ 2 + 3 \end{bmatrix} = \begin{bmatrix} 0 \\ 5 \end{bmatrix}
$$

$$
A\vec{y} = \begin{bmatrix} 1 & -1 \\ 2 & 3 \end{bmatrix} \begin{bmatrix} -1 \\ 2 \end{bmatrix} = \begin{bmatrix} -1 - 2 \\ -2 + 6 \end{bmatrix} = \begin{bmatrix} -3 \\ 4 \end{bmatrix}
$$

#### Soal 2:

*Hitung $A\vec{x}$:*

$$
A\vec{x} = \begin{bmatrix} 2 & 0 \\ -1 & 3 \end{bmatrix} \begin{bmatrix} 1 \\ 1 \end{bmatrix} = 
\begin{bmatrix} 2(1) + 0(1) \\ -1(1) + 3(1) \end{bmatrix} = 
\begin{bmatrix} 2 \\ 2 \end{bmatrix}
$$

*Hitung $A\vec{y}$:*

$$
A\vec{y} = \begin{bmatrix} 2 & 0 \\ -1 & 3 \end{bmatrix} \begin{bmatrix} -1 \\ 2 \end{bmatrix} = 
\begin{bmatrix} 2(-1) + 0(2) \\ -1(-1) + 3(2) \end{bmatrix} = 
\begin{bmatrix} -2 \\ 7 \end{bmatrix}
$$




---

#### Soal 5: 

Dari gambar, terlihat bahwa:

- Vektor (1,0) dipetakan ke vektor *(1,2)*.
- Vektor (0,1) dipetakan ke vektor *(2,3)*.

Maka matriks transformasinya adalah:

$$
A_5 = \begin{bmatrix}
1 & 2 \\
2 & 3 \\
\end{bmatrix}
$$



#### Soal 6:

Dari gambar, terlihat bahwa:

- Vektor (1,0) dipetakan ke vektor *(1,1)*.
- Vektor (0,1) dipetakan ke vektor *(-1,1)*.

Maka matriks transformasinya adalah:

$$
A_6 = \begin{bmatrix}
1 & -1 \\
1 & 1 \\
\end{bmatrix}
$$

---

