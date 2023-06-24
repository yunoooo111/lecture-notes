---
title: "initial condition for sho"
date: 2022-12-04T17:51:00+07:00
authors: ['Sparisoma Viridi']
tags: ['fi1101']
math: true
draft: false
url: "0002"
---
Suatu benda yang bergerak dalam satu-dimensi dengan gerak harmonis sederhana (GHS), atau simple harmonic motion (SHM), memiliki solusi yang telah umum dikenal. Penerapan syarat awal yang berbeda akan memberikan penjelasan mengenai koefisien-koefisien pada solusi umum tersebut.


# equation of motion and solution
Sebuah benda dengan persamaan gerak

$$\tag{1}
\frac{d^2 x}{dt^2} + \omega^2 x = 0
$$

akan memiliki solusi untuk posisinya dalam bentuk

$$\tag{2}
x = A \sin (\omega t + \varphi_0),
$$

dengan simpangan $x$, amplitudo simpangan $A$, frekuensi angular $\omega$, dan fasa awal $\varphi_0$. Selanjutnya, solusi untuk kecepatan $v$ benda saat $t$ adalah

$$\tag{3}
v = \omega A \sin (\omega t + \varphi_0),
$$

dengan $v_{\max} = \omega A$ adalah amplitudo kecepatan atau laju maksimum benda. Dengan cara yang sama dapat ditulskan bahwa $x_{\max} = A$ adalah simpangan maksimum.


# questions
1. Tunjukkan bahwa Persamaan (2) merupakan solusi dari Persamaan (1) dengan melakukan substitusi Persamaan (2) ke Persamaan (1).
2. Apakah nilai $\varphi_0$ pada Persamaan (2) mempengaruhi bentuk persamaan gerak benda pada Persamaan (1)?
3. Dengan menggunakan hubungan antara besaran-besaran kinematika, tunjukkan bagaimana Persamaan (3) diperoleh dari Persamaan (2).


# .
Solusi persamaan gerak sistem GHS berbentuk

$$\tag{1}
x = A \sin (\omega t + \varphi_0)
$$

memerlukan dua syarat awal saat $t = t_0$, yaitu $x(t_0) = x_0$ dan $v(t_0) = v_0$, yang untuk memudahkan dipilih $t_0 = 0$.

Benda, massa yang terikat pegas atau bandul yang terikat tali, diberi simpangan awal $x_0$ dan dilepas tanpa kecepatan awal atau $v_0 = 0$ saat $t = 0$, maka dari Persamaan (1) dapat diperoleh

$$\tag{2}
\begin{array}{rcl}
x  & = & A \sin (\omega t + \varphi_0) \newline
x(0) & = & A \sin (\omega \cdot 0 + \varphi_0) \newline
x_0 & = & A \sin \varphi_0
\end{array}
$$

dan dari turunan Persamaan (1) terhadap waktu $t$ diperoleh

$$\tag{3}
\begin{array}{rcl}
v  & = & \omega A \cos (\omega t + \varphi_0) \newline
v(0) & = & \omega A \cos (\omega \cdot 0 + \varphi_0) \newline
v_0 & = & \omega A \cos \varphi_0.
\end{array}
$$

Dari dikarenakan $v_0 = 0$ maka dari Persamaan (3) diperoleh $\varphi_0 = (n + \tfrac12) \pi$ dengan $n = 0, 1, 2, ..$. Bila dipih $n = 0$, diperoleh $\varphi_0 = \tfrac12 \pi$, sehingga Persamaan (2) akan menjadi

$$\tag{4}
\begin{array}{rcl}
x_0 & = & A \sin \tfrac12 \pi \newline
& = & A,
\end{array}
$$

yang memberikan nilai amplitudo $A$. Dengan hasil dari Persamaan (4), Persamaan (1) dapat dituliskan kembali menjadi

$$\tag{5}
x = x_0 \sin (\omega t + \tfrac12 \pi),
$$

yang merupakan solusi khusus dari sistem GHS dengan syarat awal $x(0) = x_0$ dan $v(0) = 0$.


# .
Solusi persamaan gerak sistem GHS berbentuk

$$\tag{1}
x = A \sin (\omega t + \varphi_0)
$$

memerlukan dua syarat awal saat $t = t_0$, yaitu $x(t_0) = x_0$ dan $v(t_0) = v_0$, yang untuk memudahkan dipilih $t_0 = 0$.

Benda, massa yang terikat pegas atau bandul yang terikat tali, pada posisi kesetimbangannya atau $x_0 = 0$ diberi kecepatan awal $v_0$ saat $t = 0$, maka dari Persamaan (1) dapat diperoleh

$$\tag{2}
\begin{array}{rcl}
x  & = & A \sin (\omega t + \varphi_0) \newline
x(0) & = & A \sin (\omega \cdot 0 + \varphi_0) \newline
0 & = & A \sin \varphi_0
\end{array}
$$

dan dari turunan Persamaan (1) terhadap waktu $t$ diperoleh

$$\tag{3}
\begin{array}{rcl}
v  & = & \omega A \cos (\omega t + \varphi_0) \newline
v(0) & = & \omega A \cos (\omega \cdot 0 + \varphi_0) \newline
v_0 & = & \omega A \cos \varphi_0.
\end{array}
$$

