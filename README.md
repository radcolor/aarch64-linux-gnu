# GNU GCC Toolchain

Bleeding edge GNU GCC toolchains built from sources with latest binutils and glibc.

## Getting the toolchain

Clone using git
```
$ git clone https://github.com/theradcolor/aarch64-linux-gnu --depth=1
```

> Note: This is continous updating repository made from the latest GNU's GCC sources rather than stable releases, so if you want to use the stable release of gcc clone the stable-gcc branch of this repository

For stable gcc
```
$ git clone https://github.com/theradcolor/aarch64-linux-gnu -b stable-gcc --depth=1
```

For ARM, checkout https://github.com/theradcolor/arm-linux-gnueabi.git

For x86_64, checkout https://github.com/theradcolor/x86_64-linux-gnu.git

## Using the toolchain

Export the `CROSS_COMPILE` in enviroment

```
$ export CROSS_COMPILE=<toolchain-path>/bin/aarch64-linux-gnu-
```

## License

GCC is licensed under version 3 of the [GNU General Public License.](https://www.gnu.org/licenses/gpl-3.0.html)
The GCC runtime exception permits compilation of proprietary and free software programs with GCC and usage of free software plugins. The availability of this exception does not imply any general presumption that third-party software is unaffected by the copyleft requirements of the license of GCC. 