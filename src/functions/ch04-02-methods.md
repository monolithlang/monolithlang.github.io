# Methods

Function can work with methods and be defined with methods. Methods may be responsible for a specific implementation of a data type, and also be determined by this very data type.

## Syntax

```go
func (method_name type) func_name() -> type { body }
func (method_name type) func_name() { body }
```

## Example

```go
struct user {
    first_name  string,
    second_name string,
};

// Setter
func (data user) set_first_name(v string) {
    data.first_name = v;
}

// Getter
func (data user) get_first_name() -> string {
    return data.first_name;
}
```