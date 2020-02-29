# Alone attribute

Attributes allow you to specify additional information for various constructs such as data types, functions, variables, and so on. This information can be used by the hint compiler to generate more effective code.

## Syntax

```c
attr_decl = "#", "[" [ ... ] "]";
```

## Example

```go
// This function with a = 10, b = 10 will be inlined to 
//     return (int64)10 * 10;
#[[inline]]
func mul(a, b int32) -> int64 {
    return (int64)a * b;
}

// empty attribute means that function has no body with any logical elements, does not return any values, don't not have any arguments. 
#[[empty]]
func empty() {}

// noreturn attribute means that function doesnt have return statement and return variables.
#[[noreturn]]
func nosense(a, b int32) {
    let _ = a + b; // nosense
}

// pure attribute means that function is pure (determined, without any side-effects) by default.
#[[pure]]
func pure_calc(x, y const int32) -> int64 {
    return (int64)x * y;
}
```