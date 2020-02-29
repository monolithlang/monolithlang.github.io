# for

## Syntax
```c
// EBNF
for_stmt = ...;
```

_for_-statement<br>
&nbsp;&nbsp;&nbsp;&nbsp;**_for_** ( expression ) statement

_control_-statement<br>
&nbsp;&nbsp;&nbsp;&nbsp;
_**break**_;<br>
&nbsp;&nbsp;&nbsp;&nbsp;**_continue_**;<br>
&nbsp;&nbsp;&nbsp;&nbsp;**_fallthrough_**;

## Example

```rust
    // Infinity loop
    let n int32;
    for {
        n++;
        if (n >= 128) {
            break; // n == 128 true
        }
    }

    // Conditional statement
    for (n < 256) {
        n++;
    }

    // Conditional statement with delclaration body
    for (let i = 0; i <= 512; i++) {
        n++;
    }
```