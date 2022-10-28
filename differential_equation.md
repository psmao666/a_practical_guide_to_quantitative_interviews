## Seperable Differential Equation
Seperate $\frac{dy}{dx}$ and integrate both side

## First-order Linear Differential equation
Consider the form $$\frac{dy}{dx}+P(x)y=Q(x)$$
We create an intergration factor, $I(x)$, and multiply both sides, so we have $$I(x)\frac{dy}{dx}+I(x)P(x)y=Q(x)I(x)$$
Then we have $$I(x)\frac{dy}{dx}+I(x)P(x)y=I(x)(y'+P(x)y)$$
And we want this to be equivalent to product rule in differentiation, which means $$(I(x)y)'=I(x)y'+I(x)P(x)y$$
Then we can have $$(I(x)y)'=Q(x)I(x)$$
Therefore $$I(x)y=\int Q(x)I(x)dx$$
And then $$y=\int \frac{Q(x)I(x)}{I(x)}dx$$
Notice that, to make $(I(x)y)'=I(x)y'+I(x)P(x)y$ true, $$I'=I(x)P(x)$$ has to be true, thus $I(x)=\int e^{P(x)} dx$

## Homogeneous linear equations
$$a(x)\frac{d^{2}y}{dx^{2}}+b(x)\frac{dy}{dx}+c(x)y=0$$
Suppose that $y_{1},y_{2}$ are linearly independent solutions to the homogeneous linear equation, then any $y(x)=c_{1}y_{1}(x)+c_{2}y_{2}(x)$, is a solution to the HLE for any constant $c_{1}$ and $c_{2}$.

### Proof
OK let's prove this shit. for $y_{1},y_{2}$ to be solutions to this HLE, we have
$$a(x)\frac{d^{2}y_{1}}{dx^{2}}+b(x)\frac{dy_{1}}{dx}+c(x)y_{1}=0 \qquad (a)$$
$$a(x)\frac{d^{2}y_{2}}{dx^{2}}+b(x)\frac{dy_{2}}{dx}+c(x)y_{2}=0 \qquad (b)$$
Now substitute $y(x)$ in, we have
$$a(x)\frac{d^{2}(c_{1}y_{1}+c_{2}y_{2})}{dx^{2}}+b(x)\frac{d(c_{1}y_{1}+c_{2}y_{2})}{dx}+c(x)(c_{1}y_{1}+c_{2}y_{2})=0$$
according to $(a)\times c_{1}+(b)\times c_{2}=0$
### Formula deduction
Now, this indicates that HLE has infinite number of solutions, but how do we find the pattern?

Let $r_{1},r_{2}$ be the roots of the characteristic equaiton $ar^{2}+br+c=0$

1. if $r_{1},r_{2}$ are real, and $r_{1}\neq r_{2}$, then the general solution is $y=c_{1}e^{r_{1}x}+c_{2}e^{r_{2}x}$
1. if $r_{1},r_{2}$ are real, and $r_{1}=r_{2}=r$, then the general solution is $y=c_{1}e^{rx}+c_{2}e^{rx}$
1. if $r_{1},r_{2}$ are complex, in the form of $\alpha\pm i\beta$, then the general solution is $y=e^{\alpha x}(c_{1}cos\beta x+c_{2}sin\beta x)$

## Nonhomogeneous linear equations

$$a(x)\frac{d^{2}y}{dx^{2}}+b(x)\frac{dy}{dx}+c(x)y=d(x)$$
it will be homogenous solution plus particular solution, ie $$y=y_{p}(x)+y_{g}(x)$$

