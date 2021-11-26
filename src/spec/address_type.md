# Address Type

The `address` type represents a 20 byte Ethereum address.

Example:

```Python
contract Example:
  # An address in storage
  someone: address

  fn do_something():
    # A plain address (not part of a tuple, struct etc) remains on the stack
    dai_contract: address = address(0x6b175474e89094c44da98b954eedeac495271d0f)
```