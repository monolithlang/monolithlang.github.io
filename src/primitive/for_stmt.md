# 2.7 For statement

`for` statement use conceptions from Go, no needs for `loop`, `while`, `do`. One looping construction.

```rust
    let n = 0;
    
    // infinity loop
    for {
        n++;
    }
    
    // do-while replacement
    for {
        if (n == 0xff) {
            break;
        } else {
            n++;
        }
    }
    
    // loop for 10 times
    for (let i = 0; i < 10; i++) {
        std::printf("Hello!");
    }
```