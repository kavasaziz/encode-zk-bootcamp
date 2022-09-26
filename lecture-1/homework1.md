# Homework-1
## Maths Introduction
1. Working with the following set of integers S = {0,1,2,3,4,5,6}, what is
   1. `4+4` : $4+4=8; 1 \equiv 8 (mod 7)$
   2. `3x5` : $3x5 (mod 7) \equiv 1$
   3. `3^-1` :
      1. `Multiplicative Inverse`: Using Fermat's Theorem ($a \equiv a^p (mod p)$); $3^-1 mod 7 \equiv 5$ is multiplicative inverse. This can be easily proven by $3x5 (mod 7) \equiv 1$
      2. `Additive Inverse`: $-3(mod7) \equiv 4$, which can be proven as $3+4(mod7) \equiv 0$
2. For S = {0,1,2,3,4,5,6}, can we consider S and the operation + to be a group?

Simply a group is a set of elements {a,b,c,...} plus a binary operation, which is `+` (addition) in our case. To be considered a group this combination needs to have certain properties.

- [x] Closure
- [x] Associativity
- [x] Identity element (= 0)
- [x] Inverse element

Namely, `S` forms a group with `+` operator.

3. What is -13 mod 5?

$$-13(mod5) \equiv 2$$

## Use Cases
> Think of some use cases of ZKP. What problems are there when using zkps in real world situation?

- We can prove that we are a real person without sharing our identity card.
- We can prove that we have payed the tax without sharing bank receipt to tax authority.

???