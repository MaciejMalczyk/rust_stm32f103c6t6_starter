# Rust stm32f103c6t6 starter
Preconfigured package with scripts to develop stm32f103c6t6 Blue Pill microcontroller with serial adapter.

## Usage
To flash use:
https://sourceforge.net/p/stm32flash/wiki/Home/
or install it from your package manager, f. e. "apt install stm32flash".

To build type: cargo run-script build. This will generate binary file in the root of the crate.

To flash: set BOOT0 to 1, reset, and then type: cargo run-script flash. Next swap BOOT0 jumper to 0 and reset.

## Credits
Code in src taken from:
https://github.com/stm32-rs/stm32f1xx-hal

## License
MIT

