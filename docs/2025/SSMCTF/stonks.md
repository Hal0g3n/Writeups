---
title: stonks
CTF: SSMCTF
Year: 2025
category: [crypto]
author: Hal0g3n
date: 29 Jun 2025

hide:
- footer
- toc
---

# STONKS
by [Hal0g3n](https://github.com/Hal0g3n)
> STOCKS ONLY GO UP
> 
> r/wallstreetbets

## Problem Setup

The shares we get is Shamir's Secret Sharing, a small easter egg that is kewl and all, but not relevant to the solution.

Let us define our secret sharing protocol first:

$$
\begin{aligned}
&\fbox{Shamir's Hidden Parameters}\\
f(x)    &\text{: unknown polynomial with degree } d,\\
&\text{where } 4 \leq d < 8\\
f(x)    &= r_0 x^0 + r_1x^1 + \cdots + r_dx^d\\
r_i     &\text{: unknown 58-bit integer}\\
r_0=tf  &\text{: unknown 48-bit integer}\\
q       &\text{: 256-bit prime}\\
\end{aligned}
$$

$$
\begin{aligned}
&\fbox{Shamir's Public Parameters}\\
p       &= 2^{128} - 159 \text{ (prime)} \\
x_k         &\text{: 128-bit integer}\\
y_k         &\text{: 128-bit integer},\\
& \text{where } y_k = f(x_k) \mod p \\
\\
g       &= 2\\
vv_i    &= g^{r_i} \mod q \\
\end{aligned}
$$

For the public parameters, we are always given $k=4$ pairs, and all $vv_i$. Our goal is to get $tf$, and submit it to get the flag.

## Linearising Polynomials
[[Hint imaeg]]

From this hint (thanks @gr0undup), it is quite clear we need LLL of some sorts. Usually in CTFs, LLL is used to solve linear equations... which a polynomial is (technically)

Re-looking at the polynomial,

$$
\begin{aligned}
y = f(x)    &= r_0 x^0 + r_1x^1 + \cdots + r_dx^d\\
\end{aligned}
$$

We can see it is just a linear combination of powers of $x$. Putting it in vector form with our 4 pairs of $(x, y)$:

$$
\begin{pmatrix} y_1 \\ y_2 \\ y_3 \\ y_4 \end{pmatrix} = r_0\begin{pmatrix} x_1^0 \\ x_2^0 \\ x_3^0 \\ x_4^0 \end{pmatrix} + r_1\begin{pmatrix} x_1^1 \\ x_2^1 \\ x_3^1 \\ x_4^1 \end{pmatrix} + r_2\begin{pmatrix} x_1^2 \\ x_2^2 \\ x_3^2 \\ x_4^2 \end{pmatrix} + \cdots + r_d\begin{pmatrix} x_1^d \\ x_2^d \\ x_3^d \\ x_4^d \end{pmatrix}
$$

## LLL
We will follow SAGEMATH's (/sɑːɡeɪmæθ/) convention and put the vectors as rows (contrary to columns like most materials online).

Our matrix looks like this:

$$
\left(
\begin{array}{cccc|cc}
x_1^0 & x_2^0 & x_3^0 & x_4^0 & \\
\vdots & \vdots & \vdots & \vdots & &\LARGE{I_{d\times {d+1}}}\\
x_1^d & x_2^d & x_3^d & x_4^d & \\
\\
\hline
\\
y_1 & y_2 & y_3 & y_4 && 0\ \ 0\ \cdots 1\\
\\
\hline
\\
q&0&0&0 &&\\
0&q&0&0 &&\\
0&0&q&0 && \LARGE{0_{4\times d}}\\
0&0&0&q &&\\
\end{array}
\right)
$$

Let us define each row as $\braket{\vec{v_i}\ |\ i\in[0, 1, 2, \cdots, d+4]}$.
From the modular linear equations we got, we know that the first 4 columns must follow this equation:

$$
r_0 \vec{v_0} + r_1 \vec{v_1} + \cdots + r_1 \vec{v_1} = \vec{v_d} + k_1\vec{v_{d+1}} + k_2\vec{v_{d+2}} + k_3\vec{v_{d+3}} + k_4\vec{v_{d+4}}
$$

Where $k_1,k_2,k_3,k_4$ are arbitrary integer constants representing modulus. 

Rearranging everything to one side we get:

$$
r_0 \vec{v_0} + r_1 \vec{v_1} + \cdots + r_1 \vec{v_1} - \vec{v_d} - k_1\vec{v_{d+1}} - k_2\vec{v_{d+2}} - k_3\vec{v_{d+3}} - k_4\vec{v_{d+4}} = \vec{0}
$$

So our aim is to get the following vectors:

$$
\begin{pmatrix}0&0&0&0&r_0&r_1&\cdots&r_d & -1\end{pmatrix}\\
\text{or}\\
\begin{pmatrix}0&0&0&0&-r_0&-r_1&\cdots&-r_d & 1\end{pmatrix}
$$

Let us LLL and... oh noes, it gave this as its shortest vector:

$$
\begin{pmatrix}1&1&1&1&1&0 & 0 &\cdots&0 \end{pmatrix}
$$

Which is just $\vec{v_0}$... In hindsight, it is pretty obvious since $r_i$ is at least 48-bits, which is way larger than that

### A small trick
Since the target vector is so big, what if we artificially made it smaller 🤔

We will divide $r_0, r_1, \cdots r_d$ by $2^{60}$, which is the maximal value of $\sqrt{\sum r_i^2}$ (Proof left as exercise for the reader). We keep the last value as $1$ or $-1$ to ensure that $\vec{v_d}$ is only taken once (as it it large compared to $r_i$)

So now our target vectors are:

$$
\begin{pmatrix}0&0&0&0&\frac{r_0}{2^{60}}&\frac{r_1}{2^{60}}&\cdots&\frac{r_d}{2^{60}} & -1\end{pmatrix}\\
\text{or}\\
\begin{pmatrix}0&0&0&0&-\frac{r_0}{2^{60}}&-\frac{r_1}{2^{60}}&\cdots&-\frac{r_d}{2^{60}} & 1\end{pmatrix}
$$

As a sanity check, we compare magnitudes of the target vector and $\vec{r_0}$

$$
|\vec{r_0}| = \sqrt{5} \\
\text{}\\
|\text{target}| = \sqrt{1+\sum{\frac{r_i^2}{2^{60}}}} \leq \sqrt{1+1} \leq \sqrt{5} = |\vec{r_0}| \\
$$

Nice, and now we just LLL and viola, we got the secret $tf$. \
$$what = tf$$

## Solve.py
```py
# Our constants
p =  2**128 - 159
g = 2

# STONKS
stonks = {
    b"GOOGL": (5, 12),
    b"AMZN": (6, 16),
    b"META": (5, 15),
    b"MSFT": (7, 17),
    b"AAPL": (6, 12),
    b"NVDA": (7, 16),
    b"TSLA": (8, 13),
}

from pwn import *

# io = remote("34.124.170.181", 17983) # REMOTE
# io = process(['python', './stonks/chall.py']) # LOCAL

io.sendline(b"1")
io.recvuntil(b" of $")
company = io.recvuntil(b" ").strip()
io.recvuntil(b": ")

# Retrieving our known variables
shares = eval(io.recvuntil(b"]"))
vv = eval(io.recvuntil(b"]"))
degree = stonks[company][0]


# Generate M
M = []
for i in range(degree):
    M.append([])
    M[-1].append(shares[0][0] ^ i % p)
    M[-1].append(shares[1][0] ^ i % p)
    M[-1].append(shares[2][0] ^ i % p)
    M[-1].append(shares[3][0] ^ i % p)
    M[-1] += [1/2^61 if i == j else 0 for j in range(degree + 1)]
M.append([share[1] for share in shares] + [0 for i in range(degree)] + [1])
M.append([p if 0 == j else 0 for j in range(4)] + [0 for i in range(degree + 1)])
M.append([p if 1 == j else 0 for j in range(4)] + [0 for i in range(degree + 1)])
M.append([p if 2 == j else 0 for j in range(4)] + [0 for i in range(degree + 1)])
M.append([p if 3 == j else 0 for j in range(4)] + [0 for i in range(degree + 1)])
M = matrix(M)

# Perform LLL
M = M.LLL()

# Locate the target vector
for row in M:
    if row[0:4] != 0: continue
    if abs(row[-1]) != 1: continue
    tf = abs(row[4] * 2^61)
    break # Might have multiple answers, but the smallest is the best

print(f"[*] Found {tf = }, a {ceil(tf).bit_length()}-bit integer")

# Send in tf
io.sendline(b"7828322")
io.sendline(str(tf).encode())
io.recvuntil(b"casino.")
print(io.recvall())
```

Flag: `SSMCTF{if_w3_4lll_d0Nt_s3lll_ST0NKS_c4n_0NlY_g0_uPpp}`