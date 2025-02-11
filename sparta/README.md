# Sparta

Sparta is a toolkit for modeling/simulation engineers to build CPU,
GPU, and platform simulations.  This is a _framework_ much like `STL`
or Boost in that it doesn't do anything on its own, but rather
provides structure/organization as well as numerous helper classes and
interfaces allowing models built with Sparta to work together for
functional simulation, performance simulation, analysis, and design.

This framework is built on the principles of a OO framework design.
It's written in C++ (mostly C++11 and some 17) as well as python.  The
concepts in modeling communication/scheduling are similar to SystemC
and Gem5, but takes a much more abstract approach to simulation
design.

## Documentation

All great projects have great documentation.  The Sparta team is
striving to have the same, but there's always room for improvement.
There are presentations and online documentation being built, with a
few ready for use.

Specifically, start by generating your own Doxygen build or flip
through the [online generated
documentation](https://sparcians.github.io/map/).

To build your own copy, after cloning the repo, ensure Doxygen and dot
(part of the Graphviz tool suite) are installed.  Then `cd doc; make`.
On the Mac, type `open html/index.html` and peruse the documentation
about the `SkeletalPipeline` and the `Core Example`.

Presentations:

- [Sparta Overview](https://docs.google.com/presentation/d/e/2PACX-1vS1BWtVv0x3qXKQWAeECe2gsF9cMG3Zp2HnXJw52grCAcl21lv3a9pLW6J0lZ32e5DWdZkFyUMcE_AI/pub?start=false&loop=false&delayms=3000)

Examples:

- [Olympia, the RISC-V Performance Core/MSS Model](https://github.com/riscv-software-src/riscv-perf-model)

## Building Sparta

Follow the directions found in [map/README.md](https://github.com/sparcians/map/tree/master#building-map).

## Developing on Sparta

See CONTRIBUTING.md

### Python Shell (not well supported)

To build Sparta with the python shell:

1. `mkdir build-python` (directory name not important)
2. `cd build-python`
3. `cmake -DCMAKE_BUILD_TYPE=[Debug|Release] -DCOMPILE_WITH_PYTHON=ON ..`
4. `make`
