
On the main branch this brings up nushell with just nu_cmd_lang and nothing else...

Start out with a copy of the src directory from nushell...
The rest of the crates are pulled in from crates.io

The files that need modified are

* Cargo.toml
* src/main.rs

```rust
use nu_cmd_lang::create_default_context;
```
