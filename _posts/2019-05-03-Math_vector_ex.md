---
title:  "[Math] 00 vector_ex_01"
last_modified_at: 2019-04-30 11:33:59
author: dsaint31
categories: physics 
use_math: true
tags: math
---

# [CP] 00 Vector Function관련 예제
@(Physics)

## 다음과 같은 vector a,b,c가 있을 때, 아래를 계산하시오.

$$
\text{a}=[3,-2,0], \text{b}=[4,-1,3],\text{c}=[-2,7,-3]
$$

*  $(\text{a} \times \text{b}) \cdot \text{c}$
*  $\text{c} \times (\text{a} + \text{b} ) $

### sol.

*  $(\text{a} \times \text{b} ) \cdot \text{c}$

$$
\begin{align*}
\text{a} \times \text{b} &= \left | 
\begin{array}{cc}
i&j&k \\
3&-2&0 \\
4&-1&3 \\
\end{array}
\right | \\
&= -6i-9j+5k
\end{align*} 
$$

$$
\begin{align*}
(-6i-9j+5k)\cdot(-2i+7j-3k) &= 12-63-15\\
&=-66
\end{align*} 
$$

*  $\text{c} \times (\text{a} + \text{b} ) $

$$
\begin{align*}
\text{a} + \text{b} &= 7i-3j+3k
\end{align*} 
$$

$$
\begin{align*}
\left | 
\begin{array}{cc}
i&j&k \\
-2&7&-3 \\
7&-3&3 \\
\end{array}
\right | &= (21-9)i+(-21+6)j+(6-49)k \\
&= 12i-15j-43k \\
&=[12,-15,-43]
\end{align*} 
$$



## 다음의 vector function으로 표시되는 곡선 r(t)에 대해 점 P에서의 unit tangent vector를 구하시오.

$$
\text{r}(t) = t \text{i} +t^2 \text{j}+t^3\text{k} \\
P = [1,1,1]
$$

### sol.

$$
\begin{align*}
\left[\text{r}(t)\right]_{\text{at} P}&=1 \text{i} +1 \text{j}+1\text{k} \\
&=t \text{i} +t^2 \text{j}+t^3\text{k}\\
\therefore t&=1\\
\\
\text{r}(t) &= t \text{i} +t^2 \text{j}+t^3\text{k} \\
\text{r'}(t) &= 1 \text{i} +2t \text{j}+3t\text{k} \\
\text{r'}(1)&=1 \text{i} +2 \text{j}+3\text{k} \\
\text{u}(1)&=\frac{1 \text{i} +2 \text{j}+3\text{k}}{\sqrt{14}} \\
\end{align*}
$$

## 다음의 velocity vector에 대해, unit tangent vector와 unit normal vector를 구하시오.

$$
\vec{v}(t)= [t,\cos{t},\sin{t}]
$$

### sol.

* unit tangent vector

$$
\frac{d\vec{v}(t)}{dt}= [1,-\sin{t},\cos{t}] \\
\left| \frac{d\vec{v}(t)}{dt}\right| = \sqrt{1^2+(-\sin{t})^2+(\cos{t})^2} =\sqrt{2} \\
\therefore \vec{u}(t) = \frac{1}{\sqrt{2}}(\text{i}-\sin{t}\text{j}+\cos{t}\text{k})
$$

* unit normal vector

$$
\vec{n}(t) = (0\text{i}-\cos{t}\text{j}-\sin{t}\text{k})
$$
