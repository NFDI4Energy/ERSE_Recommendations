## Inventing is great, reinventing is a waste of time

#### Background

The core of science is to build on top of other's ideas and
contributions. Especially in recent years, more and more research
software projects are released as open-source and can be extended and
reused by the community. Still, we often feel the necessity to start
from scratch and build our own library or framework. For example, a
recent review identified 63 different open-source, optimization-based
frameworks for energy system modeling[^1]. They all
share the same underlying principle of network-based energy flow
optimization with similar architectures. Many frameworks are only used
by their home institutions, which indicates possible redundancy[^1]. However, writing code is only one of our many
diverse responsibilities. Overall, researchers have too little time to
reimplement work already done by others. Instead, we should aim to reuse
and extend existing high-quality software and focus on implementing
novel research contributions. While familiarizing oneself with the
documentation of other tools seems more time-consuming in the beginning,
this time will be saved later on because existing code often already
comes with a lot of testing, verification, and documentation which you
would otherwise need to create for your new code. This recommendation
discusses creating high-quality research software without implementing
everything from scratch.

#### Recommendations

The first step of reusing software is to find existing software that
solves your problem or parts of it. The natural approach is to do a
literature survey beforehand. While this is an important step, not all
software is published as a conference or journal publication. Instead,
software registries and similar platforms can be used to find research
software. For energy research, the Open Energy Platform[^2] and DOE
CODE[^3] are available. Additionally, the Helmholtz Research Software
Directory[^4] and the JOSS[^5] list research software without a
domain focus. Software repositories like GitHub[^6] can also be
searched. In these cases, energy-specific keywords should be used. The
final recommendation for finding reusable software is to ask experienced
colleagues and other researchers who work on similar problems. They can
often tell you about hitherto unknown tools, e.g., those under
development in other research projects, and which libraries are useful.

To use external software for your research project, you should check
their license and see if it is compatible with your code and its
envisioned use case (see also
open). If the software does not entirely cover
your use case, you can contact the software maintainers. They may be
already discussing and planning the feature you need. If they do not
want to implement it they may wish to include your software when it is
finished. By explicitly communicating with other researchers, redundant
software can be prevented, and as a side effect, overall collaboration
in science is strengthened. This *collaboration first* thinking should
follow through the whole software project. For example, write issues and
pull requests when finding bugs in other software you use. Not only does
this help other people, but it also improves your software as a side
effect.

However, there are exceptions to the rule of reusing existing software.
When the existing solutions are of low quality or outdated, starting a
new software from scratch can be a good idea. Also, developing an
open-source alternative can have a significant scientific impact if the
existing software is proprietary. In general, parallel development is
perfectly fine to some extent. It results in competition and provides
other researchers with options that have respective pros and cons.

Reusing existing research software results in higher-quality software
for less effort. It accelerates scientific progress and supports overall
collaboration. Hence, the following recommendation:

**Reuse and extend other software if possible and useful!**

[^1]: M. Hoffmann et al., “A review of mixed-integer linear formulations for framework-based energy system models,” Advances in Applied Energy, vol. 16, p. 100190, Dec. 2024, doi: 10.1016/j.adapen.2024.100190.
[^2]: <https://openenergyplatform.org/>, last
    access 2024-12-04
[^3]: <https://www.osti.gov/doecode/>m last access 2025-01-20
[^4]: <https://helmholtz.software/software?&keywords=%5B%22Energy%22%5D&page=0&rows=12>,
    last access 2024-12-04
[^5]: <https://joss.theoj.org>, last access
    2024-12-16
[^6]: <https://github.com/search?q=%22power%20system%22&type=repositories>,
    last access 2024-12-04
