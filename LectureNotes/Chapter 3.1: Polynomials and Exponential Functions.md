# 3.1: Derivatives of Polynomials and Exponential Funtions

## Theorem: Derivative of a constant

$$\frac{d}{dx}(c) = 0$$

### Proof:

Let $f(x) = c$. Then

\begin{align*}
  \frac{d}{dx}(c) & = \lim_{h \rightarrow 0} \frac{c - c}{h} \\
      & = \lim_{h \rightarrow 0} 0 \\
      & = 0
\end{align*}

## Theorem: Derivative of $x$

$$\frac{d}{dx}(x) = 1 $$

### Proof:

$$\begin{align*}
  \frac{d}{dx}(x) & = \lim_{h \rightarrow 0} \frac{(x+h) - (x)}{h} \\
      & = \lim_{h \rightarrow 0} \frac{h}{h} \\
      & = \lim_{h \rightarrow 0} 1 \\
      & = 1
\end{align*}$$

## Theorem: Derivative of $x^2$

$$\frac{d}{dx}(x^2) = 2x $$

### Proof:
<!-- 

$$ \begin{align*}
  \frac{d}{dx}(x^2) & = \lim_{h \rightarrow 0} \frac{(x + h)^2 - (x)^2}{h} \\
      & = \lim_{h \rightarrow 0} \frac{x^2 + 2 x h + h^2 - x^2}{h} \\
      & = \lim_{h \rightarrow 0} \frac{2 x h + h^2}{h} \\
      & = \lim_{h \rightarrow 0} 2 x + h \\
      & = 2x
\end{align*} $$

## Theorem: Derivative of $x^3$

The derivative of $x^3$ is
$$\frac{d}{dx}(x^3) = 3x^2 $$

### Proof:
$$ \begin{align*}
  \frac{d}{dx}(x^3) & = \lim_{h \rightarrow 0} \frac{(x + h)^3 - x^3}{h} \\
      & = \lim_{h \rightarrow 0} \frac{x^3 + 3 x^2 h + 3 x h^2 + h^3 - x^3}{h} \\
      & = \lim_{h \rightarrow 0} \frac{3 x^2 h + 3 x h^2 + h^3}{h} \\
      & = \lim_{h \rightarrow 0} 3 x^2 + 3 x h + h^2 \\
      & = 3 x^2
\end{align*} $$

## Theorm: Derivative of $x^4$

The derivative of $x^4$ is
$$\frac{d}{dx}(x^4) = 4x^3 $$

### Proof:

$$ \begin{align*}
   \frac{d}{dx}(x^4) & = \lim_{h \rightarrow 0} \frac{(x + h)^4 - x^4}{h} \\
      & = \lim_{h \rightarrow 0} \frac{x^4 + 4 x^3 h + 6 x^2 h^2 + 4 x h^3 + h^4 - x^3}{h} \\
      & = \lim_{h \rightarrow 0} \frac{4 x^3 h + 6 x^2 h^2 + 4 x h^3 + h^4}{h} \\
      & = \lim_{h \rightarrow 0} 4 x^3 + 6 x^2 h + 4 x h^2 + h^3 \\
      & = 4 x^3
\end{align*} $$

## Theorem: Derivative of $x^n$

The derivative of $x^n$ is 
$$\frac{d}{dx}(x^n) = nx^{n-1} $$

### Proof:

$$ \begin{align*}
  \frac{d}{dx}(x^n) & = \lim_{h \rightarrow 0} \frac{(x + h)^n - x^n}{h} \\[.2cm]
      & = \lim_{h \rightarrow 0} \frac{x^n + n x^{n-1} h + \ldots + n x h^{n-1} - x^n}{h} \\[.2cm]
      & = \lim_{h \rightarrow 0} \frac{n x^{n-1} h + \ldots +n x h^{n-1} + h^n}{h} \\[.2cm]
      & = \lim_{h \rightarrow 0} (n x^{n-1} + \ldots +n x h^{n-2} + h^{n-1}) \\[.2cm]
      & = n x^{n-1}
