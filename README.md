# Rust stm32f103c6t6 starter
Preconfigured package with scripts to develop stm32f103c6t6 Blue Pill microcontroller with serial adapter.

## Prerequisites

Linux c:

Install stm32flash:

https://sourceforge.net/p/stm32flash/wiki/Home/

or (on debian) ``` apt install stm32flash ```

Install cargo-make:
``` cargo install cargo-make ```

Install rust thumbv7m-none-eabi target:
``` rustup target install thumbv7m-none-eabi ```

## Usage
Build and flash: ``` cargo make deploy [serialport] ```

Only build: ``` cargo make build-release ``` and  ``` cargo make build-objcopy ```

Only flash: ``` cargo make flash [serialport] ```

Rememeber to set BOOT 0 jumper to 1 and reset. After flash set jumper to O and reset.

## Credits
Code in src taken from:
https://github.com/stm32-rs/stm32f1xx-hal

## License
MIT

