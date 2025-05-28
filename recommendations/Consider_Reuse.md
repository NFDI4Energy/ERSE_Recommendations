## Building upon research requires reusable software

#### Background

To effectively build upon research, it is often required to build upon
research software, and therefore, a software's reusability is a key
factor to its scientific success. Research based on openly available and
reusable software is cited more often than research where the software
is not reusable. To achieve this, it is necessary to consider your
software's applicability to more general problems (than your own). This
is decided by your software's abstraction level (generalized vs.
specific implementation). However, there is a conflict regarding this
abstraction level most of the time. There are two extreme ends to this
aspect:

1.  Implementing highly specialized features that serve exactly one use
    case, e.g., a specific heat pump model that does not enable any
    parametrization (e.g., to implement different coefficients of
    performance, capacities, or others).

2.  Finding an abstraction for every feature, which provides maximal
    freedom for analyzing other use cases than the one that shall be
    implemented in the first case, e.g., a generalized heat pump model,
    which does not even have a specific mathematical model but enables
    you to provide an arbitrary one by yourself.

Both ends are extreme, and usually, you want to avoid both cases.
However, there is a large spectrum of possibilities between these
extremes.

#### Recommendations

We recommend finding a sensible abstraction level, as it is crucial for
the reusability of the software, and good abstractions enable other
researchers (including yourself and your group) to build upon your
software. At the same time, no unnecessary complexities should be
introduced by choosing an overgeneralized abstraction. This might render
your software less usable due to the lack of specific implementations
and understandability. Consequently, users need to invest more effort,
and reusing becomes difficult.

Another aspect of this is to think about the scope and objective of your
software. These determine to which level your software should be
abstracted. As a rule of thumb, every artifact should focus on precisely
one type of research. This can be on different, relatively macroscopic
levels of energy research. For example, you can develop one type of
energy component model (i.e., for heat pumps) or one software to
simulate decentralized individual behaviors of actors in energy
communities using agent-based modeling.

Besides the level of your implementation, meta aspects, like the name of
the software, can also impact the reusability of your software. Also, we
recommend considering the scientific community you contribute to and how
they organize themselves in open software projects. Integrating your
contribution in the form of software to these software communities
increases your visibility and strengthens the community as a whole.
Example communities for ERS could be based on research frameworks,
e.g., oemof[^1], or generally communities of your favorite programming
language, e.g., the Julia communities[^2]. Furthermore, considering the
target audience, which will eventually reuse your software, is
essential. To improve the compatibility of the software, you can use
ontologies, such as the open energy ontology[^3] to develop and validate
whether the keywords used in your software and documentation fit those
of the broader community.

In short, software reusability is essential for making energy research
sustainable and interoperable, not only for you and your working group
but also for the broader research community you are working in.

**Consider the reuse of your research software!**

[^1]: <https://oemof.org>, last access 2024-12-18
[^2]: <https://julialang.org/community/organizations/>, last access
    2024-12-18
[^3]: <https://openenergyplatform.org/ontology/>, last access 2024-12-18
