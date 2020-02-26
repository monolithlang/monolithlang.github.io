# Variables

Variables only are declared with `let` keyword. `let` statement support multiple-variable declaration.

**Note:** let only means a LOCAL declaration inside of function. If you want to declare constant or static variable outside of function, you must use:

`const IDENT [type] = value;` | `static IDENT [type] = value;` without `let` keyword.

```rust
    // Simple `let` statement. 
    // Automatically assigned `int32` type with `0` literal.
    let x = 0; // int32

    // `let` statement with no value. 
    // Between that `let` statement have default value assignment. 
    let y int32; // int32 with 0 literal

    // `let` statement with forced type expression.
    let z uint64 = 0;   // uint64
    let z_ = (uint64)0; // uint64 with forced type casting
    
    // `let` statement with multiple variable declaration.
    let a, b, c = 0, (int64)0, ""; // int32, int64, string
```