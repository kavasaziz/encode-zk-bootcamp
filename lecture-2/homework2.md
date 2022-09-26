# Homework-2

1. Group / field theory

    > Take the set of bits B = {0,1} and the operation ⊕ with the following rules:
    > ```
    > 0 ⊕ 0 = 0
    > 0 ⊕ 1 = 1
    > 1 ⊕ 0 = 1
    > 1 ⊕ 1 = 0
    > ```
    > Does the set B and the operation `⊕` satisfy the group properties?

    To be considered a group this combination needs to have certain properties.

    - [x] Closure <br>
        As shown in the questions itself, any combination of binary operation gives a results which is also in set `B`.

    - [x] Associativity <br>
        Order of elements does not changes the result. Namely, `0 ⊕ 1 = 1 ⊕ 0`, or `0 ⊕ (0 ⊕ 1) = (0 ⊕ 0) ⊕ 1`.

    - [x] Identity element (= 0) <br>
        `0 ⊕ 0 = 0` and `1 ⊕ 0 = 1`. Therefore, `0` is identity element

    - [x] Inverse element <br>
        `1 ⊕ 1 = 0`, only element of one with the inverse of itself.

2. Modular arithmetic - you just need to find examples, you don't need to prove anything.
   1. Is it true that all odd squares are ≡ 1 (mod 8) ?
        All odds square are = $1 mod 8$ <br>
        $(2n-1)^2 mod 8 = 1$
   2. what about even squares (mod 8) ?
        All even squares = mod 8
        it looks like it is cyclic:
            $2^2 = 4 mod8$ <br>
            $4^2 = 0 mod8$ <br>
            $6^2 = 4 mod8$ <br>
            $8^2 = 0 mod8$ <br>
            $10^2 = 4 mod8$ <br>





3. Try out the vanity bitcoin address example at [asecurity](https://asecuritysite.com/blockchain/vanity) or the Ethereum [version](https://vanity-eth.tk/)

4. $\Omicron$ symbol represents the worst case space or time complexity of an algorithm. In terms of time,

    - $\Omicron(1)$ : means constant time, namely time required for an operation to be completed is independent of input size.
    - $\Omicron(\log n)$ : time required for an operation to be completed is proportional with logarithm of input size
    - $\Omicron(n)$ : time required for an operation to be completed is proportional with input size

5. In terms proof size, we are asking for space complexity, where $\Omicron(1)$ is better because size of proof will be independent of the input size.