# load

`load` is an improved `#include` from C, but have another included scope. Unused functions, constants, variables, etc will not be componed into a static object/executable file.

## Syntax

```c
// EBNF
load_decl = "#load", string [ "as", ident ] ";";
```

_load_-declaration<br>
&nbsp;&nbsp;&nbsp;&nbsp;**#load** ident [ as ident ]

## Example

```c
#load "std";           // std
#load "winapi" as w32; // w32 alias, uses w32::

func entry() -> int64 {
    return 0;
}
```