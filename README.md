# ECO_s394C_Summer2024
This repository contains the core knowledge notes for the course ECO_s394C_Summer2024.

## Functions of Several Variables

### Implicit Differentiation

If $F(x_1,x_2,\cdots,x_n,z)=c$, then we have $z_{x_i}'=\frac{F_{x_i}'}{F_z'}$.

If $F(x,y)=c$, then $y''=\frac{-1}{(F_2')^3}[F_{11}''(F_2')^2-2F_{12}''F_1'F_2'+F_{22}''(F_1')^2]$

### Homogeneity

$f(tx,ty)=t^kf(x,y)$

Euler's Theorem: If function $f(x,y)$ is homogeneous, and then $xf'_x+yf'_y=kf(x,y)$, and $f_x'$ and $f_y'$ are also homogeneous, with degree of homogeneity for $k-1$.

Every homogeneous function is homothetic.

### Economics Application

#### Marginal Product

For example, $F'_L$ is marginal production by Labor.

#### Elasticity

For $f(x,y)$, we have $El_xf(x,y)\frac{x}{f(x,y)}f'_x(x,y)$ and $El_yf(x,y)=\frac{y}{f(x,y)}f'_y(x,y)$.

If $|El|<1$, it is inelastic, while $|El|\geq1$ is elastic.

Marginal rate of substitute of y for x: $MRS=R_{yx}=\frac{F_x'}{F_y'}$

For along level curve $F(x,y)=c$, elasticity of substitute: $\sigma_{yx}=El_{R_{yx}}(y/x)=\frac{R_{yx}}{y/x}\times\frac{d(y/x)}{dR_{yx}}$.

#### Tax

If we have tax $t$, then profit is represented as $\pi=(P+t)Q-Cost$.

If we have tax credit $t$, then the effective price is $r=p-t$.

## Multivariable Optimization

### Extreme Value Theorem

If the function is continuous and feasible region is compact, then given the extreme value theorem, the maximum/minimum value is attained.

### FOC's

$f_x'=0$ and $f_y'=0$ are neccessary conditions of the points where we reach the maximum/minimum values.

Let's denote $A=f_{xx}''$, $B=f_{xy}''$, $C=f_{yy}''$, and then we have:

(i) $f\text{ is concave }\iff A\leq0,C\leq0,AC-B^2\geq0$

(ii) $f\text{ is convex }\iff A\geq0,C\geq0,AC-B^2\geq0$

(iii) $A<0,AC-B^2>0\implies\text{strictly concave}$

(iv) $A>0,AC-B^2>0\implies\text{strictly convex}$

If (i) or (ii) everywhere, then $f$ is concave or convex global.

### SOC's TEST for Local Extreme

$A<0,AC-B^2>0\implies\text{strictly local maximum}$

$A>0,AC-B^2>0\implies\text{strictly local minimum}$

$AC-B^2<0\implies\text{saddle point}$

$AC-B^2=0\implies\text{the point may be maximum point or minimumu point or saddle point}$

### Lagrange Multipliers

If we want to $\max f(x,y,z)\text{ s.t. }g_1(x,y,z)=c_1,g_x(x,y,z)=c_2$,

we could set up $\mathcal{L}(x,y,z)=f(x,y,z)-\lambda_1[g_1(x,y,z)-c_1]-\lambda_2[g_2(x,y,z)-c_2]$.

And the **neccessary** conditions are:

(i) $\mathcal{L}_x'=0$

(ii) $\mathcal{L}_y'=0$

(iii) $\mathcal{L}_z'=0$

(iv) $g_1(x,y,z)=c_1$

(v) $g_2(x,y,z)=c_2$

### KKT

#### General KKT

If we want to $\max f(x,y)\text{ s.t. }g_1(x,y)\leq c_1,g_2(x,y)\leq c_2$,

we could set up $\mathcal{L}(x,y)=f(x,y)-\lambda_1[g_1(x,y)-c_1]-\lambda_2[g_2(x,y)-c_2$.

And the **neccessary** conditions are:

(i) $\mathcal{L}_x'=0$

(ii) $\mathcal{L}_y'=0$

(iii) $\lambda_1\geq0,\text{ with }\lambda_1=0,\text{ if }g_1<c_1$

(iv) $\lambda_2\geq0,\text{ with }\lambda_2=0,\text{ if }g_2<c_2$

(v) $g_1(x,y)\leq c_1$

(vi) $g_2(x,y)\leq c_2$

When we solve these conditions, we could split into cases:

Case 1: $g_1<c_1,\lambda_1=0$ and $g_2<c_2,\lambda_2=0$

Case 2: $g_1<c_1,\lambda_1=0$ and $\lambda_2\geq0$

Case 3: $\lambda_1\geq0$ and $g_2<c_2,\lambda_2=0$

Case 4: $\lambda_1\geq0$ and $\lambda_2\geq0$

If we want to find the minimum of $f(x,y)$, we could use the transformation like $\min f(x,y)=\max -f(x,y)$.

If $g_1=c_1$ with $g_{1_x}'=g_{1_y}'=0$ and $g_2=c_2$ with $g_{2_x}'=g_{2_y}'=0$ at the maximum of the problem, this method may fail.

#### Nonnegative KKT

If we want to $\max f(x,y)\text{ s.t. }g(x,y)\leq c,x\geq0,y\geq0$,

A. $\mathcal{L}(x,y)=f(x,y)=\lambda[g(x,y)-c]$

B.

  (i) $L_x'\leq0,\text{ with }=0,\text{ if }x>0$

  (ii) $L_x'\leq0,\text{ with }=0,\text{ if }x>0$

C. $\lambda\geq0,\text{ and }=0,\text{ if }g(x,y)<c$

D. $g(x,y)<c,x\geq0,y\geq0$

### Envelope Theorem

$\frac{\partial\pi^*}{\partial\alpha}=\frac{\partial\pi}{\partial\alpha}\vert_{(x=x^\*,y=y^\*)}$

For Lagrange Multipliers, given envelope theorem, we have:

$\frac{\partial f^*(c_j)}{c_j}=\lambda_j$

$f(c+dc)^\*-f(c)^\*\approx\lambda_1(c)dc_1+\cdots+\lambda_m(c)dc_m$

## Algebra

### Vector

$|\overrightarrow{a}\cdot\overrightarrow{b}|\leq|\overrightarrow{a}|\cdot|\overrightarrow{b}|$

$\overrightarrow{a}\cdot\overrightarrow{b}=|\overrightarrow{a}|\times|\overrightarrow{b}|\times\cos\theta$

$\overrightarrow{a}\cdot\overrightarrow{a}=0\iff\overrightarrow{a}=\overrightarrow{0}$

### Matrix

#### Mutiple

$A_{3\times2}B_{2\times2}=C_{3\times2}$

Only when **A** is square, $AA=A^2$.

$(PQ)^2\neq(P^2Q^2)$

$AB\neq BA$

#### Transposition

$(A')'=A$

$(A+B)'=A'+B'$

$(\alpha A)'=\alpha A'$

$(AB)'=B'A'$

If **A** is symmetric $\iff A=A'$

#### Inverse

Inversable $\iff AA^{-1}=A^{-1}A=I\iff |A|\neq0$

$(A^{-1})^{-1}=A$

$(AB)^{-1}=B^{-1}A^{-1}$

$(A')^{-1}=(A^{-1})'$

$(\alpha A)^{-1}=\alpha^{-1}A^{-1}$

##### How to Calculate Inverse?

**Method 1**

$A^{-1}=\frac{1}{|A|}adj(A)$

$adj(A)=(C^+)'$, where $C$ is all the cofactors of A.

For example, for 

$$
A=\begin{bmatrix}
   1 & 2 & 3\\
   4 & 5 & 6\\
   7 & 8 & 9
\end{bmatrix}
$$

we have

$$
C_{11}=\begin{bmatrix}
   5 & 6 \\
   8 & 9
\end{bmatrix}
$$

### Determinant

$|A'|=|A|$

$|\alpha A|=\alpha^n|A|$

$|AB|=|A||B|$

$|A+B|\neq|A|+|B|$

### Cramer's Rule

For example, for equations:

$$
\begin{bmatrix}
   1 & 2 \\
   3 & 4
\end{bmatrix}
\begin{bmatrix}
   x \\
   y
\end{bmatrix}=
\begin{bmatrix}
   5 \\
   6
\end{bmatrix}
$$

we could slove them as:

$$
x=
\frac
{\begin{vmatrix}
   5 & 2 \\
   6 & 4
\end{vmatrix}}
{\begin{vmatrix}
   1 & 2 \\
   3 & 4
\end{vmatrix}}
$$

$$
y=
\frac
{\begin{vmatrix}
   1 & 5 \\
   3 & 6
\end{vmatrix}}
{\begin{vmatrix}
   1 & 2 \\
   3 & 4
\end{vmatrix}}
$$

### Least Square Regression

$\hat\beta=(A'A)^{-1}A'\overrightarrow{y}$

For example, we have observations $(2,1)$, $(5,2)$, $(7,3)$, $(8,3)$, so we could set up equations below:

$$
\begin{bmatrix}
   1 & 2 \\
   1 & 5 \\
   1 & 7 \\
   1 & 8
\end{bmatrix}
\begin{bmatrix}
   \beta_0 \\
   \beta_1
\end{bmatrix}=
\begin{bmatrix}
   1 \\
   2 \\
   3 \\
   3
\end{bmatrix}
$$

which means $A\overrightarrow{\hat\beta}=\overrightarrow{y}$,

so $\hat{y}=A\hat\beta=A(A'A)^{-1}A'\overrightarrow{y}$.
