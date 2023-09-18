---
title: "hello world"
date: 2023-09-18T07:44:00+07:00
authors: ['Yurnero Nolla', "Yudha Matias"]
tags: ['xx1000']
draft: false
math: true
url: "0048"
---
{{< toc >}}

## Equation
$$
\mathbf{M} =
\left[
\begin{matrix}
1 & 2 & 3 & 4 & 5 \newline
1 & 2 & 3 & 4 & 5 \newline
1 & 2 & 3 & 4 & 5 \newline
\end{matrix}
\right]
$$

$$
x_{1,2} = \frac{a-b \pm \sqrt{b^2 - 4ac}}{2a}
$$

$$
y = ax^2 + bx + c
$$

## Quotee
<!-- italics -->
*This text* is italic

_This text_ is italic

<!-- Strong -->
**This text** is Strong

__This text__ is Strong

<!-- Strikethrought -->
~~ This Text ~~ is Strikethrought

<!-- Horizontal Rule -->
---
___

<!-- BlockQuote -->
> This is a Quote

<!-- Inline Code Block -->
'<p>This is a paragraph</p>'

## IMAGES
![Markdown Logo](https://2.bp.blogspot.com/-rj720H-LRDk/XFrag8wyxdI/AAAAAAAAG2U/jTD2baKPkMM_HpyFT8FXQf-jiSlcNOlTACPcBGAYYCw/s1600/LOGO%2BPSPS%2BPEKANBARU%2B%255Bwww.blogovector.com%255D.png)

## Youtube
{{< youtube tboRK8CQZzk >}}

## Link
+ [Google](https://www.google.com/)
+ [Github](https://github.com/)

##List
+ Provinsi
	- Kabupaten/Kota
	- Kecamatan
	- Kelurahan/Desa
	
+ Badan Intelijen Negara
	- Deputi 1
	- Deputi 2
	- Deputi 3

## table
No | Tanggal | Kegiatan | Info
:-: | :- | -:| :-: 
1 | 18 Sept | Senin | **UPACARA**
2 | 19 Sept | Selasa | $\sqrt{x^2}{y^2}$
3 | 20 Sept | Rabu | [Instagram](https://instagram.com/yudhamatias/)
4 | 21 Sept | Kamis | *Slebew KIWKIW*

## Flowchart

{{< mermaid >}}
flowchart LR
	B --> I --> P --> O --> E 
	B(("Begin"))
	I[/"Input"/]
	P["Process"]
	O[/"Output"/]
	O(("End"))
{{< /mermaid >}}	

## Animation with svg

rect,width,height
{{< html >}}
<svg style ="background: #eee;">
	<rect width="50" height="50"></rect>
</svg>
{{< /html >}}

{{< html >}}
<svg style="background: #eee;">
  <rect x="80" y="40" width="50" height="50"></rect>
</svg>
{{< /html >}}


{{< html >}}
<svg style="background: #eee;">
  <rect x="0" y="50" width="50" height="50">
    <animate
      attributeName="x"
      from="0" to="300"
      begin="0s" dur="2s"
      repeatCount="indefinite" />
  </rect>
</svg>
{{< /html >}}

{{< html >}}
<svg style="background: #eee;">
  <rect x="0" y="50" width="50" height="50">
    <animate
      attributeName="x"
      from="300" to="0"
      begin="0s" dur="2s"
      repeatCount="indefinite" />
  </rect>
</svg>
{{< /html >}}

{{< html >}}
<svg style="background: #eee;">
  <rect x="150" y="75" width="50" height="50">
    <animateTransform
      attributeName="transform"
      type="rotate"
      from="0 150 75" to="360 150 75"
      begin="0s" dur="3s"
      repeatCount="indefinite" />
  </rect>
</svg>
{{< /html >}}

{{< html >}}
<svg style="background: #eee;">
  <rect x="150" y="75" width="50" height="50">
    <animateTransform
      attributeName="transform"
      type="rotate"
      from="360 150 75" to="0 150 75"
      begin="0s" dur="3s"
      repeatCount="indefinite" />
  </rect>
</svg>
{{< /html >}}

{{< html >}}
<svg style="background: #eee;">
  <rect x="0" y="0" width="50" height="50">
    <animateTransform
      attributeName="transform"
      type="scale"
      from="0 0" to="6 3"
      begin="0s" dur="3s"
      repeatCount="indefinite" />
  </rect>
</svg>
{{< /html >}}

{{< html >}}
<svg style="background: #eee;">
  <rect x="0" y="0" width="50" height="50">
    <animateTransform
      attributeName="transform"
      type="scale"
      from="0 5" to="6 3"
      begin="0s" dur="3s"
      repeatCount="indefinite" />
  </rect>
</svg>
{{< /html >}}




