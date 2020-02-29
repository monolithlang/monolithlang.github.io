# lib

Uses the understanding of the “library” which can be implemented by the second side, and can also be connected as an addition to the standard program.

There are two build states: _program_ and _library_.
- _KIND_PROGRAM_ = "program";
- _KIND_LIBRARY_ = "library";

Entry (main) program always are "entry.m" with "entry" library which can load another external libraries.

## Syntax

```c
// EBNF
lib_decl = "#lib", ident, ";";
```

_lib_-declaration<br>
&nbsp;&nbsp;&nbsp;&nbsp;**#lib** ident

## Example

_math.m_
```go
// Define new `math library
#lib math;

// `mul` function ...
pub func mul(a, b int32) -> int64 {
    return (int64)a * b;
}
```

_entry.m_
```rust
#lib entry;
#load "std";
#load "math" as m; // load external library `math` with `m` alias

func entry() -> int64 {
    let r = m::mul(10, 10); // 100
    std::printf("Resulting value: %d", r);
    return 0;
}
```
