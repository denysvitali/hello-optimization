# Hello Optimization

Some Hello World compared: what's the best language in terms of binary size, and what's the worst?

## Hello World Performance

Tested on an Acer Aspire VN7 Nitro Black Edition, Intel(R) Core(TM) i7-6700HQ CPU @ 2.60GHz, 32 GB of RAM

Programming Language | Source Size (in Bytes) | Binary Size (in Bytes) | Compilation time | Run time
-------------------- | :--------------------: | :--------------------: | :--------------: | :------:
C                    |           58           |          8368          |      0,037       |  0,002
Crystal (Debug)      |           19           |         601952         |      0,537       |  0,005
Crystal (Release)    |           19           |         227168         |      2,248       |  0,005
Java                 |           89           |          390*          |      0,349       |  0,002
Rust (Debug)         |           40           |        1911160         |      0,202       |  0,004
Rust (Release)       |           40           |        1911008         |      0,180       |  0,004

* Java's "binary" is just the bytecode for the JVM

## Environment

Programming Language | Compiler Version
-------------------- | ----------------------------------------------------------------------------------------------------------
C                    | gcc version 6.3.1 20170306
Crystal              | Crystal 0.20.5 (2017-01-25)
Java                 | OpenJDK Runtime Environment (build 1.8.0_121-b13)\ OpenJDK 64-Bit Server VM (build 25.121-b13, mixed mode)
Rust                 | rustc 1.15.1