\end{align*} $$

## Theorem: Constant Multiple Rule

If $c$ is a constant and $f$ is differentiable, then the derivative of $c f(x)$ is
$$\frac{d}{dx}(c f(x)) = c \frac{d}{dx} f(x)$$

### Proof:

  $$\begin{align*}
    \frac{d}{dx}\left(c f(x)\right) & = \lim_{h \rightarrow 0} \frac{c f(x+h) - c f(x)}{h} \\[.2cm]
      & = \lim_{h \rightarrow 0} c \hspace{.1cm} \frac{f(x+h) - f(x)}{h} \\[.2cm]
      & = c f'(x)
  \end{align*}$$

## Theorem: Sum and Difference Rule

The derivative of the sum is the sum of the derivatives.

$$ \frac{d}{dx}[f(x) + g(x)] = \frac{d}{dx} f(x) + \frac{d}{dx} g(x) $$

The derivative of the difference is the difference of the derivatives.

$$ \frac{d}{dx}[f(x) - g(x)] = \frac{d}{dx} f(x) - \frac{d}{dx} g(x)$$

### Proof:

  $$\begin{align*}
    \frac{d}{dx} [f(x) + g(x)] &  = \lim_{h \rightarrow 0} \frac{(f(x+h) + g(x+h)) - \left(f(x) + g(x)\right)}{h} \\
      & = \lim_{h \rightarrow 0} \frac{f(x+h) - f(x)}{h} + \lim_{h \rightarrow 0} \frac{g(x+h) - g(x)}{h}\\
      & = \frac{d}{dx} f(x) + \frac{d}{dx} g(x)
  \end{align*}$$
and
  $$\begin{align*}
    \frac{d}{dx} [f(x) - g(x)] &  = \lim_{h \rightarrow 0} \frac{(f(x+h) - g(x+h)) - \left(f(x) - g(x)\right)}{h} \\
      & = \lim_{h \rightarrow 0} \frac{f(x+h) - f(x)}{h} - \lim_{h \rightarrow 0} \frac{g(x+h) - g(x)}{h}\\
      & = \frac{d}{dx} f(x) - \frac{d}{dx} g(x)
  \end{align*}$$

## Exponential Functions

Let $f(x) = b^x$. Then
$$\begin{align*}
f'(x) & = \lim_{h \rightarrow 0} \frac{f(x+h) - f(x)}{h} \\
      & = \lim_{h \rightarrow 0} \frac{b^{x+h} - b^x}{h} \\
      & = \lim_{h \rightarrow 0} \frac{b^x(b^h - 1)}{h} \\
      & = \left(\lim_{h \rightarrow 0} \frac{b^h - 1}{h}\right) b^x
\end{align*}$$

This is the original function $b^x$, multiplied by the

$$\displaystyle\lim_{h \rightarrow 0} \frac{b^h - 1}{h}$$

This does not depend on $x$ and is a constant in the context of the function $b^x$. 
At $b=2$ and $b=3$, we approximate this limit by letting $h$ approach 0.

| h | $\frac{2^h - 1}{h}$ | $\frac{3^h - 1}{h}$ |
|---|---|---|
|.1|.712|1.161|
|.01|.696|1.105|
|.001|.693|1.099|
|.0001|.693|1.099|

We can plot this for different values of b.

It looks like there is a value of b, between 2 and 3, for which $\displaystyle\lim_{h \rightarrow 0} \frac{b^h - 1}{h} = 1$

## Definition: The number $e$

The value for the base, $b$, that makes the above limit equal to 1 is $e$. $$\lim_{h \rightarrow 0} \frac{e^h - 1}{h} = 1$$

## Theorem: Derivative of $e^x$

$$ \frac{d}{dx} (e^x) = e^x $$ -->
