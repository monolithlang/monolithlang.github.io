# Literals

Monolith have string `""`, character `''`, integer `0`, float `0.0`, boolean `true`, unit `() {}` literals.

Integer can be expanded by using a octal, binary, hexadecimal notation:
- Octal notation `0o` prefix, `0o1234567`
- Binary notation `0b` prefix, `0b00010001`
- Hexadecimal notation `0x` prefix, `0x9ef`, `0xff`, `0x53E2bf`

Underscores can be inserted in integer literals for more readability, eg: `1_200` is the same as `1200`.

```rust
func entry() -> int64 {
    let octal       = 0o1234567;
    let binary      = 0b00010001;
    let hexadecimal = 0x9ef;

    let str     = "";
    let integer = 0;
    let float   = 0.0;
    let boolean bool = true;
    return 0;
}
```