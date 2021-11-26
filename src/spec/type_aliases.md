# Type aliases

> **<sup>Syntax</sup>**\
> _TypeAlias_ :\
> &nbsp;&nbsp; `type` [IDENTIFIER]&nbsp;`=` [_Type_]

A _type alias_ defines a new name for an existing [type]. Type aliases are
declared with the keyword `type`.

For example, the following defines the type `BookMsg` as a synonym for the type
`u8[100]`, a sequence of `100` `u8` numbers which is how sequences of bytes are represented in Fe.

```
type BookMsg = Array<u8, 100>
```

[IDENTIFIER]: identifiers.md
[_Type_]: types.md
[type]: types.md