+++
title = "TypeOf"
description = "TypeOf"
template = "page-documentation.html"
+++

- Action Code: `0x44`
- Stack: `1 → 1`
- SWF version: `5`

# Abstract AS2

```
@t0 = @pop();
@push(typeof @t0);
```

# Adobe documentation

## ActionToString

ActionTypeOf pushes the object type to the stack, which is equivalent to the ActionScript TypeOf() method. The
possible types are:
- `number`
- `boolean`
- `string`
- `object`
- `movieclip`
- `null`
- `undefined`
- `function`

| Field             | Type               | Comment                        |
|-------------------|--------------------|--------------------------------|
| ActionTypeOf      | ACTIONRECORDHEADER | ActionCode = 0x44              |

ActionTypeOf does the following:
1. Pops the value to determine the type of off the stack.
2. Pushes a string with the type of the object on to the stack.
