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
&\int_{u=0}^{u=\infty} \frac{1}{3} e^{-u} du \\ 
&= \frac{1}{3} \left[-e^{-u}]\right\vert_0^{\infty} \\
&= \frac{1}{3} \\
\end{aligned}$$

Ans: $\frac{1}{3}$

## 19.
For each $n=1,2,3,...$ define  <br>
$f_n(x):=x(1-x^{2n})$ for every $x\in[-1,1]$. <br>

Then the function f defined by <br>
$$f(x):=\lim_{n\to\infty} f_n(x)$$
exists for each $x\in[-1,1]$ and is equal to

#### Solution
When $x=\pm1$: <br>
$f(1):=\lim_{n\to\infty} 1(1-\pm 1^{2n})= \lim_{n\to\infty} 1(1-1^{n})=0$ since $1^{\infty}= 1$ <br>
When $-1 < x < 1$: <br>
$f(x):=\lim_{n\to\infty} x(1-x^{2n})=0$ since $x^{\infty}=x$ for every $x\in(-1,1)$

Ans: 

$$\begin{equation}
  f(x) =
    \begin{cases}
      x & |x|<1\\
      0 & |x|=1\\
    \end{cases}       
\end{equation}$$

## 20.
Consider thw following partial differential equation:<br>
$$\frac{\partial^2 u}{\partial x^2}-\frac{\partial^2 u}{\partial y^2}=0$$
where $u=u(x,y)$ is the unknown function. <br>

Define the following function: <br>
$u_1(x,y):=\cos(2xy)$; $u_2(x,y)=\sin(x^2y)$; and $u_3(x,y)=e^{-(x^2+y^2)}$ <br>
Which of this function are the solution to the above PDE?

#### Solution
Just plug in the mentioned functions.

$$\frac{\partial^2 u_1}{\partial x^2}-\frac{\partial^2 u_1}{\partial y^2} = 4(x^2-y^2)\cos(2xy) \neq 0 $$ 

$$\frac{\partial^2 u_2}{\partial x^2}-\frac{\partial^2 u_2}{\partial y^2} = x^4-4x^2y^2 \sin(x^2y) \neq 0 $$ 

$$\frac{\partial^2 u_3}{\partial x^2}-\frac{\partial^2 u_3}{\partial y^2} = 4(x^2 -y^2)\sin(x^2y) \neq 0 $$ <br>

Ans: None of the functions.

## 21.
A bag contains 50 balls, of which 20 are red and 30 are green. The average (mean) mass for all the balls is $\bar{x}$
kg, and the mean mass for the red balls is $\bar{x}_R$ kg. The mean mass for the green balls is

#### Solution
$$\bar{x}_G=\frac{Total\\; mass\\; of\\; green\\; ball}{Total\\; amount\\; of\\; green\\; ball}= \frac{50*\bar{x}-20*\bar{x}_R}{30}$$

## 22.
A group of 10 students received the following marks for a test: 58, 89, 65, 78, 55, 26, 93, 46, 43, 59. 
The standard deviation of their marks is (to two decimal places)

#### Solution
Standard Deviation Formula:

$$ \sigma=\sqrt{\frac{\sum (x_i-\bar{x})^2}{n}} $$

Calculate the mean, $\bar{x}$ and put the marks into the equation, we get $\sigma=20.91$. <br>
We can also guess the answer since standard deviation is usually much lower than the mean.

## 23.
A magician has 20 coins in his pocket. Twelve of these coins are normal fair coins (with one head and one
tail) and eight are defective coins with heads on both sides. The magician randomly draws a coin from his
pocket and flips it. Given that the flipped coin shows a head, what is the probability that it is defective?

#### Solution
This is a typical example of the application of conditional probability:

$$ P(B|A)=\frac{P(B \cap A)}{P(A)} $$

Hence,

$$ P(defective|head)=\frac{P(defective \cap head)}{P(head)}=\frac{16/40}{28/40}=\frac{4}{7} $$

## 24.
A bag contains 20 balls: 8 red balls and 12 blue balls. Six of these balls are classied as "heavy", and three of
the heavy balls are red. If a ball is chosen at random from the bag, what is the probability that it is red or
heavy?

#### Solution

$$ P(Red \cup Heavy) = \frac{N(Red \cup Heavy)}{Total\\;number\\;of\\;balls}= \frac{ 8 + 3 }{20} = \frac{11}{20} $$

## 25.
A jar contains 5 red balls and 12 blue balls. Two balls are drawn at random from the hat without replacement.
What is the probability that both balls drawn are red?

#### Solution

$$ P(both\\;balls\\;drawn\\;are\\;red)=\frac{Total\\;ways\\;of\\;getting\\;two\\;balls\\;from\\;five\\;red\\;balls\\;(order\\;doesn't\\;matter)}{Total\\;ways\\;of\\;getting\\;two\\;balls\\;from\\;all\\;seventeen\\;balls\\;(order\\;doesn't\\;matter)}= \frac{\binom{5}{2}}{\binom{17}{2}} $$

Also, you may immediately perceive the answer to be:

$$ \frac{5}{17} \times \frac{4}{16} = \frac{5 \times 4}{17 \times 16} = \frac{\binom{5}{2}}{\binom{17}{2}} $$

## 26.
A magician has a collection of 52 cards, with 26 red and 26 black cards. Four of these cards are classied as
'special', and two of the special cards are red. If a card is chosen at random from the 52 cards, what is the
probability that the card is special or red?

#### Solution
Similar to question 24.

$$ P(Special \cup Red) = \frac{N(Special \cup Red)}{Total\\;number\\;of\\;cards}= \frac{ 2 + 26 }{52} = \frac{28}{52} $$

## 27.
A class has 30 girls and 22 boys. A teacher selects 15 students at random from the class to participate in a
competition. What is the probability that out of the 15 selected students, 6 of them are boys?

#### Solution
Similar to question 25. 

$$\begin{aligned}
&P(6\\;boys\\;from\\;15\\;students) \\
&=\frac{Total\\;ways\\;of\\;choosing\\;6\\;boys\\;out\\;of\\;22\\;(order\\;doesn't\\;matter) \times Total\\;ways\\;of\\;choosing\\;9\\;girls\\;out\\;of\\;30\\;(order\\;doesn't\\;matter)}{Total\\;ways\\;of\\;choosing\\;15\\;students\\;out\\;of\\;52\\;(order\\;doesn't\\;matter)} \\
&= \frac{\binom{22}{6} \times \binom{30}{9}}{\binom{52}{15}} \\
\end{aligned}$$

(It is easy to see that this method can be easily generalized to more complicated situations).<br>
Noted that we **cannot** solve this by using a binomial probability formula, such that:

$$ P(6\\;boys\\;from\\;15\\;students)=\binom{15}{6} \times (22/52)^6 \times (30/52)^9 $$

because binomial probability formula is using for **independent** events, while in our case here, all student being chosen will not be put back, so the probability of choosing a boy will not be the same after a boy is chosen. Same goes to girl. Be careful when applying this formula.

##28.
The random variable X has the following probability density function:

$$\begin{equation}
  f_X(x) =
    \begin{cases}
      \frac{c}{x^2} & 1\leq x \leq \infty\\
      0 & elsewhere\\
    \end{cases}       
\end{equation}$$

where c is a constant. Find P(X>25)
