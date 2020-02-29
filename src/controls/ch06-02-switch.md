# switch

## Syntax

```c
// EBNF
switch_stmt = "switch", "(", expr, ")", block_stmt;
```

_switch_-statement<br>
&nbsp;&nbsp;&nbsp;&nbsp;**_switch_** ( expression ) statement

_label_-statement<br>
&nbsp;&nbsp;&nbsp;&nbsp;
_**case**_ expression: statement<br>
&nbsp;&nbsp;&nbsp;&nbsp;**_default_**: statement<br>

## Example

```go
    let name = "Jack";
    switch (name) {
        case "Jack":
            std::printf("%s", "I know you, Jack");
        case "Abram":
            std::printf("%s", "I know you, Abram");
        default:
            std::printf("I dont know you, %s", name);
            break;
    }
```

