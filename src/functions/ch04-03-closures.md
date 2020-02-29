# Closures

Closures use C++ and Go mixed model.
Closures can capture local environment of standart or reference values.

## Syntax

```go
func (params) -> type { body }
func (params) { body }
func () { body }
```

## Example

```rust
    let x = 0;
    let y = 0;
    let z = 0;

    // We capture local scope variables x, y, z, and we take x0, y0, z0 argument.
    let closure = func(x0, y0, z0 int32) -> int64 {
        x = x0 * 2;
        y = y0 * 2;
        z = z0 * 2;

        return (int64)x * y * z;
    }(10, 20, 30); 

    // Or
    closure(10, 20, 30);
```

```go
func sq_fmul(x, y, z int) -> func() -> int64 {
    return func() -> int64 {
        let r = x * z * z;
        return (int64)r;
    };
}
```