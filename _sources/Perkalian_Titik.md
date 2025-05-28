---
title: 'Perkalian_Titik '

---

# Perkalian Titik (Dot Product)
Pengertian:
Perkalian titik (dot product) adalah operasi aljabar antara dua vektor yang menghasilkan skalar (bilangan real). Operasi ini mencerminkan kesamaan arah dua vektor dan terkait dengan sudut di antara keduanya.

Rumus Dot Product
## 1. Secara Aljabar (berdasarkan komponen vektor):
- Untuk vektor 2D: $\mathbf{A}=\left(a_1, a_2\right)$ dan $\mathbf{B}=\left(b_1, b_2\right)$

$$
\mathbf{A} \cdot \mathbf{B}=a_1 \cdot b_1+a_2 \cdot b_2
$$
- Untuk vektor 3D: $\mathbf{A}=\left(a_1, a_2, a_3\right)$ dan $\mathbf{B}=\left(b_1, b_2, b_3\right)$

$$
\mathbf{A} \cdot \mathbf{B}=a_1 \cdot b_1+a_2 \cdot b_2+a_3 \cdot b_3
$$

## 2. Secara Geometri (berdasarkan sudut $\theta$ ):

$$
\mathbf{A} \cdot \mathbf{B}=\|\mathbf{A}\| \cdot\|\mathbf{B}\| \cdot \cos \theta
$$

- Jika $\theta=90^{\circ}$ (vektor tegak lurus), hasilnya nol karena $\cos 90^{\circ}=0$.

<iframe src="https://www.geogebra.org/classic/gtngavvq?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

Rumus:
Untuk dua vektor $\mathbf{A}=\left(a_1, a_2\right)$ dan $\mathbf{B}=\left(b_1, b_2\right)$ di ruang 2D:

$$
\mathbf{A} \cdot \mathbf{B}=a_1 \cdot b_1+a_2 \cdot b_2
$$

Hasilnya adalah skalar (bilangan real).

Contoh Perhitungan

## 1. Vektor $\mathbf{a}=(0,0)$ dan $\mathbf{b}=(2,1)$
 
$$
\mathbf{a} \cdot \mathbf{b}=(0)(2)+(0)(1)=0+0=0
$$

Keterangan:
- Vektor nol ( 0,0 ) selalu menghasilkan dot product = 0 dengan vektor apa pun.

## 2. Vektor $\mathbf{a}=(0,0)$ dan $\mathbf{c}=(-1,2)$

$$
\mathbf{a} \cdot \mathbf{c}=(0)(-1)+(0)(2)=0+0=0
$$

Keterangan:
o Sama seperti contoh pertama, vektor nol tidak memiliki "arah", sehingga tidak berkontribusi pada hasil dot product.
3. Vektor $\mathbf{b}=(2,1)$ dan $\mathbf{c}=(-1,2)$

$$
\mathbf{b} \cdot \mathbf{c}=(2)(-1)+(1)(2)=-2+2=0
$$

Keterangan:
- Hasil dot product 0 menandakan kedua vektor tegak lurus (sudut $\theta=90^{\circ}$ ).
- Ini karena $\cos 90^{\circ}=0$, sehingga $\mathbf{b} \cdot \mathbf{c}=\|\mathbf{b}\|\|\mathbf{c}\| \cdot \mathbf{0}=\mathbf{0}$.

<iframe src="https://www.geogebra.org/classic/xxck5z3y?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

## Geometri dari Hasil Kali Titik

1. Hubungan dengan Sudut Antara Dua Vektor
Rumus geometris dot product:

$$
\mathbf{A} \cdot \mathbf{B}=\|\mathbf{A}\| \cdot\|\mathbf{B}\| \cdot \cos \theta
$$
- ||A||: panjang vektor A,
- $\|\mathbf{B}\|$ : panjang vektor $\mathbf{B}$,
- $\theta$. sudut antara $\mathbf{A}$ dan $\mathbf{B}$.

Interpretasi:
- Jika A dan B searah ( $\theta=0^{\circ}$ ): 

$$
\mathbf{A} \cdot \mathbf{B}=\|\mathbf{A}\| \cdot\|\mathbf{B}\| \quad \text { (nilai maksimum) }
$$

- Jika A dan B berlawanan arah $\left(\theta=180^{\circ}\right)$ : 

$$
\mathbf{A} \cdot \mathbf{B}=-\|\mathbf{A}\| \cdot\|\mathbf{B}\| \quad \text { (nilai minimum) }
$$

- Jika A dan B tegak lurus $\left(\theta=90^{\circ}\right)$ : 

$$
\mathbf{A} \cdot \mathbf{B}=0 \quad\left(\text { karena } \cos 90^{\circ}=0\right)
$$

2. Proyeksi Vektor

Dot product juga merepresentasikan proyeksi vektor $\mathbf{A}$ ke arah vektor $\mathbf{B}$ (atau sebaliknya).
$$
\text { Proyelssi A ke B }=\frac{\mathbf{A} \cdot \mathbf{B}}{\|\mathbf{B}\|}
$$
- Hasil proyeksi adalah panjang vektor $\mathbf{A}$ yang "terlihat" sepanjang arah $\mathbf{B}$.

Contoh:
Misal $\mathbf{A}=(3,4)$ dan $\mathbf{B}=(1,0)$ : 

$$
A \cdot B=3 \cdot 1+4 \cdot 0=3
$$

Proyeksi A ke B: 

$$
\frac{3}{\sqrt{1^2+0^2}}=3 \quad \text { (sesuai dengan komponen } x \text { dari } \mathrm{A} \text { ). }
$$ 

3. Contoh Kasus Geometris

