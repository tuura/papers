# I. Process Windows

Presented at the International Conference on Application of Concurrency to System Design, 2017.

## Abstract

We describe a method for formally representing the behaviour of complex
processes by _process windows_. Each window covers a part of the
system behaviour, i.e. a part of the underlying transition system, and
is easier to understand and analyse than the complete transition system.
Process windows can overlap and have shared states and transitions so that
the complete system behaviour is the _union_ of window behaviours.
We demonstrate the advantage of such representations when dealing
with complex system behaviours, and discuss potential applications
in circuit design and process mining.

As a motivational example we consider the problem of covering
transition systems by _marked graphs_, or more generally choice-free
Petri nets. The obtained windows correspond to choice-free behavioural
_scenarios_ of the system, wherein one window can take over,
or _wake up_, after another window has become inactive. The
corresponding _wake-up conditions_ and _wake-up markings_
can be derived automatically.

# II. Reduction of Order Structures

Presented at the International Conference on Application of Concurrency to System Design, 2017.

## Abstract

Relational order structures are used to describe and investigate properties of concurrent systems.
To reduce the complexity of order structures, one typically considers only their essential components,
which, in the case of partial orders, leads to the notion of Hasse diagrams. We lift this notion to
the level of generalised mutex order structures, which are used to model not only causal dependencies
but also weak causality and mutual exclusion. We provide a new and more concise axiomatic definition of
these structures, investigate their important properties, and present efficient algorithms for computing
their _reduction_ and _closure_. The algorithms are implemented in a publicly available software tool
with graphical user interface.
