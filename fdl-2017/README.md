# Language and Hardware Acceleration Backend for Graph Processing

Presented at the Forum on specification & Design Languages (FDL), 2017.

## Abstract

Graphs are important in many applications however their analysis on conventional computer
architectures is generally inefficient because it involves highly irregular access to
memory when traversing vertices and edges. As an example, when finding a path from a source
vertex to a target one the performance is typically limited by the memory bottleneck whereas
the actual computation is trivial.

This paper presents a methodology for embedding graphs into silicon, where graph vertices
become finite state machines communicating via the graph edges. With this approach many common
graph analysis tasks can be performed by propagating signals through the physical graph and
measuring signal propagation time using the on-chip clock distribution network. This eliminates
the memory bottleneck and allows thousands of vertices to be processed in parallel.
We present a domain-specific language for graph description and transformation, and demonstrate
how it can be used to translate application graphs into an FPGA board, where they can be
analysed up to 1000x faster than on a conventional computer.

## Implementation

See https://github.com/tuura/fantasi and https://github.com/tuura/centrifuge.
