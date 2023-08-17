---
title: "position to velocity to acceleration"
date: 2023-08-16T12:00:00+07:00
authors: ['Sparisoma Viridi']
tags: ['fi1101']
draft: false
math: true
url: "0011"
subt: "application of calculus in kinematics"
---
Essence of calculus is derivative, that is the instantaneous rate of change of a function with respect to one of its variables, which is equivalent to finding the slope of the tangent line to the function at a point ([Watkins et al., 1999](https://web.mit.edu/wwmath/calculus/differentiation/definition.html)). Position, change of position, and various rates of change of position are referred as kinematic variables, where the terms kinematics means the study of motion, from the Greek word for movement, kinesis ([Redish, 2019](https://www.compadre.org/nexusph/course/Kinematic_variables)). If position is something as function of time, the first derivative gives its velocity, and the second derivative gives its acceleration, or simply differentiate position to get velocity and further differentiate velocity to get acceleration ([Zegarelli, 2021](https://www.dummies.com/article/academics-the-arts/math/calculus/how-to-analyze-position-velocity-and-acceleration-with-differentiation-188086/)), where the derivative means derivative with respect to time.


## position and its derivatives
Suppose that there is position as function of time t in 3-d

$$
\begin{array}{rcl}
\vec{r} & = & x \ \hat{i} + y \ \hat{j} + z \ \hat{k} \newline
& = & x \ \hat{e}_x + y \ \hat{e}_y + z \ \hat{e}_z \newline
& = & x \ \hat{x} + y \ \hat{y} + z \ \hat{z} \newline
& = & x_1 \ \hat{x}_1 + x_2 \ \hat{x}_2 + x_3 \ \hat{x}_3 \newline
& = & x_1 \ \hat{e}_1 + x_2 \ \hat{e}_2 + x_3 \ \hat{e}_3,
\end{array}
$$

where the first style is common in high school, second and third styles in college of science, and the last two styles in college of engineering. It would be better that all styles is understood. Third style will be used here.

Velocity is first derivative of position with respect to time

$$
\begin{array}{rcl}
\vec{v} & = & \displaystyle \frac{d\vec{r}}{dt} \newline
&&\newline
& = & \displaystyle \frac{dx}{dt} \ \hat{x} + \frac{dy}{dt} \ \hat{y} + \frac{dz}{dt} \ \hat{z} \newline
&&\newline
& = & v_x \ \hat{x} + v_y \ \hat{y} + v_z \ \hat{z} \newline
\end{array}
$$

and acceleration is first derivative of velocity

$$
\begin{array}{rcl}
\vec{a} & = & \displaystyle \frac{d\vec{v}}{dt} \newline
&&\newline
& = & \displaystyle \frac{dv_x}{dt} \ \hat{x} + \frac{dv_y}{dt} \ \hat{y} + \frac{dv_z}{dt} \ \hat{z} \newline
&&\newline
& = & a_x \ \hat{x} + a_y \ \hat{y} + a_z \ \hat{z} \newline
\end{array}
$$

or second derivative of position.

The relation between position and its derivatives can also be displayed for each coordinate, e.g.

$$
v_x = \frac{dx}{dt}, \ \ \ \  a_x = \frac{dv_x}{dt},
$$

for $x$ coordinate,

$$
v_y = \frac{dy}{dt}, \ \ \ \  a_y = \frac{dv_y}{dt},
$$

for $y$ coordinate, and

$$
v_z = \frac{dz}{dt}, \ \ \ \  a_z = \frac{dv_z}{dt},
$$

for $z$ coordinate.


Read this on Medium [@6unpnp/d335de4e1676](https://medium.com/@6unpnp/position-to-velocity-to-acceleration-d335de4e1676)
