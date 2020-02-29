# Comments

Comments are divided into two types: **regular** and **documentary**. 

Regular comments are ignored by the compiler, and the documentation comments used for generating project documentation.

## Syntax

* Regular comment which are ignored by the compiler:
    - `// Oneline comment for newline \n`
    - `/* Multiline comment by the block delimiter */`
* Documentation comment which will be parsed:
    - `/// Oneline documentation comment for newline \n`

## Example

```rust
// Oneline comment.
// Oneline but with multiline style.

    // Copyright (c) 2019 0x9ef. All rights reserved.
    // Use of this source code is governed by an MIT license
    // that can be found in the LICENSE file.

/* Multiline comment. */

    /** 
    * Copyright (c) 2019 0x9ef. All rights reserved.
    * Use of this source code is governed by an MIT license 
    * that can be found in the LICENSE file.
    */

/// `func` documentation comment
/// ...

    /// Copyright (c) 2019 0x9ef. All rights reserved.
    /// Use of this source code is governed by an MIT license
    /// that can be found in the LICENSE file.
```