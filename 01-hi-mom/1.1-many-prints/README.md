# 1.1 Many Prints

Rust has some built-in macros for displaying text on the console.

- `println!` - :fire: 10/10, appends a new line
- `print!` - writes output to the console, but nothing is appended
- `eprintln!` - similar to `println!`, but is printed to Standard Error (std::err) instead of Standard Output
- `eprint!` - similar to `print!`, but is printed to Standard Error (std::err)

<br />

`main.rs`
```rs
fn main() {
  println!("I didn't eat the whole pizza");
  print!("... trust me!");
  
  // the following will only be caught by stderr
  // eprintln!("error: liar!")
}
```

**Output**
```
I didn't eat the whole pizza... trust me!
```