Berikut contoh vektor dan analisis geometrismya:
1. Vektor $\mathbf{A}=(2,1)$ dan $\mathbf{B}=(-1,2)$
o Dot Product: 

$$
A \cdot B=(2)(-1)+(1)(2)=-2+2=0
$$ 

o Interpretasi Geometris:
Hasil 0 menunjukkan kedua vektor tegak lurus ( $\theta=90^{\circ}$ ).
2. Vektor $\mathbf{C}=(3,4)$ dan $\mathbf{D}=(3,0)$
o Dot Product: 

$$
\mathbf{C} \cdot \mathbf{D}=(3)(3)+(4)(0)=9+0=9
$$

o Interpretasi Geometris:
Hasil positif menunjukkan sudut $\theta<90^{\circ}$.
3. Vektor $\mathbf{F}=(0,0)$ dan $\mathbf{F}=(2,5)$
o Dot Product: 

$$
E \cdot F=0 \cdot 2+0 \cdot 5=0
$$

o Interpretasi Geometris:
Vektor nol ( 0,0 ) tidak memiliki arah, sehingga dot product-nya dengan vektor lain selalu 0 (tapi tidak berarti tegak lurus).

4. Menghitung Sudut Antara Dua Vektor

Dot product memungkinkan kita menghitung sudut $\theta$ antara dua vektor. 

$$
\cos \theta=\frac{\mathbf{A} \cdot \mathbf{B}}{\|\mathbf{A}\| \cdot\|\mathbf{B}\|}
$$

Contoh:

Untuk $\mathbf{A}=(1,0)$ dan $\mathbf{B}=(1, \sqrt{3})$ : 

- $\mathrm{A} \cdot \mathrm{B}=1 \cdot 1+0 \cdot \sqrt{3}=1$.

$\|A\|=1,\|B\|=\sqrt{1^2+(\sqrt{3})^2}=2$,

- $\cos \theta=\frac{1}{1.2}=0.5 \Longrightarrow \theta=60^{\circ}$.

## Sifat-Sifat Pertama Perkalian Titik (Dot Product)
Perkalian titik memiliki beberapa sifat dasar yang penting dalam operasi vektor. Berikut penjelasan lengkaprya:
1. Sifat Komutatif (Pertukaran)

$$
\mathbf{A} \cdot \mathbf{B}=\mathbf{B} \cdot \mathbf{A}
$$

Penjelasan:
Urutan vektor tidak memengaruhi hasil dot product.
Contoh:
- $\mathbf{A}=(2,1)$ dan $\mathbf{B}=(-1,2)$

$$
\begin{aligned}
& \mathbf{A} \cdot \mathbf{B}=(2)(-1)+(1)(2)=-2+2=0 \\
& \mathbf{B} \cdot \mathbf{A}=(-1)(2)+(2)(1)=-2+2=0
\end{aligned}
$$

Hasilnya sama: 0 .
2. Sifat Distributif terhadap Penjumlahan Vektor

$$
\mathbf{A} \cdot(\mathbf{B}+\mathbf{C})=\mathbf{A} \cdot \mathbf{B}+\mathbf{A} \cdot \mathbf{C}
$$

Penjelasan:
Dot product dapat "didistribusikan" ke penjumlahan vektor.
Contoh:

- $\mathbf{A}=(3,4), \mathbf{B}=(3,0), \mathbf{C}=(0,4)$

$$
\begin{gathered}
A \cdot(B+C)=(3,4) \cdot(3+0,0+4)=(3)(3)+(4)(4)=9+16=25 \\
A \cdot B+A \cdot C=9+16=25
\end{gathered}
$$

Hasilnya sama: 25.
3. Kompatibel dengan Perkalian Skalar

$$
(c \mathbf{A}) \cdot \mathbf{B}=c(\mathbf{A} \cdot \mathbf{B})
$$

Penjelasan:
Skalar (c) bisa dipindahkan ke dalam operasi dot product.
Contoh:

- $c=2, A=(1,3), B=(4,-1)$

$$
\begin{gathered}
(2 \mathrm{~A}) \cdot \mathrm{B}=(2,6) \cdot(4,-1)=8-6=2 \\
2(\mathrm{~A} \cdot \mathrm{~B})=2 \cdot(4-3)=2
\end{gathered}
$$

Hasilnya sama: 2.

4. Hubungan dengan Panjang Vektor

$$
\mathbf{A} \cdot \mathbf{A}=\|\mathbf{A}\|^2
$$

Penjelasan:
Dot product vektor dengan dirinya sendiri sama dengan kuadrat panjangnya.
Contoh:
- $\mathbf{A}=(3,4)$

$$
\begin{gathered}
\mathbf{A} \cdot \mathbf{A}=3^2+4^2=9+16=25 \\
\|\mathbf{A}\|=\sqrt{25}=5 \Rightarrow\|\mathbf{A}\|^2=25
\end{gathered}
$$

5. Ortogonalitas (Tegak Lurus)

$$
\mathbf{A} \cdot \mathbf{B}=0 \Rightarrow \theta=90^{\circ}
$$

Penjelasan:
Jika hasil dot product 0, kedua vektor tegak lurus.
Contoh:
- $\mathbf{A}=(2,1)$ dan $\mathbf{B}=(-1,2)$

$$
\mathbf{A \cdot B}=(2)(-1)+(1)(2)=-2+2=0
$$

Kedua vektor membentuk sudut $90^{\circ}$.
6. Perkalian dengan Vektor Nol

$$
A \cdot 0=0
$$

Penjelasan:
Dot product antara vektor apa pun dengan vektor nol selalu 0 .
Contoh:

- $\mathbf{A}=(5,-3)$ dan $0=(0,0)$

$$
A \cdot 0=(5)(0)+(-3)(0)=0
$$