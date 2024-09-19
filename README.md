C++11 implementation of Lox
=========================

I'm reading [Crafting Interpreters book](http://craftinginterpreters.com/) by
Bob Nystrom and writing Lox interpreter in modern C++ since the original code
is in Java and C.


Chapters complete
---

4. Scanning
5. Represening code
6. Parsing Expressions
7. Evaluating Expressions
8. Statements and State
9. Control flow

Building
---

Just run CMake:

```sh
# in build dir
cmake <src-dir>
```

and then

```sh
cmake --build . --target lox
```

To build with tests:

```sh
# in build dir
cmake <src-dir> -DBUILD_TESTING=ON
```

To run tests:

```sh
cmake --build . --target check
```

Alternatively:

```sh
ctest .
```

Usage
---

Run a simple example:

```sh
lox examples/test.lox
```

