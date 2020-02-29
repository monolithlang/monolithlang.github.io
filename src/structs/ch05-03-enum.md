# enum

## Syntax

```c
// EBNF
enum_decl = "enum", ident, [ "(" ident ")" ] "{", ... "};";
```

_enum_-declaration<br>
&nbsp;&nbsp;&nbsp;&nbsp;**enum** ident [ (type) ] statement

```rust
enum ident {
    VALUE, 
    ...
}; // int32 by default

enum ident (type) {
    VALUE, 
    VALUE0 = 200,
    ...
}; // type
```

## Example

```rust
enum colors {
    RED,
    GREEN,
    BLUE,
}; // int32

enum colors (int8) {
    RED, GREEN, BLUE,
}; // int8
```
