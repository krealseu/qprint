# A macro quick print variable  

## Example
```
Cargo.toml
[dependencies]
qprint = {git="https://github.com/krealseu/qprint.git"}


src.rs
use qprint::println as qprintln;

fn print(){
    let current_dir = std::env::current_dir();
    let temp_dir = std::env::temp_dir();
    qprint::println!(current_dir);
    qprintln!(current_dir,temp_dir);
}
```
