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

