---
title: "shortcode inner"
date: 2023-09-15T17:30:00+07:00
authors: ['Sparisoma Viridi']
tags: ['xx1000']
draft: false
math: true
url: "0046"
---
{{< toc >}}


## highlight
To display

{{< highlight python >}}
N = 2
for i in range(0, N):
  print(i)
print("Done.")
{{< /highlight >}}

following shortcode is used

```python
{{</* highlight python */>}}
N = 2
for i in range(0, N):
  print(i)
print("Done.")
{{</* /highlight */>}}
```

## objective
+ Display content between opening and closing shortcodes.
+ Translate content to SVG elements, the simple first, e.g. line, circle and rectangle.


## test
Following is a SVG image whose border is added using JS

{{< shape >}}
<svg id="fig1" height="100" width="100">
  <circle cx="50" cy="50" r="40"
   stroke="black" stroke-width="3" fill="red" />
  Sorry, your browser does not support inline SVG.  
</svg>

<script>
console.log("hello");
var g = document.getElementById("fig1");
g.style.border = "1px solid blue";
</script>
{{< /shape >}}

with the lines of code are

```md
{{</* shape */>}}
<svg id="fig1" height="100" width="100">
  <circle cx="50" cy="50" r="40"
   stroke="black" stroke-width="3" fill="red" />
  Sorry, your browser does not support inline SVG.  
</svg>

<script>
console.log("hello");
var g = document.getElementById("fig1");
g.style.border = "1px solid blue";
</script>
{{</* /shape */>}}
```

## possible problem
+ Security due if using external JS with some uknown purposes, besides what are required. 
