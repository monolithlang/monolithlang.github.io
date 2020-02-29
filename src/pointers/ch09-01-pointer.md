# Pointers

Pointers are useful, but at some points pointers should be avoided and references should be used instead. 

1. The first and most important reason is the null pointer, dereferencing the null pointer will cause the program to crash.
2. A dangling pointer which refers to an invalid memory block is also possible. This occurs when the object is deleted or moved without pointers to pointers to zero.
3. A reference unlike a pointer cannot be uninitialized.
## Example

```rust
    let p *int32; // int32 pointer
    let x, y, z = 10, 20, 30;
    p = &x; // *p now 10
    p = &y; // *p now 20
    p = &z; // *p now 30
```