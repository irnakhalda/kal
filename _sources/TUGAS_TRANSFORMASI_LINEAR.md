---
title: TUGAS_TRANSFORMASI_LINEAR

---

---
title: TUGAS_TRANSFORMASI_LINEAR

---

# TUGAS TRANSFORMASI LINEAR
## Tugas 1

buktikan bahwa $T(v1,v2)-(v1+v2,v1)$ adalah transformasi linier

Kita harus menunjukkan bahwa $T: \mathbb{R}^2 \rightarrow \mathbb{R}^2$ memenuhi dua sifat utama transformasi linier:

### **Langkah 1: Definisi transformasi linier**

Sebuah fungsi $T: \mathbb{R}^2 \rightarrow \mathbb{R}^2$ dikatakan **transformasi linier** jika untuk semua $\mathbf{u}, \mathbf{v} \in \mathbb{R}^2$ dan skalar $c \in \mathbb{R}$, berlaku:

1. **Penjumlahan:** $T(\mathbf{u} + \mathbf{v}) = T(\mathbf{u}) + T(\mathbf{v})$
2. **Perkalian skalar:** $T(c\mathbf{v}) = cT(\mathbf{v})$

---

### **Langkah 2: Misalkan $\mathbf{v} = (v_1, v_2)$, maka:**

$$
T(v_1, v_2) = (v_1 + v_2, v_1)
$$

---

### **Langkah 3: Uji Penjumlahan**

Misalkan:

$$
\mathbf{u} = (u_1, u_2), \quad \mathbf{v} = (v_1, v_2)
$$

Hitung $T(\mathbf{u} + \mathbf{v})$:

$$
\mathbf{u} + \mathbf{v} = (u_1 + v_1, u_2 + v_2)
$$

$$
T(\mathbf{u} + \mathbf{v}) = ((u_1 + v_1) + (u_2 + v_2), u_1 + v_1) = (u_1 + u_2 + v_1 + v_2, u_1 + v_1)
$$

Sekarang hitung $T(\mathbf{u}) + T(\mathbf{v})$:

$$
T(\mathbf{u}) = (u_1 + u_2, u_1), \quad T(\mathbf{v}) = (v_1 + v_2, v_1)
$$

$$
T(\mathbf{u}) + T(\mathbf{v}) = (u_1 + u_2 + v_1 + v_2, u_1 + v_1)
$$

Karena hasilnya sama, maka **sifat penjumlahan terpenuhi**.

---

### **Langkah 4: Uji Perkalian Skalar**

Misalkan $c \in \mathbb{R}$, dan $\mathbf{v} = (v_1, v_2)$

$$
c\mathbf{v} = (cv_1, cv_2)
$$

$$
T(c\mathbf{v}) = (cv_1 + cv_2, cv_1) = c(v_1 + v_2, v_1) = cT(\mathbf{v})
$$

Jadi **sifat perkalian skalar juga terpenuhi**.

---

### **Langkah 5: Representasi dalam Matriks**



Misalkan:

$$
\mathbf{v} = \begin{bmatrix} v_1 \\ v_2 \end{bmatrix}
\Rightarrow T(\mathbf{v}) = \begin{bmatrix} v_1 + v_2 \\ v_1 \end{bmatrix}
$$

Kita ingin mencari matriks $A$ sehingga:

$$
T(\mathbf{v}) = A \mathbf{v}
$$

Perhatikan:

$$
\begin{bmatrix} v_1 + v_2 \\ v_1 \end{bmatrix}
= \begin{bmatrix} 1 & 1 \\ 1 & 0 \end{bmatrix}
\begin{bmatrix} v_1 \\ v_2 \end{bmatrix}
$$

Jadi, matriks representasi dari transformasi $T$ adalah:

$$
A = \begin{bmatrix} 1 & 1 \\ 1 & 0 \end{bmatrix}
$$


---


### **Langkah 6: Kesimpulan**


 **Maka, $T$ adalah transformasi linier.**

---
## Tugas 2

### 1. Refleksi Terhadap Sumbu-X

Matriks: 

$$
M_x=\left[\begin{array}{cc}
1 & 0 \\
0 & -1
\end{array}\right]
$$

Langkah di GeoGebra:

1. Membuat titik asal:
- Ketik A $=(2,3)$ di Input Bar.

- Ketik B $=(1,-2)$ di Input Bar.

