# Constants & Modifiers

`const` is a immutable value which cannot be modified at runtime.

## Example 

```rust
const MAGIC = 0x55;

func entry() -> int64 {
    MAGIC = 0; // error: cannot modify constant value

    let const square_param = 0x64; 
    square_param = square_param * square_param; // error: cannot modify constant value

    return 0;
}
```

_counter.m_

```rust
// Counter library.
#lib counter;

// Static variable with public modifier.
pub static COUNTER int32 = 0;
```

_entry.m_

```rust
#lib entry;
#load "counter" as count32;

// We can increment COUNTER variable by another library.
func inc() {
    count32::COUNTER++;
}

func entry() -> int64 {
    for {
        if (COUNTER >= 128) {
            break;
        }
        inc(); // increment COUNTER.
    }
    return 0;
}
```