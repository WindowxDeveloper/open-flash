+++
title = "Primitives"
description = "Primitive definition"
template = "page-documentation.html"
+++

# PADDING

Any sequence of bytes, including nothing. `PADDING` mostly used after
useful date to reach the expected size. There is no value associated with
padding itself.

When emitting SWF data, `PADDING` should be minimized: use no padding at all
or the shortest allowed padding. If padding is required, it should be filled with
zeros.

# UINT8

Unsigned 8-bit integer.

# LE_UINT16

Unsigned 16-bit integer in little-endian representation.
This is the main type used for 16-bit values.

# BE_UINT16

Unsigned 16-bit integer in big-endian representation.
This type is only rarely used for 16-bit values.

# LE_UINT32

Unsigned 32-bit integer in little-endian representation.

# NUL_UTF8

An unbounded nul-terminated UTF-8 buffer.

Buffers containing encoding errors are invalid.

This encodes a string as a sequence of unicode codepoints, except for the codepoint `0`.

# LE_FLOAT32

Based on the documentation of the modulo action, Adobe uses `0x7FC00000` as the canonical NaN representation.
