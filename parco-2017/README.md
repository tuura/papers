# Distributed Event-based Computing

Presented at the ParCo 2017 conference.

## Abstract

As computing systems get larger in capability - a good thing - they also
get larger in ways less desirable: cost, volume, power requirements and so on.
Further, as the datastructures necessary to support large computations grow
physically, the proportion of wallclock time spent communicating increases
dramatically at the expense of the time spent calculating. This state of affairs is
currently unacceptable and will only get worse as exa-scale machines move from
the esoteric to the commonplace. As the unit cost of non-trivial cores continues to
fall, one powerful approach is to build systems that have immense numbers of
relatively small cores embedded (both geometrically and topologically) in a vast
distributed network of stored state data: take the compute to the data, rather than
the other way round. In this paper, we describe POETS - Partially Ordered Event
Triggered Systems. This is a novel kind of computing architecture, built upon the
neuromorphic concept that has inspired such machines as SpiNNaker and
BrainScaleS. The central idea is that a problem is broken down into a large set
of interacting devices, which communicate asynchronously via small, hardware
brokered packets (the arrival of which is an event). The set of devices is the task
graph. You cannot take a conventional codebase and port it to a POETS
architecture; it is necessary to strip the application back to the underlying
mathematics and reconstruct the algorithm in a manner sympathetic to the solution
capabilities of the machine. However, for the class of problems for which this
approach is suitable, POETS has already demonstrated solution speedups of a
factor of 200 over conventional techniques.
