# continue

The `continue` keyword means a specific continuation (skipping) of the loop.

## Syntax

```ebnf
continue = "continue" ;
```

## Example

This is an infinitive example.

```rust
    let n = 0;
    for {
        if (n >= 128) {
            break;
        } else {
            continue; // go to start of loop
        }
        n++; // will not be executed, because we skip the loop
    }
```