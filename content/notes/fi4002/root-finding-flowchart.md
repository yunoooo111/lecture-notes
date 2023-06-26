---
title: "root finding flowchart"
date: 2023-01-26T13:19:00+07:00
authors: ['Sparisoma Viridi']
tags: ['fi4002']
draft: false
math: true
url: "0003"
---
Secara umum rumusan pencarian akar secara iteratif melibatkan setidaknya dua nilai tebakan sebelumnya dan fungsinya atau satu tebakan sebelumnya dan fungsi serta turunannya. Generalisasi ini mencakup metode Newton-Raphson, secant, dan false position.

## flowchart
Untuk mencari akar suatu fungsi $f(x)$ dapat dirumuskan terdapatnya suatu fungsi $g(f(x), f'(x), x)$ yang akan memberikan nilai tebakan berikutnya $x_n$, yang semakin mendekati nilai akar yang dicari dengan bergerak dari tebakan awal, misalnya $x_1$ (dan $x_2$), dengan menggunakan informasi $f(x)$ dan $f'(s)$. Diagram alir pencarian akar ini diberikan pada Gambar 1.

{{< mermaid >}}
flowchart TD
  B --> I --> N1 --> o1a
  o1b --> P1 --> P2 --> o2a
  o2b --> C --"N"--> N2 --> o1c
  C --"Y"--> O --> o3a
  o3b --> E
  B(["Begin"])
  I[/"x(1), x(2),<br>f(x), f'"/]
  N1["n = 3"]
  N2["n = n + 1"]
  P1["x(n) = x(n-1) +<br>g(f, f', x(n-2))"]
  P2["fn = f(x(n))"]
  C{"|fn| < &epsilon;"}
  O[/"x(n)"/]
  o1a(("1"))
  o1b(("1"))
  o1c(("1"))
  o2a(("2"))
  o2b(("2"))
  o3a(("3"))
  o3b(("3"))
  E(["End"])
{{< /mermaid >}}

Gambar 1. Diagram alir pencarian akar suatu persamaan $f(x)$.

Dikarenakan keterbatasan dukungan Mermaid untuk MathJax, lambang-lambang pada Gambar 1 menggunakan simbol terdekat yang diharapkan tidak menimbulkan salah penafsiran, seperti misalnya `x(1)` untuk $x_1$ dan `fn` untuk $f_n$.