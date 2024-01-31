# zkllvm-unroll
Unroll for loops with integer literal bounds using an attribute-like macro `unroll_for_loops` that can be applied to functions.
This macro looks for loops to unroll and unrolls them at compile time.

# Example
```
#[unroll_for_loops]
fn main() {
    println!("matrix = ");
    for i in 0..10 {
        for j in 0..10 {
            print!("({:?}, {:?})", i, j);
        }
        println!("");
    }
}
```

# License
This repository is licensed under either of

- Apache License, Version 2.0, (LICENSE-APACHE or https://www.apache.org/licenses/LICENSE-2.0)
- MIT License (LICENSE-MIT or https://opensource.org/licenses/MIT)

at your option.

# The original repository: https://gitlab.com/elrnv/unroll
