# 2.6 If statement

Traditional `if` statement, with else-if branch.
```rust
    let x = 10;
    if (x > 10) {
        x = -1;
    } else if (x < 10) {
        x += x * x;
    } else {
        x = 0;
    }
    std::printf("%d", x) // 0
```

`if` can be used as an expression.
```rust
    let a, b = 0, 10;
    let x = if ((a + b) == 10) {
        100
    } else {
        -1
    } 
    std::printf("%d", x); // 100
```
