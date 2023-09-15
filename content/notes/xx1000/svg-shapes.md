---
title: "svg shapes"
date: 2023-09-15T19:43:00+07:00
authors: ['Sparisoma Viridi']
tags: ['xx1000']
draft: false
math: true
url: "0047"
---
{{< toc >}}

## predefined shapes
There are at least seven predefined SVG shape elements that can be used, which are rectangle, circle, ellipse, line, polyline, polygon, and path ([W3Schools, 2023](https://www.w3schools.com/graphics/svg_rect.asp)).


## rectangle
+ Code
```md
{{</* html */>}}
<svg width="200" height="100" style="background: #eee;">
  <rect x="30" y="20" width="50" height="50"
   stroke="red" fill="none"></rect>
  <rect x="120" y="30" width="50" height="50"
   fill="blue"></rect>
</svg>
{{</* /html */>}}
```
+ Result
{{< html >}}
<svg width="200" height="100" style="background: #eee;">
  <rect x="30" y="20" width="50" height="50"
   stroke="red" fill="none"></rect>
  <rect x="120" y="30" width="50" height="50"
   fill="blue"></rect>
</svg>
{{< /html >}}
