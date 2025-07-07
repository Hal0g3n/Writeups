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

# idk
by [Hal0g3n](https://github.com/Hal0g3n)
> STOCKS ONLY GO UP
> 
> r/wallstreetbets

## Problem Setup


```py
tf = getrandbits(48)

p =  2**128 - 159
q = getPrime(256)
g = 2

def make_random_shares(minimum, num_shares):
    coefficients = [tf]
    vv = [pow(g, tf, q)]
    
    for i in range(1, minimum):
        r = randint(2**58, 2**59)
        coefficients.append(r)
        vv.append(pow(g, r, q))

    shares = []
    for _ in range(num_shares):
        x = randint(2**127, 2**128)
        y = 0
        for power, coeff in enumerate(coefficients):
            y = (y + coeff * pow(x, power, p)) % p
        shares.append((x, y))

    return shares, vv
```

From this [Useful LLL resource](https://crypto.stackexchange.com/a/86548), we can see that LLL can be used to solve any linear modular equation (a powerful framing for many crypto challenges). Now all we need to do is convert the polynomial into linear modular equations.

Flag: `SSMCTF{if_w3_4lll_d0Nt_s3lll_ST0NKS_c4n_0NlY_g0_uPpp}`