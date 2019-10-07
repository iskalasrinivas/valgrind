# valgrind
[![Build Status](https://travis-ci.org/iskalasrinivas/valgrind.svg?branch=valgrind_exercise)](https://travis-ci.org/iskalasrinivas/valgrind)
---

## Overview

C++ project for finding and fixing bugs using valgrind tool.

## Standard install via command-line
```
git clone --recursive https://github.com/iskalasrinivas/valgrind
cd <path to repository>
mkdir build
cd build
cmake ..
make
Run tests: ./test/cpp-test
Run program: ./app/shell-app
```
## valgrind commands used

valgrind --leak-check=full  ./app/shell-app  "to check for the bugs in the program"

valgrind --log-file=filename --leak-check=full  ./app/shell-app "to save output in text file."


## install kcachegrind

sudo apt-get install kcachegrind

## running memory profiler

valgrind --tool=callgrind ./app/shell-app this command creates a .out file in the same directory.
run this file to see the memroy profile
