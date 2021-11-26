# `revert` statement


> **<sup>Syntax</sup>**\
> _RevertStatement_ :\
> &nbsp;&nbsp; `revert` [_Expression_]<sup>?</sup>

The revert statement is denoted with the keyword `revert`. Evaluating a `revert`
statement will cause to revert all state changes made by the call and return with an revert error to the caller. A revert statement may be followed by an expression that evaluates to a [struct] in which case the struct is encoded as revert data as defined by [EIP-838].

An example of a `revert` statement without revert data:

```
contract Foo:
    fn transfer(self, to : address, value : u256):
        if not self.in_whitelist(to):
            revert
        # more logic here
```

An example of a `revert` statement with revert data:

```
contract Foo:
    fn transfer(self, to : address, value : u256):
        if not self.in_whitelist(to):
            revert ApplicationError(code=5)
        # more logic here
```

[_Expression_]: expressions.md
[struct]: structs.md
[EIP-838]: https://github.com/ethereum/EIPs/issues/838