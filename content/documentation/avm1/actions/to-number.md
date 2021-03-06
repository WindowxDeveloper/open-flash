+++
title = "ToNumber"
description = "ToNumber"
template = "page-documentation.html"
+++

- Action Code: `0x4a`
- Stack: `1 → 1`
- SWF version: `5`

# Abstract AS2

```
@push(+@pop());
```

# Adobe documentation

## ActionToNumber

Converts the object on the top of the stack into a number, and pushes the number back to the stack.
For the Object type, the ActionScript valueOf() method is invoked to convert the object to a Number type for
ActionToNumber. Conversions between primitive types, such as from String to Number, are built-in.

| Field             | Type               | Comment                        |
|-------------------|--------------------|--------------------------------|
| ActionToNumber    | ACTIONRECORDHEADER | ActionCode = 0x4A              |

ActionToNumber does the following:
1. Pops the object off of the stack.
2. Pushes the number on to the stack.
