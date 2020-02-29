# union

## Syntax

```c
// EBNF
union_decl = "union", ident, "{", ... "};";
```

_union_-declaration<br>
&nbsp;&nbsp;&nbsp;&nbsp;**union** ident statement

```rust
union union_name {
    field_name data_type,
    ...
};
```

## Example
```rust
union mem_pool {
    __permitted_chunk0 int16,
    permitted_chunk1 int32,
};

func entry() -> int64 {
    let obj = &mem_pool{
        __permitted_chunk0 = 0xff,
    };
    obj.permitted_chunk1 = 0; // ERR
    return 0;
}
```