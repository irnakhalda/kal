---
title: sistem_persamaan_3variabel

---

# SISTEM PERSAMAAN LINEAR 3 VARIABEL

---

## Penyelesaian Sistem Linear dengan Eliminasi Gauss
### Sistem Persamaan Linear
Diberikan sistem persamaan linear berikut:
\[
\begin{align*}
2x + y - z &= 3  & \text{(Persamaan 1)} \\
x - 3y + 2z &= -4 & \text{(Persamaan 2)} \\
3x + 2y + z &= 5  & \text{(Persamaan 3)}
\end{align*}
\]

### **Langkah 1: Membuat Matriks Augmented**
\[
\begin{align*}
\left[
\begin{array}{ccc|c}
2 & 1 & -1 & 3 \\
1 & -3 & 2 & -4 \\
3 & 2 & 1 & 5
\end{array}
\right]
\end{align*}
\]

### **Langkah 2: Eliminasi Gauss**
**Langkah 2.1: Membuat elemen pertama pada baris pertama menjadi 1.**
\[
\begin{align*}
\left[
\begin{array}{ccc|c}
1 & -3 & 2 & -4 \\
2 & 1 & -1 & 3 \\
3 & 2 & 1 & 5
\end{array}
\right]
\end{align*}
\]

**Langkah 2.2: Eliminasi elemen di bawah pivot pertama.**
\[
\begin{align*}
R_2 &= R_2 - 2R_1 \\
R_3 &= R_3 - 3R_1
\end{align*}
\]

Hasil:
\[
\begin{align*}
\left[
\begin{array}{ccc|c}
1 & -3 & 2 & -4 \\
0 & 7 & -5 & 11 \\
0 & 11 & -5 & 17
\end{array}
\right]
\end{align*}
\]

**Langkah 2.3: Membuat elemen kedua pada baris kedua menjadi 1.**
\[
\begin{align*}
R_2 &= \frac{1}{7} R_2
\end{align*}
\]

Hasil:
\[
\begin{align*}
\left[
\begin{array}{ccc|c}
1 & -3 & 2 & -4 \\
0 & 1 & -\frac{5}{7} & \frac{11}{7} \\
0 & 11 & -5 & 17
\end{array}
\right]
\end{align*}
\]

**Langkah 2.4: Eliminasi elemen di atas dan di bawah pivot kedua.**
\[
\begin{align*}
R_1 &= R_1 + 3R_2 \\
R_3 &= R_3 - 11R_2
\end{align*}
\]

Hasil:
\[
\begin{align*}
\left[
\begin{array}{ccc|c}
1 & 0 & -\frac{1}{7} & \frac{29}{7} \\
0 & 1 & -\frac{5}{7} & \frac{11}{7} \\
0 & 0 & \frac{30}{7} & \frac{36}{7}
\end{array}
\right]
\end{align*}
\]

**Langkah 2.5: Membuat elemen ketiga pada baris ketiga menjadi 1.**
\[
\begin{align*}
R_3 &= \frac{1}{\frac{30}{7}} R_3
\end{align*}
\]

Hasil:
\[
\begin{align*}
\left[
\begin{array}{ccc|c}
1 & 0 & -\frac{1}{7} & \frac{29}{7} \\
0 & 1 & -\frac{5}{7} & \frac{11}{7} \\
0 & 0 & 1 & \frac{6}{5}
\end{array}
\right]
\end{align*}
\]

**Langkah 2.6: Eliminasi elemen di atas pivot ketiga.**
\[
\begin{align*}
R_1 &= R_1 + \frac{1}{7}R_3 \\
R_2 &= R_2 + \frac{5}{7}R_3
\end{align*}
\]

Hasil:
\[
\begin{align*}
\left[
\begin{array}{ccc|c}
1 & 0 & 0 & -\frac{1}{5} \\
0 & 1 & 0 & \frac{53}{35} \\
0 & 0 & 1 & \frac{6}{5}
\end{array}
\right]
\end{align*}
\]

### **Langkah 3: Solusi**
\[
\begin{align*}
x &= -\frac{1}{5} \\
y &= \frac{53}{35} \\
z &= \frac{6}{5}
\end{align*}
\]

### **Verifikasi Solusi**
Substitusikan ke persamaan awal:

1. **Persamaan 1:**
\[
\begin{align*}
2(-\frac{1}{5}) + \frac{53}{35} - \frac{6}{5} &= 3 \\
-\frac{2}{5} + \frac{53}{35} - \frac{42}{35} &= 3 \\
\frac{53 - 42 - 14}{35} &= 3 \\
3 &= 3
\end{align*}
\]

2. **Persamaan 2:**
\[
\begin{align*}
-\frac{1}{5} - 3(\frac{53}{35}) + 2(\frac{6}{5}) &= -4 \\
-\frac{1}{5} - \frac{159}{35} + \frac{12}{5} &= -4 \\
-\frac{7}{35} - \frac{159}{35} + \frac{84}{35} &= -4 \\
-\frac{159 - 7 + 84}{35} &= -4 \\
-4 &= -4
\end{align*}
\]

3. **Persamaan 3:**
\[
\begin{align*}
3(-\frac{1}{5}) + 2(\frac{53}{35}) + \frac{6}{5} &= 5 \\
-\frac{3}{5} + \frac{106}{35} + \frac{6}{5} &= 5 \\
-\frac{21}{35} + \frac{106}{35} + \frac{42}{35} &= 5 \\
\frac{106 - 21 + 42}{35} &= 5 \\
5 &= 5
\end{align*}
\]

### **Kesimpulan**
\[
\begin{align*}
x &= -\frac{1}{5}, \quad y = \frac{53}{35}, \quad z = \frac{6}{5}
\end{align*}
\]


### Geogebra Persamaan Linear dengan 3
<iframe src="https://www.geogebra.org/calculator/jpjtusjh?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>