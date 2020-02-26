# Functions

> **WARNING!** Function can have default values, but cannot be overloaded.

Function without any arguments and returned values.
```go
func nosense() -> {}

```

Primitive function with two arguments but without default values.
```go
func mul(a, b int32) -> int64 {
    return (int64)a * b;
}
```

Primitive function with arguments and default values.
```go
func mul_by_default_64(a, b int32 = 64) -> int64 {
    return (int64)a * b;
}
```