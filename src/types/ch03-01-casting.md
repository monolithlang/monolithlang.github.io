# Casting

The type casting syntax equals to C casting syntax, but a slightly different philosophy. You cannot cast float to byte or integer.

## Syntax

```c
// EBNF
cast_expr = ...;
```

_cast_-expression<br>
&nbsp;&nbsp;&nbsp;&nbsp;**(type_expr)** expr

## Example

```rust
    let x int64;
    let y int128;
    let z uint128;

    let r = (int128)x * (uint128)y * z;
    let r0 &uint128;
    r0 = &z;
    r0 = (&uint128)&z;
```