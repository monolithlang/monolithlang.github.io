# Strings

Monolith have two builtin types for release one-byte string or multi-wide string.
Traditional one-byte string assigned with type string, multi-wide string only can have ustring data type with adjacent aliases. 

```rust
    // Simple double-quoted string.
    let str = "Hello World\n";

    // Raw double-quoted string.
    // \n\r\t literal will not be escaped.
    let rstr = r"Hello World \n\r\t"; // output: Hello World \n\r\t

    // Raw multiple double-quoted string.
    let mstr = r"My mistress’ eyes are nothing like the sun;
Coral is far more red than her lips’ red;
If snow be white, why then her breasts are dun;
If hairs be wires, black wires grow on her head.
I have seen roses damasked, red and white,
But no such roses see I in her cheeks;
And in some perfumes is there more delight
Than in the breath that from my mistress reeks.
I love to hear her speak, yet well I know
That music hath a far more pleasing sound;
I grant I never saw a goddess go;
My mistress when she walks treads on the ground.
And yet, by heaven, I think my love as rare
As any she belied with false compare.";

    let char               = 'A';            // uint8_t
    let onebyted   string  = "Hello World!"; // []uint8_t
    let multiwided ustring = "Hello World!"; // []uint32_t
```