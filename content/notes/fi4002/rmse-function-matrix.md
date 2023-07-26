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

dengan dimensi dari $c_0$ dan $c_1$, berturut-turut, adalah sama dengan dimensi dari $y$ dan $y/x$.