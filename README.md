# Sambucks

Sambucks is a secure, decentralized, and anonymous cryptocurrency that is open-source and free for anyone to use.

This project was inspired by the motivational tool Schrute Bucks.

https://www.dailymotion.com/video/x2rlg76_schrute-bucks_fun

Any naming conventions used by this cryptocurrency are purely coincidental and not meant to represent any specific individual.

## Quickstart

1. Spin-up a box running Ubuntu 16.04

2. Type the following command to install dependencies:

    ```sudo apt-get update && apt-get install -y boost1.58 libboost1.58-dev```

3. Download and install the sambucks binaries

## Building Sambucks
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
Good luck!

## Authors

jedec0x0

## License

This project is licensed under the MIT License

## Acknowledgments

* We snapped up CryptoNote's code to make this wonderful piece of art
* Special thanks to the Crown Prince of San Marino
