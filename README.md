## GNU GCC Toolchain

Bleeding edge [GNU GCC](https://gcc.gnu.org/) AArch64 systems. built from sources with latest binutils and glibc. These Builds (on master/main branch) are always made from the latest GCC sources rather than stable releases.

This toolchain AArch64 [AArch32 here](https://github.com/theradcolor/arm-linux-gnueabi.git). Built with Support for Link Time Optimization, -O3, --disable-nls and removed extras that we don't need.

### Getting the toolchain

Clone using git from this repo, As currently we don't have any mirror or a archived release.

```
$ git clone https://github.com/theradcolor/aarch64-linux-gnu --depth=1
```

> Note: This is continous updating repository made from the latest GCC sources rather than stable releases, if you want to use stable release of gcc clone the stable-gcc branch of this repository.

For stable gcc
```
$ git clone https://github.com/theradcolor/aarch64-linux-gnu -b stable-gcc --depth=1
```

>  Note: Also using depth flag (--depth=1) is recommended as repository size is large and will keep increasing in future updates.

### Using the toolchain

Export the `CROSS_COMPILE` in enviroment

```
$ export CROSS_COMPILE=<toolchain-path>/bin/aarch64-linux-gnu-
```

### Sources

Along with the compiler (GCC) which is built from latest sources, the GNU and other libraries and prerequisite are also been built from latest sources itself.

> GNU Compiler Collection (GCC) https://gcc.gnu.org/git.html

> GNU Binutils https://www.gnu.org/software/binutils/

> For Headers (LINUX KERNEL) https://www.kernel.org/

> GNU Multiple Precision Arithmetic Library (GMP) https://gmplib.org/

> Multiple-Precision Floating-Point Computations with Correct Rounding (MPFR) http://www.mpfr.org/

> GNU Complex Floating-Point Library with Exact Rounding (MPC) http://www.multiprecision.org/

> Integer Set Library (ISL) http://isl.gforge.inria.fr/

> GNU C Standard Library (GLIBC) https://www.gnu.org/software/libc/

> C Standard Library Intended for use on Embedded Systems (NEWLIB) https://sourceware.org/newlib/

### License

GCC is licensed under version 3 of the [GNU General Public License.](https://www.gnu.org/licenses/gpl-3.0.html)
The GCC runtime exception permits compilation of proprietary and free software programs with GCC and usage of free software plugins. The availability of this exception does not imply any general presumption that third-party software is unaffected by the copyleft requirements of the license of GCC. 
