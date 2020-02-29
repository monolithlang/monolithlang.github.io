# Complex

Complex functions are functions implemented without methods.

> **_Note:_** `entry` function always must return `int64` value.

## Syntax

```c
// EBNF
func_decl = [ "pub" ] "func", ident, ...;
```

_func_-declaration<br>
&nbsp;&nbsp;&nbsp;&nbsp;[**_pub_**] **_func_** ( expression ) statement

## Example

```go
// Complex function
func print() {
    std::printf("%s", "Hello Simple");
}

// Complex function with arguments
func print_msg(msg string) {
    std::printf("%s", msg);
}

// Complex function with returned arguments
func mul(a, b int32) -> int64 {
    return (int64)a * b;
}

// Complex function with multiple return arguments (tuple)
func mul_sq(x, y, z int32) -> (int64, int64) {
    return ((int64)x * z, (int64)y * z);
}

func entry() -> int64 {
    print();
    print_msg("Hello World");
    
    let r = mul(5, 5); // 25
    let r_sq0, r_sq1 = mul_sq(12, 24, 2); // 24, 48
    return 0;
}
```
