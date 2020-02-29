# Inlined

The function can be marked as an inline attribute, this will be a hint to the compiler that the body of the function can be substituted at each point of the call, instead of generating a call code.

## Example

```go
#[[inline]]
func mul(a, b int32) -> int64 {
    return (int64)a * b;
}
```