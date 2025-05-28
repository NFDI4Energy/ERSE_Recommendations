## The structure of your software determines its research potential

#### Background

Choosing and developing a suitable architecture is essential to
developing research software efficiently. A typical definition of
software architecture would be: \"The software architecture of a program
or computing system is the structure or structures of the system, which
comprise software components, the externally visible properties of those
components, and the relationships among them.\"[^1].
Here, we mainly think of the composition of software components, the
chosen abstractions of the real world, and the applied design patterns.
Inadequate and/or outdated architectures lead to different problems.
They slow the development of additional features and increase the
complexity of finding bugs. This happens because such architectures do
not adequately induce a structure that helps you to handle the code (and
its bugs) and, therefore, to extend and reiterate it. For example, using
clearly defined interfaces to modules of your code can drastically
improve your ability to provide different implementations for the same
task (e.g., using different MILP solvers). Considering these types of
decisions early saves a lot of code refactoring.

#### Recommendations

We recommend creating the most straightforward possible architecture for
ERS while making it
as complex as necessary to fulfill the specific needs of your research
questions. For this, looking at typical architectures and patterns to
fulfill different needs is necessary. In ERS, we often encounter two types of overall
architectures: (1) single-process input-output simulations or
optimizations and (2) agent-based architectures. However, when looking
at the details, there are a lot of architectural design patterns to
structure these types according to specific needs (i.e., Gangs of Four[^2]). Further, one goal of implementing an architecture is to
keep it maintainable, which includes some enforcement of the
architectural patterns for future development. If it is sensible that
some technical data is not directly accessible, technically enforce it
by restricting access to specific data fields.

To determine how to implement the architecture, it is often helpful to
look at the interfaces of your components to each other (which data
belongs to which component, how much data should be shared, and how the
data should be shared). We recommend using standards wherever possible,
for example, the CIM[^3] for power grids or the
FMI[^4] for dynamic
simulation models. The same is true for reusing established APIs. For
example, most energy-related reinforcement learning frameworks[^5], [^6], [^7]
reuse the well-known `Gymnasium` API to be compatible with open-source
algorithms.

Additionally, it makes sense to think about the interface other
researchers should use when applying your software. Your architecture
should allow the development of user-centric APIs (designed to be used
easily, not implemented easily).

When developing ERS, you often decide on many specific
architectural aspects. Be aware of them, and document them and their
reasoning. For example, if you are developing a grid model and choose to
represent it as a table vs. using a graph, be aware of its advantages
and disadvantages. Also, do not hesitate to change these decisions and
reiterate the architecture if your software outgrows your original
decision and is starting to hold it back.

Lastly, actively consider knowledge transfer for your software's
lifecycle. This includes transferring your knowledge to others (e.g.,
using architectural documentation) and learning about basic
architectural knowledge[^1] and design patterns, such as
Gangs of Four[^2].

To conclude, we recommend thinking and iterating on your architecture as
much as needed while aiming to keep it as simple as possible to ensure
the maintainability of your software.

**Keep the architecture as simple as possible (but as complex as necessary)!**

[^1]: Bass, Len; Paul Clements, Rick Kazman (1998). Software Architecture In. Practice. Boston: Addison-Wesley, ISBN 0-201-19930-0
[^2]: E. Gamma, R. Helm, R. Johnson, and J. M. Vlissides, Design patterns: elements of reusable object-oriented software. in Addison-Wesley professional computing series. Reading, Mass. [u.a.]: Addison-Wesley, 1995.
[^3]: M. Uslar, M. Specht, S. Rohjans, J. Trefke, and J. M. Vasquez Gonzalez, The Common Information Model CIM, vol. 66. in Power Systems, vol. 66. Berlin, Heidelberg: Springer Berlin Heidelberg, 2012. doi: 10.1007/978-3-642-25215-0.
[^4]: <https://fmi-standard.org/>, last access 2025-01-02
[^5]: T. Wolgast, OPF-Gym. (May 10, 2025). Python. Accessed: May 28, 2025. [Online]. Available: https://github.com/Digitalized-Energy-Systems/opfgym
[^6]: S. Hou, S. Gao, W. Xia, E. M. S. Duque, P. Palensky, and P. P. Vergara, “RL-ADN: A High-Performance Deep Reinforcement Learning Environment for Optimal Energy Storage Systems Dispatch in Active Distribution Networks,” Aug. 08, 2024, arXiv: arXiv:2408.03685. doi: 10.48550/arXiv.2408.03685.
[^7]: C. Yeh et al., “SustainGym: Reinforcement Learning Environments for Sustainable Energy Systems”.



