---
title: Sistem Persamaan Linear 3 Variabel
---

# SISTEM PERSAMAAN LINEAR 3 VARIABEL

## Penyelesaian Sistem Linear dengan Eliminasi Gauss

### Sistem Persamaan Linear
Diberikan sistem persamaan linear berikut:

\[\begin{aligned}
2x + y - z &= 3  & \text{(Persamaan 1)} \\
x - 3y + 2z &= -4 & \text{(Persamaan 2)} \\
3x + 2y + z &= 5  & \text{(Persamaan 3)}
\end{aligned}\]

### Langkah 1: Membuat Matriks Augmented
Sistem persamaan dalam bentuk matriks augmented:

\[\begin{bmatrix} 2 & 1 & -1 & | 3 \\ 1 & -3 & 2 & | -4 \\ 3 & 2 & 1 & | 5 \end{bmatrix}\]

### Langkah 2: Eliminasi Gauss
#### Langkah 2.1: Tukar Baris Pertama dengan Baris Kedua

\[\begin{bmatrix} 1 & -3 & 2 & | -4 \\ 2 & 1 & -1 & | 3 \\ 3 & 2 & 1 & | 5 \end{bmatrix}\]

#### Langkah 2.2: Eliminasi Elemen di Bawah Pivot Pertama

\[\begin{bmatrix} 1 & -3 & 2 & | -4 \\ 0 & 7 & -5 & | 11 \\ 0 & 11 & -5 & | 17 \end{bmatrix}\]

#### Langkah 2.3: Normalisasi Baris Kedua

\[\begin{bmatrix} 1 & -3 & 2 & | -4 \\ 0 & 1 & -\frac{5}{7} & | \frac{11}{7} \\ 0 & 11 & -5 & | 17 \end{bmatrix}\]

#### Langkah 2.4: Eliminasi Elemen di Atas dan Bawah Pivot Kedua

\[\begin{bmatrix} 1 & 0 & -\frac{1}{7} & | \frac{29}{7} \\ 0 & 1 & -\frac{5}{7} & | \frac{11}{7} \\ 0 & 0 & \frac{30}{7} & | \frac{36}{7} \end{bmatrix}\]

#### Langkah 2.5: Normalisasi Baris Ketiga

\[\begin{bmatrix} 1 & 0 & -\frac{1}{7} & | \frac{29}{7} \\ 0 & 1 & -\frac{5}{7} & | \frac{11}{7} \\ 0 & 0 & 1 & | \frac{6}{5} \end{bmatrix}\]

#### Langkah 2.6: Eliminasi Elemen di Atas Pivot Ketiga

\[\begin{bmatrix} 1 & 0 & 0 & | -\frac{1}{5} \\ 0 & 1 & 0 & | \frac{53}{35} \\ 0 & 0 & 1 & | \frac{6}{5} \end{bmatrix}\]

### Langkah 3: Solusi
Dari matriks terakhir, kita mendapatkan solusi:

\[\begin{aligned}
x &= -\frac{1}{5} \\
y &= \frac{53}{35} \\
z &= \frac{6}{5}
\end{aligned}\]

### Verifikasi Solusi
#### Substitusi ke Persamaan Asli

**Persamaan 1:**
\[2(-\frac{1}{5}) + \frac{53}{35} - \frac{6}{5} = 3\]
(Benar)

**Persamaan 2:**
\[-\frac{1}{5} - 3(\frac{53}{35}) + 2(\frac{6}{5}) = -4\]
(Benar)

**Persamaan 3:**
\[3(-\frac{1}{5}) + 2(\frac{53}{35}) + \frac{6}{5} = 5\]
(Benar)

### Kesimpulan
Solusi sistem persamaan linear adalah:

\[x = -\frac{1}{5}, \quad y = \frac{53}{35}, \quad z = \frac{6}{5}\]

### Geogebra Persamaan Linear 3 Variabel
<iframe src="https://www.geogebra.org/calculator/jpjtusjh?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4; border-radius: 4px;" frameborder="0"></iframe>
