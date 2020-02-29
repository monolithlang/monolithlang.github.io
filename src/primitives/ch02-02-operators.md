# Operators

## Example (Lexer)

```rust
pub enum tokens (int32) {
    ...

    PLUS,  // +
    MINUS, // -
    DIV,   // /
    MUL,   // *
    MOD,   // %
    INC,   // ++
    DEC,   // --

    BITWISE_XOR,    // ^
    BITWISE_OR,     // |
    BITWISE_AND,    // &
    BITWISE_NOT,    // ~
    BITWISE_LSHIFT, // <<
    BITWISE_RSHIFT, // >>

    LOGICAL_OR,  // ||
    LOGICAL_AND, // &&
    LOGICAL_NOT, // !

    OP_EQUAL,         // ==
    OP_NEQUAL,        // !=
    OP_GREATER,       // <
    OP_LESS,          // > 
    OP_GREATER_EQUAL, // <=
    OP_LESS_EQUAL,    // >=
    OP_THREEWAY,      // <=>
};
```