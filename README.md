
There is one extra branch here besides main and that is
 * nucmdshell

 The main branch has just nu-cmd-lang with no table viewer.

 The nucmdshell branch has the table viewer which can be tested with the following 2 commads..

 * version
 * help commands

On the main branch this brings up nushell with just nu_cmd_lang and nothing else...

### To build this repo from scratch after each release

Start out with a copy of the src directory from nushell...
The rest of the crates are pulled in from crates.io

The files that need modified are

* Cargo.toml
* src/main.rs

```rust
use nu_cmd_lang::create_default_context;
```
