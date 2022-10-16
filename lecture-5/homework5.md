# Homework-5
## Q1
In simplest words, recursive functions are the functions calling itself. This is programming approach preferred in cairo instead of loops because **Cairo supports a read-only nondeterministic memory**. In other words, the value for each memory cell is chosen by the prover, but it cannot change over time (during a Cairo program execution). Therefore, we cannot use variables which is updated in every stage.

The code used in Cairo playground given below
```cairo
%builtins output

from starkware.cairo.common.serialize import serialize_word

func compute_sum(n: felt) -> (sum: felt) {
    if (n == 0) {
        // When 0 is reached, return 0.
        return (sum=0);
    }

    // Otherwise, call `compute_sum` recursively to compute 1 + 2 + ... + (n-1).
    let (sum) = compute_sum(n=n - 1);
    // Add the new value `n` to the sum.
    let new_sum = sum + n;
    return (sum=new_sum);
}

func main{output_ptr: felt*}() {
    let (res) = compute_sum(n=10);

    // Output the result.
    serialize_word(res);
    return ();
}
```

## Q2
Tailing recursion is a type of recursive programming approach in which recursive function calls are made in the last statement of function. **Therefore, this is not a tailing recursion example.**

<details close>
<summary>Further non-tailing recursion examples</summary>

```cairo
func calculate_sum(n : felt) -> (sum : felt) {}
    if (n == 0) {
        return (sum=0,);
    }

    let (sum) = calculate_sum(n=n - 1);
    let new_sum = sum + n;
    return (new_sum,);
}
```
</details>


<details close>
<summary>Further tailing recursion examples</summary>

```cairo
func calculate_sum(n : felt) -> (sum : felt) {
    if (n == 0) {
        return (0,);
    }
    return (calculate_sum(n-1) + n,);
}
```
</details>

## Q3
While creating an a wallet, system creates and deploys a contract.

> :bulb: **TIP:** Take a look at [gitpod](https://gitpod.io/#https://github.com/ExtropyIO/ZeroKnowledgeBootcamp).
