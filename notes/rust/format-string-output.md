# Format string output  

When displaying a string, format the output with [arguments](https://doc.rust-lang.org/std/fmt/).  

In this example, each number will have at least a width of two characters. If necessary, a zero will be prepended. 

```rust
// Where hours, minutes are of type i32
write!(f, "{:02}:{:02}", hours, minutes)
```

See [width arguments](https://doc.rust-lang.org/std/fmt/#width).