2. Membuat matriks refleksi sumbu-X: 

- Ketik $M_{-} \mathrm{x}=\{\{1,0\},\{0,-1\}\}$ di Input Bar. 

3. Hitung hasil refleksi:

- Ketik A_refleksi $=$ M_x $^2$ A $\rightarrow$ Hasil: $(2,-3)$.

- Ketik B_refleksi = M_x * B $\rightarrow$ Hasil: $(1,2)$.

4. Verifikasi:

- Plot titik asli dan hasil refleksi. Pastikan titik refleksi berada di bawah sumbu-X.

### Geogebra

<iframe src="https://www.geogebra.org/calculator/sxxcbccu?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

### 2. Refleksi Terhadap Sumbu-Y

Matriks: 

$$
M_y=\left[\begin{array}{cc}
-1 & 0 \\
0 & 1
\end{array}\right]
$$

Langkah di GeoGebra:

1. Membuat matriks refleksi sumbu-Y: 

- Ketik M_y = \{\{-1, 0\}, \{0, 1\}\} di Input Bar.

2. Hitung hasil refleksi: 

- Ketik A_refleksi $=$ M_y * A $\rightarrow$ Hasil: $(-2,3)$.

- Ketik B_refleksi $=$ M_y * B $\rightarrow$ Hasil: $(-1,-2)$. 

3. Verifikasi:

- Pastikan titik refleksi berada di sisi kiri sumbu-Y.

### Geogebra

<iframe src="https://www.geogebra.org/calculator/wud46b6v?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

### 3. Refleksi Terhadap Garis ${y}={x}$

Matriks:

$$
M_{y=x}=\left[\begin{array}{ll}
0 & 1 \\
1 & 0
\end{array}\right]
$$

Langkah di GeoGebra:

1. Membuat garis $y=x$ :

- Ketik $\mathrm{y}=\mathrm{x}$ di Input Bar. 

2. Membuat matriks refleksi:

- Ketik M_yx = \{\{0, 1\}, \{1, 0\}\}.

3. Hitung hasil refieksi:

- Ketik A_refleksi $=$ M_yx $* A \rightarrow \operatorname{Hasil}:(3,2)$.

- Ketik B_refleksi $=$ M_yx * B $\rightarrow$ Hasil: $(-2,1)$.

4. Verifikasi:

- Pastikan titik refleksi adalah pencerminan diagonal dari titik asli.

### Geogebra

<iframe src="https://www.geogebra.org/calculator/thjpw7hp?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

### 4. Refleksi Terhadap Garis $y=-x$

Matriks:

$$
M_{y=-x}=\left[\begin{array}{cc}
0 & -1 \\
-1 & 0
\end{array}\right]
$$

Langkah di GeoGebra:

1. Membuat garis $y=-x$ : 

- Ketik y = -x di Input Bar.

2. Membuat matriks refleksi:

- Ketik M_ynx $=\{\{0,-1\},\{-1,0\}\}$

3. Hitung hasil refleksi:
4.
- Ketik A_refleksi $=$ M_ynx * $A \rightarrow$ Hasil: $(-3,-2)$.

- Ketik B_refleksi $=$ M_ynx * B $\rightarrow$ Hasil: $(2,-1)$.

4. Verifikasi: 

- Pastikan titik refleksi berada di kuadran berlawanan dari garis $y=-x$.

### Geogebra

<iframe src="https://www.geogebra.org/calculator/phk6u7gm?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

### 5. Refleksi Terhadap Titik Asal (Origin)

Matriks: 

$$
M_{\text {origin }}=\left[\begin{array}{cc}
-1 & 0 \\
0 & -1
\end{array}\right]
$$

Langkah di GeoGebra:
1. Membuat matriks refleksi origin:

- Ketik M_origin $=\{\{-1,0\},\{0,-1\}\}$.

2. Hitung hasil refieksi:

- Ketik A_refleksi $=$ M_origin * $A \rightarrow \operatorname{Hasil}:(-2,-3)$.

- Ketik B_refleksi $=$ M_origin * B $\rightarrow \operatorname{Hasil}:(-1,2)$.

3. Verifikasi:

- Pastikan titik refleksi berlawanan arah dari titik asli terhadap origin.

### Geogebra

<iframe src="https://www.geogebra.org/calculator/yjnjv8b5?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>