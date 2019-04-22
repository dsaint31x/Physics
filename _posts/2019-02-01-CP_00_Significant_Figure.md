---
title:  "[Physics] 00 Significant Figure"
last_modified_at: 2019-02-01 11:33:59
author: dsaint31
categories: physics
use_math: true
tags: significant figure
---

# [CP] 00 Significant Figure (유효숫자)
@(Physics)

* 모든 measured value(측정값)은 **근사값**임
* 때문에, 무의미한 자릿수들을 나열할 필요가 없음.
* 때문에, **효력이 있는 숫자**, 즉 **유효숫자(Significant figure) 만을 표시**하여야 함.
	* 유효숫자로 표시할 경우, *마지막 자리의 숫자는 불확실성*을 포함.
* **유효숫자의 개수**는 *오차를 얼마나 포함하는가를 나타냄*.
	* 정확도와 연관됨

### 예제

 A가 B에게 금속으로 된 정육면체를 만들어주기로 했다. 
B에게 주기로 한 금속 정육면체는 83g이 되어야만 한다.
이를 위해 구한 금속 덩어리의 밀도는 8.67g/㎤ 였다. 
A가 B에게 주기로 한 금속 정육면체의 부피를 계산하고 한변의 길이를 구하라. (A와 B, 그리고 여러분은 엔지니어로서 significant figure 개념을 알고 있다.)

### 풀이

부피를 구할 때, 나누기를 사용하는데, 곱셉이나 나눗셈의 경우, 다음과 같이 유효숫자 갯수가 적은 쪽에 맞춰 답을 구하게 됨 (자리를 맞추기 위해서 반올림 이용).

$$
\frac{83 \text{g}}{8.67 \text{g/cm}^3} = 9.5732... \text{cm}^3 = 9.6 \text{cm}^3
$$

이후, 한변의 길이를 구하면 다음과 같음.

$$
( 9.6 \text{cm}^3 ) ^{1/3} = 2.1253... \text{cm}=2.1\text{cm }
$$
