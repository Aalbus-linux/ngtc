# NGTC
Non-GNU toolchain

## Building

Requirements: x86_64 Linux distro with at least 6Gb of RAM and a lot of time.

Instructions: run `./build-all.sh`, this will set up the build environment, download toolchain source code and compile it.

## What is included

- `musl` libc
- `clang` compiler
- `lld` linker

## What is not included

- Any code from glibc
- Any code from gcc or libgcc
- Any code from GNU binutils

## What works

- C code compilation (requires `CFLAGS="-fPIC"`)
- C++ code compilation (requires `CXXFLAGS="-fPIC" LDFLAGS="-lunwind"`)

## Status

### Platform support

|  | x86  | ARM |
| --- | --- | --- |
| **32 bit**  |  |  |
| **64 bit**  | + |  |

### Language support

- C
- C++
- (not yet) Rust
- (not yet) Go
- (not yet) D
