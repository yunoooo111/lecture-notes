---
title: "rmse function matrix"
date: 2023-07-26T11:35:00+07:00
authors: ['Sparisoma Viridi']
tags: ['fi4002']
draft: false
math: true
url: "0005"
---
Kesalahan kuadrat rata-rata diakarkan, yang dalam bahasa Inggrisnya root mean square error atau RMSE dapat direpresentasikan dalam bentuk fungsi dan matriks.


# data
Terdapat pasangan nilai $(x_i, y_i)$ dengan $i = 1, 2, \dots, N$, di mana $N$ adalah jumlah data.

Tabel 1. Contoh data dengan $N = 8$.
$i$ | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8
:-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-:
$x_i$ | 2.0 | 3.0 | 4.0 | 5.0 | 6.0 | 7.0 | 8.0 | 9.0
$y_i$ | 7.0 | 8.5 | 11.0 | 13.5 | 15.0 | 16.5 | 19.5 | 21.0


# model
Suatu model linier yang memberikan hubungan antara variabel bebas $x_i$ dan variabel terikat $y_i$ memiliki bentuk

$$\tag{1}
y = c_0 + c_1 x,
$$

dengan dimensi dari $c_0$ dan $c_1$, berturut-turut, adalah sama dengan dimensi dari $y$ dan $y/x$. Dengan menggunakan suatu nilai observasi variabel bebas $x_i$ dapat diperoleh

$$\tag{2}
\hat{y}_i = c_0 + c_1 x_i,
$$

yang merupakan hasil prediksi menggunakan model.


## error
Kesalahan diperoleh dari selisih antara nilai hasil perhitungan menggunakan model $\hat{y}_i$ dengan nilai observasi variabel terikat $y_i$ dalam bentuk

$$\tag{3}
\varepsilon_i = y_i - \hat{y}_i,
$$

sehingga kesalahan totalnya menjadi

$$\tag{4}
\varepsilon = \sum_{i = 1}^N \varepsilon_i.
$$

Persamaan (3) dapat menyebabkan hasil dari Persamaan (4) bernilai kecil karena terjadinya kompensasi kesalahan positif dan negatif. Untuk mencegah hal ini, Persamaan (3) diubah menjadi

$$\tag{5}
\varepsilon_i^2 = (y_i - \hat{y}_i)^2.
$$

Agar nilai kesalahan kuadrat ini agak bebas dari jumlah data, dapat dirumuskan

$$\tag{6}
<\varepsilon^2> = \frac{1}{N} \sum_{i = 1}^N (y_i - \hat{y}_i)^2.
$$

yang merupakan rata-rata kuadrat kesalahan. Selanjutnya, untuk mendapatkan rumusan besaran kesalahan yang berdimensi sama dengan variabel yang diukur dilakukan pencarian akar dari Persamaan (6)

$$\tag{7}
\left( <\varepsilon^2> \right)^{\frac12} = \left[ \frac{1}{N} \sum_{i = 1}^N (y_i - \hat{y}_i)^2 \right]^{\frac12}
$$

yang dikenal sebagai RMSE.


# exercises
1. Gambarkan 

