# panic

`panic` is triggered when the program has fatal errors or panic is triggered deliberately to debug the program.

## Example

```rust
    let x = 0;
    if (x == 0) {
        std::panic("`x` cannot be zero!");
    }
```