Dari dikarenakan $x_0 = 0$ maka dari Persamaan (2) diperoleh $\varphi_0 = n \pi$ dengan $n = 0, 1, 2, ..$. Bila dipih $n = 0$, diperoleh $\varphi_0 = 0$, sehingga Persamaan (3) akan menjadi

$$\tag{4}
\begin{array}{rcl}
v_0 & = & \omega A \cos 0 \newline
& = & \omega A,
\end{array}
$$

yang memberikan nilai amplitudo $A = v_0 / \omega $. Dengan hasil dari Persamaan (4), Persamaan (1) dapat dituliskan kembali menjadi

$$\tag{5}
x = \frac{v_0}{\omega} \sin \omega t,
$$

yang merupakan solusi khusus dari sistem GHS dengan syarat awal $x(0) = 0$ dan $v(0) = v_0$.

# .
Solusi persamaan gerak sistem GHS berbentuk

$$\tag{1}
x = A \sin (\omega t + \varphi_0)
$$

memerlukan dua syarat awal saat $t = t_0$, yaitu $x(t_0) = x_0$ dan $v(t_0) = v_0$, yang untuk memudahkan dipilih $t_0 = 0$.

Benda, massa yang terikat pegas atau bandul yang terikat tali, pada posisi tertentu $x_0 = 0$ diberi kecepatan awal $v_0$ saat t = $0$, maka dari Persamaan (1) dapat diperoleh

$$\tag{2}
\begin{array}{rcl}
x  & = & A \sin (\omega t + \varphi_0) \newline
x(0) & = & A \sin (\omega \cdot 0 + \varphi_0) \newline
x_0 & = & A \sin \varphi_0
\end{array}
$$

dan dari turunan Persamaan (1) terhadap waktu $t$ diperoleh

$$\tag{3}
\begin{array}{rcl}
v  & = & \omega A \cos (\omega t + \varphi_0) \newline
v(0) & = & \omega A \cos (\omega \cdot 0 + \varphi_0) \newline
v_0 & = & \omega A \cos \varphi_0.
\end{array}
$$

Terdapat dua persamaan, yaitu Persamaan (2) dan (3) dan dua parameter yang tidak diketahui, yaitu $A$ dan $\varphi_0$, yang seharusnya dapat diperoleh.

Persamaan (2) dibagi Persamaan (3) akan memberikan

$$\tag{4}
\tan \varphi_0 = \frac{x_0}{v_0/\omega} = \frac{\omega x_0}{v_0},
$$

$$\tag{5}
\sin \varphi_0 = \frac{\omega x_0}{\sqrt{\omega^2 x_0^2 + v_0^2}},
$$

$$\tag{6}
\cos \varphi_0 = \frac{v_0}{\sqrt{\omega^2 x_0^2 + v_0^2}}.
$$

Substitusi Persamaan (5) ke Persamaan (2) atau Persamaan (6) ke Persamaan (3) akan memberikan

$$\tag{7}
\begin{array}{rcl}
x_0  & = & \displaystyle A \ \frac{\omega x_0}{\sqrt{\omega^2 x_0^2 + v_0^2}} \newline
&&\newline
A & = & \displaystyle \frac{\sqrt{\omega^2 x_0^2 + v_0^2}}{\omega} \newline
& = & \sqrt{x_0^2 + (v_0 / \omega)^2}.
\end{array}
$$

Substitusi Persamaan (5) dan (7) ke Persamaan (1) akan memberikan

$$\tag{8}
x = \left[ x_0^2 + \left( \frac{v_0}{\omega} \right)^2 \right]^{\frac12} \ \sin \left[ \omega t + \arcsin \left( \frac{\omega x_0}{\sqrt{\omega^2 x_0^2 + v_0^2}} \right) \right]
$$

yang merupakan solusi khusus dari sistem GHS dengan syarat awal $x(0) = x_0$ dan $v(0) = v_0$.


# .
Energi kinetik sistem yang bergerak mengikuti gerak harmonik sederhana (GHS) diberikan oleh

$$\tag{1}
K = \tfrac12 m \omega^2 A^2 \cos^2 (\omega t + \varphi_0),
$$

yang untuk sistem pegas-benda (pegas berkonstanta $k$ dan benda bermassa $m$) akan menjadi

$$\tag{2}
K = \tfrac12 k A^2 \cos^2 (\omega t + \varphi_0),
$$

dengan $\omega = \sqrt{k/m}$. Energi potensial pegas adalah

$$\tag{3}
U = \tfrac12 k x^2 = \tfrac12 k A^2 \sin^2 (\omega t + \varphi_0),
$$

sehingga, dengan hubungan $E = K + U$, dapat diperoleh energi total

$$\tag{4}
E = \tfrac12 k A^2,
$$

yang merupakan energi mekanik sistem.


# .
Dengan energi mekanik sistem GHS

$$\tag{1}
E = K + U
$$

dan $E = \tfrac12 kA^2$, $K = \tfrac12 m v^2$, $U = \tfrac12 k x^2$ dapat dituliskan

$$\tag{2}
K = E - U = \tfrac12 k A^2 - \tfrac12 k x^2
$$

dan lebih lanjut dapat diperoleh

$$\tag{3}
v = \omega \sqrt{A^2 - x^2},
$$

yang memberikan $v = v(x)$, di mana $\omega = \sqrt{k/m}$.
