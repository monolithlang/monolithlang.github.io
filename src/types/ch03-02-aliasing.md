# Aliasing

Each alias is subjected to strict checks for `_t` ending which indicates that it is a basic type (integer, unsigned, floating point, string, character, byte).

**_Builtin_** types list:
```go
rune

string  ustring

bool    byte

int8   int16   int32   int64   int128
uint8  uint16  uint32  uint64  uint128

float32    float64     float128
complex64  complex128  complex256

intsize  uintsize  void  empty
```

## Syntax

```c
// EBNF
type_decl = "type" ...;
```

_type_-declaration<br>
&nbsp;&nbsp;&nbsp;&nbsp;**type** ident ident;

## Example

```go
// real example
type intmax_t  int128;
type uintmax_t uint128;
```