---
title: TripleBaka
CTF: SSMCTF
Year: 2025
category: [crypto]
author: Hal0g3n
date: 29 Jun 2025

hide:
- footer
- toc
---

# idk
by [Hal0g3n](https://github.com/Hal0g3n)
> more like baka ↑↑↑↑ baka ↑↑↑↑ baka...

## WHY REV
[[Why is there rev in my crypto chal]]  

Well that is how SSM do be sometimes... time to dig in

### BAKA
```py
def baka(ba, ka):
    bakabaka = ba
    for bakabakabaka in range(ka-1):
        bakabaka = ba**bakabaka
    return bakabaka
```

With the power of hindsight, I shall refractor this function as such:

```py
def tetration(a, b):
    res = a
    for i in range(b-1):
        res = a ** res
    return res
```

WOW it really is just tetration...

### HYPERBAKA
```py
def hyperbaka(ba, ka, bakabaka):
    if bakabaka == 1:
        return ba**ka
    elif ka == 0:
        return 1
    elif bakabaka == 2 and ba == ka:
        return baka(ba, bakabaka)
    else:
        bakabakabaka = hyperbaka(ba, ka-1, bakabaka)
        return hyperbaka(ba, bakabakabaka, bakabaka-1)
```

Once again, hindsight is 20/20 and we refractor as such:

```py
def knuth_up_arrow(ba, ka, bakabaka):
    if n == 1:
        return a**b
    elif b == 0:
        return 1
    elif n == 2 and a == b:
        return tetration(a, n)
    else:
        temp = knuth_up_arrow(a, b-1, n)
        return knuth_up_arrow(a, temp, n-1)
```

Higher hyperoperations... defined with [knuth's up arrow notation](https://en.m.wikipedia.org/wiki/Knuth%27s_up-arrow_notation)

Now those $\uparrow$s in the description seems very familiar

### TRIPLEBAKA
Ok finally, the last recursive layer.

```py
def triple_baka(n):
    if n == 1:
        return hyperbaka(3, 3, 4)
    else:
        return hyperbaka(3, 3, triple_baka(n-1))
```

As usual, the power of hindsight guides us to refractor as follows:

```py
def hyper_knuth(n):
    if n == 1:
        return knuth_up_arrow(3, 3, 4)
    else:
        return knuth_up_arrow(3, 3, hyper_knuth(n-1))
```

So this is some hyper operation on the hyper operation

$$
H(n) = 3 \uparrow^{H(n-1)} 3
$$

That's pretty big. ~~that's what she said~~

## CRYPTO RANDOMS
Finally, we arrive at the cryptography portion. 

```py
bits = floor(log2(secret) + 1)

a = getPrime(bits // 2) + 1
b = getPrime(bits // 2)
x = getPrime(bits // 2)
m = getPrime(bits)

def get_next():
    global x
    x = (a * x + b) % m

print(f'{bits = }')

TRIPLE_BAKA = triple_baka(64)
for i in range(1, TRIPLE_BAKA + 1):
    get_next()
    if i <= 10:
        print(i, x)

ct = secret ^ x
print(f'{ct = }')
```

So we have a Linear Congruence Generator (LCG) and the `triple_baka(64)`-th random number is xor-ed with the secret. Well, let's start with the LCG

### LCG BREAKING
On top of the `ct` we are also given the first 10 random numbers... this means we can fully recover the LCG.

Let us re-define the following for clarity sake:

$$
\begin{aligned}
p,& b, m, x_0 \text{ is prime} \\
a &= p + 1 \\
x_i &= ax_{i-1} + b \mod m
\end{aligned}
$$

First, we need to figure out $m$, this can be found by finding values congruent to $0 \mod m$. With a little googling, we find the following value:

$$
\begin{aligned}
x_{i+2}x_i - x_{i+1}^2 &= ax_{i+1}x_i + bx_i - (ax_i + b)^2\\
&= a^2 x_i^2 + abx_i + bx_i - a^2 x_i^2 + abx_i + b
\end{aligned}
$$

After finding $m$, we can easily find $a$ as such:

$$
\begin{aligned}
x_{i+2} - x_{i+1} &= (a-1)x_{i+1} + b \mod m\\
&= (a-1)(ax_i + b) + b \mod m\\
&= (a-1)ax_i + (a-1)b + b \mod m\\
&= a(a-1)x_i + ab\mod m\\
&= a([a-1]x_i + b)\mod m\\
&= a(x_{i+1} - x_i)\mod m\\
\\
\\
\implies &x_{i+2} - x_{i+1} = a(x_{i+1} - x_i) \mod m\\
\implies &a = \frac{x_{i+2} - x_{i+1}}{x_{i+1} - x_i} \mod m
\end{aligned}
$$

With $a$ comes $b$:

$$
\begin{aligned}
&x_{i+1} = ax_i + b \mod m\\
\implies &b = x_{i+1} - ax_i \mod m
\end{aligned}
$$

Nice, now we got all parameters $a, b$ and $m$ of the LCG. Lastly, we use the fact that this is a first order recurrence relation to derive the closed form of $x$. 


$$x_n = a^nx_0 + \frac{a^n -1}{a-1}b$$

Now finally, we can proceed to calculate $x_{triple\_baka(64)}$

### LCG CYCLES
The first important note is the cyclic nature of $x_n$ with cycle length $m -1$, as shown with Fermat's Little Theorem:

$$
\begin{aligned}
x_{m-1} &= a^{m-1}x_0 + \frac{a^{m-1} -1}{a-1}b \mod m\\
 & = (1)x_0 + \frac{(1) -1}{a-1}b \mod m \\
 &= x_0 \mod m
\end{aligned}
$$

So we just need to find $triple\_baka(64) \mod m - 1$.

### MODULAR TETRATION
Let's us simplify the problem to just tetration first. How do we solve modular tetration 🤔

Recalling from RSA, $pt^e \mod m = pt^{(e \mod \phi(m))} \mod m$ where $\phi(x)$ is euler's totient function. Applying to $3 \uparrow\uparrow n$ we get:

$$
\begin{aligned}
3 \uparrow\uparrow\ n \mod m &= 3^{(3 \uparrow\uparrow\ n-1 \mod \phi(n))} \mod m \\
&= 3^{[3^{\{3 \uparrow\uparrow\ n-2 \mod \phi(\phi(n))\}} \mod \phi(m)]} \mod m \\
& ...
\end{aligned}
$$

Since $\phi(n) < n$ for all $n > 1$, eventually we will reach a point where $\phi(\phi(...\phi(n))) = 1$.

This means there is a certain value $l$ such that:

$$
3 \uparrow\uparrow\ n = 3^{3^{.^{.^{.{\{3\ \uparrow\uparrow\ n-l \mod 1\}} }}}} \mod m \\
= 3^{3^{.^{.^{.{\{0 \mod 1\}} }}}} \mod m
$$

And we can see that for all $n>l$, $3 \uparrow\uparrow n \mod m = 3 \uparrow\uparrow\ l \mod m$.

This is crucial as we can effectively reduce all values to $l$. Calculating it with SAGEMATH (/sɑːɡeɪmæθ/), we get $l = $ under $\mod m - 1$

### MAGIC OBSERVATION
It might seem like we just took a big detour. Yes... I do admit talking a little too much about the details. But we can finally see da wae (I'm old, I know). 

Simplifying our $triple_baka$ crazy hyperoperation to a tetration:

$$
\begin{aligned}
triple\_baka(64) &= 3 \uparrow^{(triple\_baka(63))} 3 \\
&= 3 \uparrow^{(triple\_baka(63) - 1)} (3 \uparrow^{(triple\_baka(63))} 2) \\
&= 3 \uparrow^{(triple\_baka(63) - 2)} [3 \uparrow^{(triple\_baka(63) - 1)} \{(3 \uparrow^{(triple\_baka(63))} 2) - 1\}]\\
&\cdots \\
&= 3 \uparrow\uparrow (3 \uparrow^3 ...)\\
\end{aligned}
$$

Wow, it is just tetration to an impossibly huge number... wait a huge number. That must mean it is larger than $l$! So under $\mod m - 1$, `triple_baka(64)` is just $3 \uparrow\uparrow l \mod m-1$

And just like that, we just calculate $(3 \uparrow\ l \mod m-1)$-th $x$ value of the LCG, xor with $ct$ and get the flag 🥳

## SOLVE.py

Flag: `grey{how_i_swear_you_shouldve_had_0_knowledge}`
