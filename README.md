# Solution-to-Quantitative-Proficiency-Test-2019
### This solution set is only serve for the education purposes, please do not commercialize it.

## 18. 
Evaluate $$\int_{0}^{\infty} \int_{y}^{\infty} 2ye^{-x^3} dxdy $$ by changing the order of the integral, the answer is:

<h4>Solution</h4>
The boundaries: <br>

$0 \leq y\leq \infty$ <br>
$y \leq x \leq \infty$ <br>

(by enclosed region) is equivalent to: <br>
$0 \leq x \leq \infty$ <br>
$0 \leq y \leq x$ <br>

Changing the order of the integral and using the second set of boudaries, we have: 

$$\begin{aligned}
&\int_{x=0}^{x=\infty} \int_{y=0}^{y=x} 2ye^{-x^3} dydx \\ 
&= \int_{x=0}^{x=\infty} \left[y^2]\right\vert_0^{x} 2e^{-x^3} dx \\
&= \int_{x=0}^{x=\infty} x^2 2e^{-x^3} dx \\
\end{aligned}$$

Subs. $u=x^3$, $du = 3x^2 dx$, and the boundary changed to $0 \leq u \leq \infty$, we have:

$$\begin{aligned}
&= \int_{u=0}^{u=\infty} \frac{1}{3} e^{-u} du \\ 
&= \frac{1}{3} \left[-e^{-u}]\right\vert_0^{\infty} \\
&= \frac{1}{3} \\
\end{aligned}$$

## 19.
For each $n=1,2,3,...$ define  <br>
$f_n(x):=x(1-x^{2n})$ for every $x\in[-1,1]$. <br>

Then the function f defined by <br>
$$f(x):=\lim_{n\to\infty} f_n(x)$$
exists for each $x\in[-1,1]$ and is equal to

#### Solution
When $x=\pm1$: <br>
$f(1):=\lim_{n\to\infty} 1(1-\pm 1^{2n})= \lim_{n\to\infty} 1(1-1^{n})=0$ since $1^{\infty}= 1$
When $x<1$: <br>
$f(x):=\lim_{n\to\infty} x(1-x^{2n})=0$ since $x^{\infty}=x$ for every $x\in(-1,1)$

## 20.

