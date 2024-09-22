# Review: Limits
$\def\lxa{\lim_{x\rightarrow a}}$
$\def\lxap{\lim_{x\rightarrow a^+}}$
$\def\lxam{\lim_{x\rightarrow a^-}}$
$\def\lxn{\lim_{x\rightarrow \infty}}$
$\def\lxnn{\lim_{x\rightarrow -\infty}}$

## Definition: Limit
Let f be a function defined on an interval that contains $x=a$, except possibly at $x=a$. Then we say that
  $$ \lxa f(x) = L $$
means that for every $\epsilon > 0$, there exists $\delta > 0$ such that
  $$\textnormal{if } 0 < \left| x - a \right| < \delta \textnormal{ then } \left| f(x) - L\right| < \epsilon $$

## Rules of Limits

Suppose that $c$ is a constant and that the limits $\lxa f(x)$ and $\lxa g(x)$ both exist. The the following are true
$$ \begin{align}
  \lxa f(x) + g(x) &= \lxa f(x) + \lxa g(x) \\
  \lxa (f(x) - g(x)) &= \lxa f(x) - \lxa g(x) \\
  \lxa c f(x) &= c \lxa f(x) \\
  \lxa (f(x) g(x)) &= \lxa f(x) \lxa g(x) \\
  \lxa \left(\frac{f(x)}{g(x)}\right) &= \frac{\lxa f(x)}{\lxa g(x)}\\
  \lxa \left(f(x)\right)^n &= \left( \lxa f(x)\right)^n \\
  \lxa \sqrt[n]{f(x)} &= \sqrt[n]{\lxa f(x)} \\
  \lxa c &= c \\
  \lxa x &= a \\
  \lxa x^n &= a^n \\
  \lxa \sqrt[n]{x} &= \sqrt[n]{a}
\end{align}$$

## Other Theorems

### Theorem: Functions that differ at $x=a$
If $f(x) = g(x)$ for all $x \neq a$, then $\displaystyle \lxa f(x) = \lxa g(x)$

### Theorem: Equivalence of one-sided and two-sided limits
$\displaystyle \lxa f(x) = L$ if and only if $\displaystyle \lxap f(x) = L = \lxam f(x)$

### Theorem: Limit is Monotonic

If $f(x) \leq g(x)$ when $x$ is near $a$, then $\displaystyle \lxa f(x) \leq \lxa g(x)$.

### The Squeeze Theorem
If $f(x) \leq g(x) \leq h(x)$ when $x$ is near $a$ and if
$$\lxa f(x) = \lxa h(x) = L$$
then $$\lxa g(x) = L$$

## Limits with finite values
### Definition: $\displaystyle \lxa f(x) = L$
For every $\epsilon > 0$, there exists $\delta > 0$ such that
  $$\textnormal{if } 0 < |x - a|< \delta, \textnormal{ then } \left| f(x) - L\right| < \epsilon. $$

### Definition: $\displaystyle \lxap f(x) = L$
For every $\epsilon > 0$, there exists $\delta > 0$ such that
  $$\textnormal{if } a < x < a+\delta, \textnormal{ then } \left| f(x) - L\right| < \epsilon. $$

### Definition: $\displaystyle \lxam f(x) = L$
For every $\epsilon > 0$, there exists $\delta > 0$ such that
  $$\textnormal{if } a - \delta< x < a, \textnormal{ then } \left| f(x) - L\right| < \epsilon. $$

## Limits: Vertical asymptotes
### Definition: $\displaystyle \lxa f(x) = \infty$
For every $N$, there exists $\delta > 0$ such that
  $$\textnormal{if } 0 < x < |a+\delta|, \textnormal{ then } f(x) > N. $$

### Definition: $\displaystyle \lxap f(x) = \infty$
For every $N$, there exists $\delta > 0$ such that
  $$\textnormal{if } a < x < a+\delta, \textnormal{ then } f(x) > N. $$

### Definition: $\displaystyle \lxam f(x) = \infty$
For every $N$, there exists $\delta > 0$ such that
  $$\textnormal{if } a - \delta < x < a, \textnormal{ then } f(x) > N. $$

### Definition: $\displaystyle \lxa f(x) = - \infty$
For every $N$, there exists $\delta > 0$ such that
  $$\textnormal{if } 0 < x < |a+\delta|, \textnormal{ then } f(x) < N. $$

### Definition: $\displaystyle \lxap f(x) = -\infty$
For every $N$, there exists $\delta > 0$ such that
  $$\textnormal{if } a < x < a+\delta, \textnormal{ then } f(x) <> N. $$

### Definition: $\displaystyle \lxam f(x) = -\infty$
For every $N$, there exists $\delta > 0$ such that
  $$\textnormal{if } a - \delta < x < a, \textnormal{ then } f(x) <> N. $$

## Limits: Horizontal Asymptotes
### Definition: $\displaystyle \lxn f(x) = L$
For every $\epsilon > 0$, there exists $N$ such that
  $$\textnormal{if } x > N, \textnormal{ then } |f(x) - L| < \epsilon. $$


### Definition: $\displaystyle \lxnn f(x) = L$
For every $\epsilon > 0$, there exists $N$ such that
  $$\textnormal{if } x < N, \textnormal{ then } |f(x) - L| < \epsilon. $$

## Limits: Unbounded behavior
### Definition: $\displaystyle \lxn f(x) = \infty$
For every $M$, there exists $N$ such that
  $$\textnormal{if } x > N, \textnormal{ then } f(x) > M. $$

### Definition: $\displaystyle \lxn f(x) = - \infty$
For every $M$, there exists $N$ such that
  $$\textnormal{if } x > N, \textnormal{ then } f(x) < M. $$

### Definition: $\displaystyle \lxnn f(x) = \infty$
For every $M$, there exists $N$ such that
  $$\textnormal{if } x < N, \textnormal{ then } f(x) > M. $$

### Definition: $\displaystyle \lxnn f(x) = - \infty$
For every $M$, there exists $N$ such that
  $$\textnormal{if } x < N, \textnormal{ then } f(x) < M. $$