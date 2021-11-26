# `break` statement


> **<sup>Syntax</sup>**\
> _BreakStatement_ :\
> &nbsp;&nbsp; `break`

The `break` statement can only be used within a [`for`] or [`while`] loop and causes the immediate termination of the loop.

If used within nested loops the `break` statement is associated with the innermost enclosing loop.

An example of a `break` statement used within a [`while`] loop.

```python
contract Foo:

    pub fn bar() -> u256:
        let sum: u256
        while sum < 10:
            sum += 1

            if some_abort_condition():
                break

        return sum

    fn some_abort_condition() -> bool:
        # some complex logic
        return true
```

An example of a `break` statement used within a [`for`] loop.

```python
contract Foo:

    pub fn bar(values: Array<u256, 10>) -> u256:
        let sum: u256
        for i in values:
            sum = sum + i

            if some_abort_condition():
                break

        return sum

    fn some_abort_condition() -> bool:
        # some complex logic
        return true
```

[`for`]: statement_for.md
[`while`]: statement_while.md