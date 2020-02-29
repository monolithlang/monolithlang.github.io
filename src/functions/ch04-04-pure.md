# Pure

A pure function is always deterministic and has no side effects. 

This means that the function cannot change static local, non-local data, and also there is no mutation of local static, non-local variables.

## Example

```go
#[[pure]]
func sum(a, b const int32) -> int32 {
    return a + b;
}
```