# Review: Limits

## Definition: Limit
Let f be a function defined on an interval that contains $x=a$, except possibly at $x=a$. Then we say that
```math
   \lim_{x\rightarrow a} f(x) = L
```
means that for every $\epsilon > 0$, there exists $\delta > 0$ such that
  $$\textnormal{if } 0 < \left| x - a \right| < \delta \textnormal{ then } \left| f(x) - L\right| < \epsilon $$

## Rules of Limits

Suppose that $c$ is a constant and that the limits $\displaystyle \lim_{x\rightarrow a} f(x)$ and $\displaystyle \lim_{x\rightarrow a} g(x)$ both exist. The the following are true
```math
 \begin{align}
  \lim_{x\rightarrow a} f(x) + g(x) &= \lim_{x\rightarrow a} f(x) + \lim_{x\rightarrow a} g(x) \\
  \lim_{x\rightarrow a} (f(x) - g(x)) &= \lim_{x\rightarrow a} f(x) - \lim_{x\rightarrow a} g(x) \\
  \lim_{x\rightarrow a} c f(x) &= c \lim_{x\rightarrow a} f(x) \\
  \lim_{x\rightarrow a} (f(x) g(x)) &= \lim_{x\rightarrow a} f(x) \lim_{x\rightarrow a} g(x) \\
  \lim_{x\rightarrow a} \left(\frac{f(x)}{g(x)}\right) &= \frac{\lim_{x\rightarrow a} f(x)}{\lim_{x\rightarrow a} g(x)}\\
  \lim_{x\rightarrow a} \left(f(x)\right)^n &= \left( \lim_{x\rightarrow a} f(x)\right)^n \\
  \lim_{x\rightarrow a} \sqrt[n]{f(x)} &= \sqrt[n]{\lim_{x\rightarrow a} f(x)} \\
  \lim_{x\rightarrow a} c &= c \\
  \lim_{x\rightarrow a} x &= a \\
  \lim_{x\rightarrow a} x^n &= a^n \\
  \lim_{x\rightarrow a} \sqrt[n]{x} &= \sqrt[n]{a}
\end{align}
```

## Other Theorems

### Theorem: Functions that differ at $x=a$
If $f(x) = g(x)$ for all $x \neq a$, then $\displaystyle \lim_{x\rightarrow a} f(x) = \lim_{x\rightarrow a} g(x)$

### Theorem: Equivalence of one-sided and two-sided limits
$\displaystyle \lim_{x\rightarrow a} f(x) = L$ if and only if $\displaystyle \lim_{x\rightarrow a^+} f(x) = L = \lim_{x\rightarrow a^-} f(x)$

### Theorem: Limit is Monotonic

If $f(x) \leq g(x)$ when $x$ is near $a$, then $\displaystyle \lim_{x\rightarrow a} f(x) \leq \lim_{x\rightarrow a} g(x)$.

### The Squeeze Theorem
If $f(x) \leq g(x) \leq h(x)$ when $x$ is near $a$ and if
```math
\lim_{x\rightarrow a} f(x) = \lim_{x\rightarrow a} h(x) = L
```
then 
```math
\lim_{x\rightarrow a} g(x) = L
```

## Limits: Finite Values
### Definition: $\hspace{1cm}\displaystyle \lim_{x\rightarrow a} f(x) = L$
For every $\epsilon > 0$, there exists $\delta > 0$ such that
```math
 \textnormal{if } 0 < |x - a|< \delta \textnormal{, then } \left| f(x) - L\right| < \epsilon
```

### Definition: $\hspace{1cm}\displaystyle \lim_{x\rightarrow a^+} f(x) = L$
For every $\epsilon > 0$, there exists $\delta > 0$ such that 
```math
  \textnormal{if }
   a < x < a+\delta \textnormal{, then } \left| f(x) - L\right| < \epsilon 
```

### Definition: $\hspace{1cm} \displaystyle \lim_{x\rightarrow a^-} f(x) = L$
For every $\epsilon > 0$, there exists $\delta > 0$ such that
  $$\textnormal{if } a - \delta< x < a, \textnormal{ then } \left| f(x) - L\right| < \epsilon $$

## Limits: Vertical asymptotes
### Definition: $\hspace{1cm} \displaystyle \lim_{x \rightarrow a} f(x) = \infty$
For every $N$, there exists $\delta > 0$ such that
  $$\textnormal{if } 0 < x < |a+\delta|, \textnormal{ then } f(x) > N $$

### Definition: $\hspace{1cm} \displaystyle \lim_{x\rightarrow a^+} f(x) = \infty$
For every $N$, there exists $\delta > 0$ such that
  $$\textnormal{if } a < x < a+\delta, \textnormal{ then } f(x) > N $$

### Definition: $\hspace{1cm} \displaystyle \lim_{x\rightarrow a^-} f(x) = \infty$
For every $N$, there exists $\delta > 0$ such that
  $$\textnormal{if } a - \delta < x < a, \textnormal{ then } f(x) > N $$

### Definition: $\hspace{1cm} \displaystyle \lim_{x\rightarrow a} f(x) = - \infty$
For every $N$, there exists $\delta > 0$ such that
  $$\textnormal{if } 0 < x < |a+\delta|, \textnormal{ then } f(x) < N $$

### Definition: $\hspace{1cm} \displaystyle \lim_{x\rightarrow a^+} f(x) = -\infty$
For every $N$, there exists $\delta > 0$ such that
  $$\textnormal{if } a < x < a+\delta, \textnormal{ then } f(x) <> N $$

### Definition: $\hspace{1cm} \displaystyle \lim_{x\rightarrow a^-} f(x) = -\infty$
For every $N$, there exists $\delta > 0$ such that
  $$\textnormal{if } a - \delta < x < a, \textnormal{ then } f(x) <> N $$

## Limits: Horizontal Asymptotes
### Definition: $\hspace{1cm} \displaystyle \lim_{x\rightarrow \infty} f(x) = L$
For every $\epsilon > 0$, there exists $N$ such that
  $$\textnormal{if } x > N, \textnormal{ then } |f(x) - L| < \epsilon $$


### Definition: $\hspace{1cm} \displaystyle \lim_{x\rightarrow -\infty} f(x) = L$
For every $\epsilon > 0$, there exists $N$ such that
  $$\textnormal{if } x < N, \textnormal{ then } |f(x) - L| < \epsilon. $$

## Limits: Unbounded behavior
### Definition: $\hspace{1cm} \displaystyle \lim_{x\rightarrow\infty} f(x) = \infty$
For every $M$, there exists $N$ such that
  $$\textnormal{if } x > N, \textnormal{ then } f(x) > M. $$

### Definition: $\hspace{1cm} \displaystyle \lim_{x\rightarrow\infty} f(x) = - \infty$
For every $M$, there exists $N$ such that
  $$\textnormal{if } x > N, \textnormal{ then } f(x) < M. $$

### Definition: $\hspace{1cm} \displaystyle \lim_{x\rightarrow -\infty} f(x) = \infty$
For every $M$, there exists $N$ such that
  $$\textnormal{if } x < N, \textnormal{ then } f(x) > M. $$

### Definition: $\hspace{1cm} \displaystyle \lim_{x\rightarrow -\infty} f(x) = - \infty$
For every $M$, there exists $N$ such that
  $$\textnormal{if } x < N, \textnormal{ then } f(x) < M. $$