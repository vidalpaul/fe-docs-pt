# `continue` statement


> **<sup>Syntax</sup>**\
> _ContinueStatement_ :\
> &nbsp;&nbsp; `continue`

The `continue` statement can only be used within a [`for`] or [`while`] loop and causes the immediate termination of the current iteration, returning control to the loop head.

If used within nested loops the `continue` statement is associated with the innermost enclosing loop.

An example of a `continue` statement used within a [`while`] loop.

```python
contract Foo:

    pub fn bar() -> u256:
        let sum: u256
        while sum < 10:
            sum += 1

            if some_skip_condition():
                continue

        return sum

    fn some_skip_condition() -> bool:
        # some complex logic
        return true
```

An example of a `continue` statement used within a [`for`] loop.

```python
contract Foo:

    pub fn bar(values: Array<u256, 10>) -> u256:
        let sum: u256
        for i in values:
            sum = sum + i

            if some_skip_condition():
                continue

        return sum

    fn some_skip_condition() -> bool:
        # some complex logic
        return true
```

[`for`]: statement_for.md
[`while`]: statement_while.md