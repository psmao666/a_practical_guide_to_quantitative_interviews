The angle $\theta$ between two vectors $x$ and $y$ has the property that $cos\theta=\frac{x^{T}y}{\lVert x \rVert\lVert y \rVert}$

The correlation coefficient of two random variables can be viewed as the cosine of the angle between them, ie $p=cos\theta$

### A very classic example

There are 3 random variables x, y and z. Corr(x,y)=0.8 and Corr(x,z)=0.8. What is the range for Corr(y,z)?

![image](https://user-images.githubusercontent.com/113750853/198502807-4ea63249-e3d5-4db9-b23a-118f3770b6f5.png)

Two possible cases, so $Corr(y,z)=cos^{-1}(2\times cos^{-1}(0.8))$ or $Corr(y,z)=cos(0)=1$

We know that $Corr(y,z)=cos(2a)=2cos^{2}-1=0.28$

Therefore, $Corr(y,z)\in [0.28,1]$

### Linear Regression Proof

Consider a set of points $(x_{i},y_{i})$, we use least square approach, let the
final line equation be $$y=mx+b$$
we have $$\epsilon=\sum (y_{i}-mx_{i}-b)^{2}$$
$$\epsilon=\sum (y_{i}^{2}+(mx_{i}+b)^{2}-2y_{i}(mx_{i}+b)$$
To minimize this, we differentiate by chain rule, and got 
$$\frac{d\epsilon}{dm}=\sum 2y_{i}
