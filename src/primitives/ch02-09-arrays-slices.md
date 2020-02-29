# Arrays & Slices

Arrays is a fixed-sized block, slices is a unfixed-sized block which can growable (expanded) at runtime.

## Example

```rust
    // Array with fixed-sized block.
    let arr [10]byte;
    arr[0] = 0x9ef;
    arr[9] = 0xff;
    arr[12] = 0x5eb; // error: index out of bounds

    // Slice with unfixed-size block.
    let slice []byte;
    slice[0] = -1;       // ok
    slice[10] = 0x3f;    // ok
    slice[1000] = 0x9ef; // ok
```