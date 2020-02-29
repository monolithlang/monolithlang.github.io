# break

The `break` keyword means stopping and exiting from the current loop.

## Syntax

```ebnf
break = "break" ;
```

## Example

```rust
    let n = 0;
    for {
        if (n >= 128) {
            break; // stop and exit from current loop
        }
        n++;
    }
```