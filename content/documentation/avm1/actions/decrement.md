+++
title = "Decrement"
description = "Decrement"
template = "page-documentation.html"
+++

- Action Code: `0x51`
- Stack: `1 → 1`
- SWF version: `5`

# Abstract AS2

```
@push(@pop() - 1);
```

# Adobe documentation

## ActionDecrement

ActionDecrement pops a value from the stack, converts it to number type, decrements it by 1, and pushes it
back to the stack.

| Field             | Type               | Comment                        |
|-------------------|--------------------|--------------------------------|
| ActionDecrement   | ACTIONRECORDHEADER | ActionCode = 0x51              |

ActionDecrement does the following:
1. Pops the number off of the stack.
2. Pushes the result on to the stack.
