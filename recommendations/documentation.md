## Undocumented code can not be used by others, and is therefore near-to useless

#### Background

When writing code, documentation is essential to help you and others
understand the code. Documentation also helps to ensure that the code is
doing what it is supposed to do. Furthermore, it allows the extension
and adaption of the code and is fundamental to ensure reproducibility
and reusability for others and yourself.

#### Recommendations

We recommend always writing documentation, no matter how large the
software project is (even if only one person is involved). Any small
documentation is always better than no documentation. However, software
papers do not count as documentation since they cannot reflect the
ever-changing nature of software.

Multiple types of documentation exist:

1.  Documentation in the code, e.g., code docstrings, describing
    methods, classes, or modules. This helps others understand your
    code.

2.  A README file, which introduces and describes the software. This is
    necessary to explain the purpose and concept of the software.

3.  A documentation page, like *readthedocs*[^1], containing further
    descriptions of the software, helping others to fully understand the
    code and use it.

4.  Documentation of tutorials or concrete examples, e.g., included in
    the documentation page, helps others to easily apply the code.

We recommend to consider your open source strategy (see
open) and try to deduce the applicable
documentation style and technique. If it is unclear how the
documentation will be processed, you can stick to easy documentation
modes. In any case, at least the following should be provided: a README
file, including a summary of the purpose of the software, an
installation guide, and an example script using your software.

Documentation requires considerable effort and should thus be
acknowledged as part of the software development process, e.g., as an
own contribution to the respective research project, and relevant
resources should be allocated. It is important not to neglect it due to
missing resources later on. When planning the documentation, it is
recommended to take into account the different types of documentation
and the respective target audience. You can define minimal requirements
for your documentation (as requirements and dependencies for the
implementation, environment, and decisions made in the development
process). Also, we recommend considering tests as part of the
documentation, as these are necessary for others to understand your
code. To support this understanding, example scenarios can be introduced
in the documentation. However, all example scenarios should be fully
executable. To simplify the documentation process, we recommend
combining the coding with the documentation (for example, via commit
messages, see vcs) by writing readable code, including comments.
Additionally, you can use templates and standards for your
documentation. Many tools are available to make the documentation
process easier and to help make your documentation findable. For Python,
*Sphinx*[^2] can be used to create technical documentation, as can
*Documenter.jl* for Julia[^3].

It also helps to look for best practices. These are for example provided
by Github[^4], but can also be part of recommendations for your
respective programming language, as *pep8* for python[^5].

Due to the interdisciplinary character of energy systems research, it is
recommended that the concept behind the software be explicitly
discussed. People from different domains should understand the purpose
of your software. Thus, also the concepts and ideas of your software,
not only the software itself, should be documented. Additionally, the
code itself should be documented so that other people can work with it
or even extend it.

**You are not done until the documentation is done!**

[^1]: <https://about.readthedocs.com/>, last access 2025-01-17
[^2]: <https://docs.readthedocs.io/en/stable/intro/sphinx.html>, last
    access 2025-01-17
[^3]: <https://github.com/JuliaDocs/Documenter.jl>, last access
    2025-01-17
[^4]: <https://google.github.io/styleguide/docguide/best_practices.html>,
    last access 2025-01-17
[^5]: <https://peps.python.org/pep-0008/>, last access 2025-01-17
