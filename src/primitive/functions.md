# 2.2 Functions

> WARN: Function can have default values, but cannot be overloaded.

Function without any arguments and returned values.
```go
func nosense() -> {}
```

Primitive function with two arguments but without default values.
```go
#[[inline]]
func mul(a, b int32) -> int64 {
    return (int64)a * b;
}
```

Primitive function with arguments and default values.
```go
#[[inline]]
func mul_by_default_64(a, b int32_t = 64) -> int64_t {
    return (int64_t)a * b;
}
```