---

layout: post
title: "Jacobson 答案"
subtitle: "不完全的个人答案"
author: "小春"
header-img: "img/post-bg-web.jpg"
header-mask: 0.4
tags:
  - Abstract Algebra

---

<script type="text/x-mathjax-config"> MathJax.Hub.Config({ tex2jax: {inlineMath: [['$','$'],['\\(','\\)']]} }); </script> <script type="text/javascript" async src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-MML-AM_CHTML"> </script>

Refeerence Text: Jacobson Basic Algebra I

# Chapter 1 Monoid and Groups

P30

#### Section 1.1

Exercise 1.1.1 .    S was a semigroup when S satisfied (1) $\forall a,b,c \in S$ with an operation (product like, we know), (2) they satisfied "associated law" in S(we need to show). As the condition that gives to us, suppose $\forall a,b,c\in S$ $ab=b$, s.t $(ab)c=bc$, $a(ab)c=a(bc)$, $abc=a(bc)$, we

 want $(ab)c=a(bc)$, $bc=a(bc)$, $(b)c=a(bc)$, $(ab)c=a(bc)$, we show "associative law" in this magma, so it's a semigroup.

Next, we guess $a$ is $id_S$, because $ab=b$, $id*b=b=b*id$, therefore, when $ba=b$, this semigroup have identity element(unit).



Exercise 1.1.2. 

 Q1 is easy . 

Sol to Q2, $(x_1,x_2)\neq (0,0)$

$A_1=(x_1,x_2)(y_1,y_2)=(x_1y_1+2x_2y_2,x_1y_2+x_2y_1)$

$A_2=(x_1,x_2)(z_1,z_2)=(x_1z_1+2x_2z_2,x_1z_2+x_2z_1)$
$$
\begin{cases}
x_{A_1}-x_{A_2}=(x_1y_1+2x_2y_2)-(x_1z_1+2x_2z_2)=0\\
y_{A_1}-y_{A_2}=(x_1y_2+x_2y_1)-(x_1z_2+x_2z_1)=0
\end{cases}
$$
$\Rightarrow$
$$
\begin{cases}
 x_1(y_1-z_1)+2x_2(y_2-z_2)=0\\
x_2(y_1-z_1)+x_1(y_2-z_2)=0
\end{cases}
$$
determinate $\begin{vmatrix}
  x_1&2x_2 \\
  x_2&x_1
\end{vmatrix}$=$x_1^2-2x_2^2$, because $x_1\neq 0$ and $x_2\neq 0$, $\det\neq 0$, hence the system of linear equations have trivial solution $y_1-z_1=0$ and $y_2-z_2=0$, that is $(y_1,y_2)=(z_1,z_2)$.

<u>$\mathbf{Hint:}det\neq 0$,homogeneous system of linear equations only have solution of 0.</u>



Exercise 1.1.3 A Machine Accepts eight-letters word, such as $A=(a_1,a_2,a_3,a_3,a_4,a_5,a_6,a_7,a_8)$, now there is an another word $B=(b_1,b_2,b_3,b_3,b_4,b_5,b_6,b_7,b_8)$, with this two words, this machine is a product, then prints an eight letters word, this process like $ApB=D$, $D=(a_1,a_2,a_3,a_4,a_5,b_6,b_7,b_8)$, therefore, this machine is a magma. Now we just need to prove that this magma product with **accociative law** and have **unit**.

Assume that there is a random word $C=(c_1,\cdots, c_8)$, $A,B$ also random,  if this product in this magma has associative law :$A(BC)=(AB)C\Rightarrow (a_1,\cdots,a_8)(b_1,b_2,b_3,b_4,b_5,c_6,c_7,c_8)=(a_1,a_2,a_3,a_4,a_5,b_6,b_7,b_8)(c_1,\cdots,c_8)$

Obviously $(a_1,a_2,a_3,a_4,a_5,c_6,c_7,c_8)=(a_1,a_2,a_3,a_4,a_5,c_6,c_7,c_8)$, so this magma is a semigroup.

Same, we can prove that the magma in Q2 is also a semigroup.

Assume that there is a unit $e=(e_1,\cdots,e_8)$ in this semigroup, if this $e$ is exist, then $eA=A=Ae$, but obviously this $e$ isn’t exist, because $(a_1,a_2,a_3,a_4,e_5,e_6,e_7,e_8)\neq (e_1,e_2,e_3,e_4,a_5,a_6,a_7,a_8)$ so this semigroup is not a monoid.



Exercise 1.1.4 $(M,p,1)$ is a monoid, $m\in M$, therefore $m$ is associative. We define $p_m(a,b)=amb$ in $M$, $(M,p_m)$ is a semigroup, because this is a magma and with associative law. 

(Not sure for the answer of Q2)

$M$ there would have been unit $1$, suppose $(M,p_m,e_m)$ is a monoid, $e_m$ is the unit relative to $p_m$, $e_m m 1=1, 1me_m=1\Rightarrow e_mm=me_m\Rightarrow e_mm^{-1}=m^{-1}e_m$ , when $m$ is invertible $(M,p_m,e_m)$ is a monoid



Exercise 1.1.5 We just need to prove asscociative law in $M$, because $S$ is semigroup $(S,p)$ and in $M$ we have something $u$ like unit.
$M=(s_1,\cdots,s_n,u)$, $ua=a=au$ for all $a\in M$, $a$ either $s$ or $u$. $(M,p_m)$ is a magma, $p_m:=up_ma=a=ap_mu$  .

If $a_1p_m(up_ma_2)=(a_1p_mu)p_ma_2$, $M$ is a semigroup, obviously $a_1p_ma_2=a_1p_ma_2$, therefore $M$ is a semigroup, and $u$ is the units in $M$, so $M$ is a monoid.

