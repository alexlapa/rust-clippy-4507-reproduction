
```
$cargo +nightly clippy --all -- -D clippy::pedantic -D warnings

error: integer type suffix should be separated by an underscore
 --> src/lib.rs:3:1
  |
3 | #[wasm_bindgen]
  | ^^^^^^^^^^^^^^^ help: add an underscore: `#[wasm_bindg_u32`
  |
  = note: `-D clippy::unseparated-literal-suffix` implied by `-D clippy::pedantic`
  = help: for further information visit https://rust-lang.github.io/rust-clippy/master/index.html#unseparated_literal_suffix

error: integer type suffix should be separated by an underscore
 --> src/lib.rs:3:1
  |
3 | #[wasm_bindgen]
  | ^^^^^^^^^^^^^^^ help: add an underscore: `#[wasm_bindg_u32`
  |
  = help: for further information visit https://rust-lang.github.io/rust-clippy/master/index.html#unseparated_literal_suffix

error: aborting due to 2 previous errors

error: Could not compile `add`.

```

```
$cargo +nightly clippy -V
clippy 0.0.212 (aeadf15 2019-09-03)
```