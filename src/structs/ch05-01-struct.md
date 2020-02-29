# struct

## Syntax

```c
// EBNF
struct_decl = "struct", ident, "{", ... "};";
```

_struct_-declaration<br>
&nbsp;&nbsp;&nbsp;&nbsp;**struct** ident statement

```rust
struct structure_name {
    field_name data_type,
    ...
};
```

## Example
```rust
struct lexer {
    ch                rune,
    offset            int32,
    rd_offset         int32,
    line_offset       int32,
    line_start_offset int32,
};

const INVALID int32 = -1;

func entry() -> int64 {
    let obj = &lexer{
        ch                = 0,
        offset            = 0,
        rd_offset         = 0,
        line_offset       = 10,
        line_start_offset = 25,
    };
    return 0;
}
```
