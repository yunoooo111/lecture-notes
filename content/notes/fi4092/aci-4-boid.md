---
title: "aligment clustering index for boid"
date: 2023-09-12T13:38:00+07:00
authors: ['Faiz Aulia Rahman', 'Utriweni Mukhaiyar', 'Sparisoma Viridi']
tags: ['fi4092']
draft: false
math: true
url: "0043"
---
{{< toc >}}

## introduction

### terminology
Some terminology ([Pemmaraju, 2013](https://code.tutsplus.com/3-simple-rules-of-flocking-behaviors-alignment-cohesion-and-separation--gamedev-3444t))
+ **Agent**: A single entity or character.
+ **Velocity vector**: An agent's current velocity.
+ **Neighborhood**: A certain area around the agent, used to look for other agents.
+ **Resultant**: The vector obtained from the calculations of the rule.

### velocities
There are velocities due to forces ([von Mammen & Jacob, 2008](https://www.researchgate.net/publication/236578103))
+ alignment
+ cohesion
+ separation
+ wander
+ bound
+ containment

### motion parameters and sets
+ Each boid $i$ has velocity $\vec{v}_i$ and position $\vec{p}_i$.
+ For boid $i$ there is set of neighbors $N_i$, the perceived ones.
+ There is also subset $S_i \subseteq N_i$ for $r_{ij} < d_{\rm min}$.


## forces

### alignment
+ It directs boid $i$ to average direction of its neighbors.
{{< svg "img/fi4092/rule_alignment.svg" >}}
{{< center >}}
([Reynolds, 2001](https://www.red3d.com/cwr/boids/))
{{< /center >}}
$$
\vec{v} _{a, i} = \frac{1}{|N_i|} \sum _{j \in N_i} \vec{v} _j.
$$

### cohesion
+ It attracts boid $i$ to center of its neighbors.
{{< svg "img/fi4092/rule_cohesion.svg" >}}
{{< center >}}
([Reynolds, 2001](https://www.red3d.com/cwr/boids/))
{{< /center >}}
$$
\vec{v} _{c, i} = \frac{1}{|N_i|} \sum _{j \in N_i} \vec{p} _j.
$$

### separation
+ It pushes away boid $i$ from center of its sub-neighbors.
{{< svg "img/fi4092/rule_separation.svg" >}}
{{< center >}}
([Reynolds, 2001](https://www.red3d.com/cwr/boids/))
{{< /center >}}
$$
\vec{v} _{s, i} = \frac{1}{|S_i|} \sum _{j \in N_i} \vec{v} _j.
$$

### wander
+ It represent "free will" of boid $i$ using random number in limited range radius $v_0$.
{{< svg "img/fi4092/rule_wander.svg" >}}
$$
\vec{v} _{r, i} = v_0 \hat{v} + v_0 (\theta \in [0, 2 \pi]) \hat{\theta}.
$$

### bound
+ It directs boid $i$ to center of its neighbors if it is outside the world region.
{{< svg "img/fi4092/rule_bound.svg" >}}
$$
\vec{v} _{b, i} = \vec{w} - \vec{p}_i.
$$

### containment
+ It forces boid $i$ to enter defined and limited region if it is outside.
{{< svg "img/fi4092/rule_containment.svg" >}}
$$
\vec{v} _{t, i} = \left\\{ v_t \hat{v} - v_t (\theta \in [0, 2 \pi]) \hat{\theta} \right\\} \ {\rm for} \ \vec{p} _i \in \Omega.
$$


## simulation

### typical lengths
+ Length used is fish body length or $(\rm BL)$.
{{< svg "img/fi4092/fish_length.svg" >}}
{{< center >}}
([Xiang et al., 2021](https://www.researchgate.net/publication/354848692))
{{< /center >}}
+ It is chosen that $1 {\rm unit \ length} \ {\rm or} \ {\rm BL} \approx {\rm 16px}$.


### parameters
+ For cohesion $d_{\rm min} = 3 \ {\rm BL}$.
+ For separation $d_{\rm min} = 0.3 \ {\rm BL}$.
+ Due to Unity limitation for real time step it uses $\Delta t = 0.025 \ {\rm s}$.
+ Simulation time $t \in [0, 600] \ {\rm s}$
+ Maximum velocity $v_{\rm max} = 15$ unit length per second.
+ Not all previous forces are considered at the same time in each simulation.

### update
For boid $i$
+ Acceleration
$$
\vec{a}_i = \sum_i c_a \vec{v} _{a,i} + c_c \vec{v} _{c,i} + c_s \vec{v} _{s,i} + c_r \vec{v} _{r,i} + c_b \vec{v} _{b,i} + c_t \vec{v} _{t,i}.
$$
+ Velocity
$$
\vec{v}_i (t + \Delta t) = \vec{v}_i (t) + \vec{a}_i.
$$
+ Position
$$
\vec{p}_i (t + \Delta t) = \vec{p}_i (t) + \vec{v}_i(t + \Delta t).
$$


## results

### coefficients
+ cohesion
+ alignment
+ separation
+ containment
+ total = 100

### 70-10-10-00 (cohesion dominant)
{{< youtube "FvfnnNrS1Ic" >}}

### 10-70-10-00 (alignment dominant)
{{< youtube "jOuLU145rKI" >}}

### 10-10-70-00 (separation dominant)
{{< youtube "V81RFPimhUg" >}}

### 10-10-10-70 (containment dominant)
{{< youtube "27UWg0wAQkU" >}}

### aci
{{< svg "img/fi4092/aci_time.svg" >}}