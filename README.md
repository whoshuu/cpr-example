# C++ Requests Example

[![Build Status](https://travis-ci.org/whoshuu/cpr-example.svg?branch=master)](https://travis-ci.org/whoshuu/cpr-example)

[C++ Requests](https://github.com/whoshuu/cpr) is a simple wrapper around [libcurl](http://curl.haxx.se/libcurl) inspired by the excellent [Python Requests](https://github.com/kennethreitz/requests) project.

This is a forkable repository that handles the boilerplate of building and integrating this library into a networked application.

## Building

This project and C++ Requests both use CMake. The first step is to make sure all of the submodules are initialized:

```
git submodule update --init --recursive
```

Then make a build directory and do a typical CMake build from there:

```
mkdir build
cd build
cmake ..
make
```

This should produce a binary in the build directory called `example`. Run it! If you get a response in the form of some json object, then everything worked as expected! The program you just ran is a sweet 3 liner you'll find [here](https://github.com/whoshuu/cpr-example/blob/master/example.cpp).

## Documentation

You can get the latest documentation [here](https://whoshuu.github.io/cpr). It's a work in progress, but it should give you a better idea of how to use the library than the [tests](https://github.com/whoshuu/cpr/tree/master/test) currently do.

## Requirements

The only explicit requirement is a C++11 compatible compiler such as clang or gcc. The minimum required version of gcc is unknown, so if anyone has trouble building this library with a specific version of gcc, do let me know.

## Disclaimer

This library is very much in a pre-alpha stage. Please don't attempt to use this in any serious or critical production environment. If you do use it and find bugs you'd like to report, see below!
