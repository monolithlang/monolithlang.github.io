# Annotations

Annotations are used for easier reading and understanding of code. Annotations are useful only for variables the practical use of annotations is possible when writing low-level constructions and functions where the role of understanding the input / output parameter is important.

Annotations can be of two types: input, output.
I love and respect old school!

## Syntax

```go
[ __In__ ] params ...
[ __Out__ ] params ...
```

## Example

```rust
struct mem_pool {
    // __In__ : input annotation.
    __In__  pool *intsize,

    // __Out__ : ouput annotation.
    __Out__ out_pool *void,
};
```