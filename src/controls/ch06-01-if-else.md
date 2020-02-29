# if/else

## Syntax

```c
// EBNF
if_stmt = "if", "(", expr, ")", block_stmt;
```

_if_-statement<br>
&nbsp;&nbsp;&nbsp;&nbsp;**if** ( expression ) statement

_label_-statement<br>
&nbsp;&nbsp;&nbsp;&nbsp;
**_case_** expression: statement<br>
&nbsp;&nbsp;&nbsp;&nbsp;**_default_**: statement<br>
    
## Example

```rust
    let x = 0;
    if (x > 0) {
        x++;
    } else if (x < 0) {
        x--;
    } else {
        x = x * x;
    }
```