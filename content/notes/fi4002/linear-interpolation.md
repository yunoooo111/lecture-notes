---
title: "linear interpolation"
date: 2023-08-29T20:07:00+07:00
authors: ['Sparisoma Viridi']
tags: ['fi4002']
draft: false
math: true
url: "0023"
---
Fungsi linier dapat dibuat untuk menghubungkan dua buah titik data terdekat sehingga titik-titik lain di antara kedua titik data diperoleh menggunakan fungsi tersebut.


## range $0$ and $1$
Ilustrasi paling sederhana untuk interpolasi adalah mencari fungsi

$$\tag{1}
f(x) = c_0 + c_1 x, \ \ \ \ 0 \le x \le 1.
$$

Terdapat dua titik data $(0, y_0)$ dan $(1, y_1)$ yang memenuhi

$$\tag{2}
f(0) = y_0, \ \ \ \ f(1) = y_1.
$$

Substitusi Persamaan (2) ke Persamaan (1) akan memberikan

$$\tag{3}
y_0 = c_0
$$

dan

$$\tag{4}
y_1 = c_0 + c_1.
$$

Substitusi Persamaan (3) ke Persamaan (4) akan memberikan

$$\tag{5}
c_1 = y_1 - y_0.
$$

Dengan demikian Persamaan (1) dapat dituliskan kembali menjadi

$$\tag{6}
f(x) = y_0 + (y_1 - y_0) x, \ \ \ \ 0 \le x \le 1.
$$


## range $x_0$ and $x_1$
Rentang $x$ dalam Persamaan (6) dapat diperluas menjadi $x_0$ dan $x_1$ dengan

$$\tag{7}
0 = \frac{x_0 - x_0}{x_1 - x_0}
$$

dan

$$\tag{8}
1 = \frac{x_1 - x_0}{x_1 - x_0},
$$

sehingga dapat memberikan

$$\tag{9}
0 \le \frac{x - x_0}{x_1 - x_0} \le 1
$$

atau

$$\tag{10}
x_0 \le x \le x_1.
$$

Titik data dalam Persamaan (2) perlu dimodifikasi menjadi

$$\tag{11}
f(x_0) = y_0, \ \ \ \ f(x_1) = y_1,
$$

yang apabila disubstitusikan ke Persamaan (1) akan memberikan

$$\tag{12}
y_0 = c_0 + c_1 x_0
$$

dan

$$\tag{13}
y_1 = c_0 + c_1 x_1.
$$

Dari Persamaan (12) dan (13) akan diperoleh

$$\tag{14}
c_1 = \frac{y_1 - y_0}{x_1 - x_0}
$$

dan

$$\tag{15}
c_0 = \tfrac12(y_0 + y_1) - \tfrac12 (x_0 + x_1) c_1.
$$
