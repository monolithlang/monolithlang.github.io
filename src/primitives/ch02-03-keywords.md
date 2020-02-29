# Keywords

## Example (Lexer)

```rust
pub enum tokens (kind_t) {
    ...

    KW_AS,        // as
    KW_ASM,       // asm
    KW_ASSERT,    // assert
    KW_LET,       // let
    KW_BREAK,     // break
    KW_CASE,      // case
    KW_CONST,     // const
    KW_CONTINUE,  // continue
    KW_DEFER,     // defer
    KW_DEFAULT,   // default
    KW_DEBUG,     // #debug
    KW_EXTERN,    // extern
    KW_EXTEND,    // extend
    KW_ENUM,      // enum
    KW_ELSE,      // else
    KW_EMPTY,     // empty
    KW_MAP,       // map
    KW_MODEL,     // model
    KW_FALSE,     // false
    KW_FOR,       // for
    KW_OPTION,    // option

    KW_FUNC,      // func
    KW_GOTO,      // goto
    KW_IF,        // if
    KW_LIB,       // #lib
    KW_LOAD,      // #load
    KW_IN,        // in
    KW_INTERFACE, // interface
    KW_RETURN,    // return
    KW_SIZEOF,    // sizeof
    KW_OFFSETOF,  // offsetof
    KW_ALIGNOF,   // alignof
    KW_STRUCT,    // struct
    KW_SWITCH,    // switch
    KW_STATIC,    // static
    KW_TRUE,      // true
    KW_TYPE,      // type
    KW_UNION,     // union
    KW_PUB,       // pub
};
```