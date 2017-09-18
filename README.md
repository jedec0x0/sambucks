### Not a cryptocurrency -- a revolution  

`"Cash rules everything around me. C.R.E.A.M. Get the money. Dolla dolla bill ya'll" - Method Man`

Imagine a world where transactions are cleared instantly, anonymously, and irreversibly.  Sambucks are inspired.  They're more than a protocol or a few lines of code.  They are a way of thinking -- of living.  This is just the beginning.  Buckle up.  

But first, Chris needs to help me compile it.

Here's what we got to do:

**1. Build the binaries and print a gensis block** (src/CryptoNoteConfig.h)

We have to compile the binaries as is and run the daemon with the `--print-genesis-tx` argument.  It will print the genesis block transaction.

Example:
```
sambucksd --print-genesis-tx
```

**2. Copy the printed transaction hash** (src/CryptoNoteConfig.h)

Copy the tx hash that has been printed by the daemon to `GENESIS_COINBASE_TX_HEX` in `src/CryptoNoteConfig.h`

Example:
```
const char GENESIS_COINBASE_TX_HEX[] = "013c01ff0001ffff...785a33d9ebdba68b0";
```

**3. Recompile the binaries**

Recompile everything again. Then it is time to change the world.


## Here is the guidance of building

### On *nix

Dependencies: GCC 4.7.3 or later, CMake 2.8.6 or later, and Boost 1.55.

You may download them from:

* http://gcc.gnu.org/
* http://www.cmake.org/
* http://www.boost.org/
* Alternatively, it may be possible to install them using a package manager.

To build, change to a directory where this file is located, and run `make`. The resulting executables can be found in `build/release/src`.

**Advanced options:**

* Parallel build: run `make -j<number of threads>` instead of `make`.
* Debug build: run `make build-debug`.
* Test suite: run `make test-release` to run tests in addition to building. Running `make test-debug` will do the same to the debug version.
* Building with Clang: it may be possible to use Clang instead of GCC, but this may not work everywhere. To build, run `export CC=clang CXX=clang++` before running `make`.

### On Windows
Dependencies: MSVC 2013 or later, CMake 2.8.6 or later, and Boost 1.55. You may download them from:

* http://www.microsoft.com/
* http://www.cmake.org/
* http://www.boost.org/

To build, change to a directory where this file is located, and run theas commands: 
```
mkdir build
cd build
cmake -G "Visual Studio 12 Win64" ..
```

And then do Build.
Githerdone Chris! Good luck!
