## Track the history and learn for the future

#### Background

Software is constantly changing. New features are implemented, bugs are
fixed, and code is improved. Sometimes, these developments also happen
in parallel. For example, you are implementing a physical model to
analyze the operating behavior of a battery, and you supervise a student
tasked to implement a thermal model for the battery and, therefore, give
them a copy of your code. When the student finishes their implementation
after a couple of months, your own code has evolved, and manually
integrating the master student's code back into your own becomes a messy
task of copy, paste, break, fix, test, and retest. This, and many other
problems associated with changing code, multiple versions, and coding as
a team, can be avoided with version control. While using version control
is standard practice in software development, it is not always the case
in research software. Tracking different versions of your code enables
you and others to keep an overview of which feature was developed and to
understand the history of the code, thereby increasing its
maintainability. It also allows for the undoing of specific changes when
a problem occurs. Additionally, version control enables reproducibility
of the research conducted with the code by providing specific links to
use exactly the same version[^1].

#### Recommendations

Version control systems can help you track different software versions.
The most popular version control system is Git[^2]. The platforms
GitHub[^3] and GitLab[^4] are based on Git and extend it by a user
interface providing a good overview and additional features. If your
institution does not allow you to use GitHub or the public GitLab, you
can often also use a GitLab instance offered by your institution.

Within Git, changes to the software are included as a *commit*. By
adding meaningful messages to each commit, the changes are documented.
At least one commit at the end of each day is recommended.

Version control systems also allow different *branches*, which are
parallel versions of the same software. It is helpful to always have a
working software version in one branch (usually called *master* or
*main*). Also, this way, different developers can work in parallel
without directly causing conflicts. A branch can be merged into another
by a *pull* or *merge request*. These requests are another good option
for additional comments and documentation to make the changes more
understandable. In software projects with multiple developers, this is
also the step where code reviews should be conducted for quality
assurance.

The version control platforms also have additional features that make it
easier to organize the software development. *Issues* can be used to
track bugs, code contributions, and new potential feature ideas. They
also allow others to get an overview of what is planned next.
Additionally, they provide options for CICD, which is the practice of automating the
integration, testing, and deployment of code changes to ensure reliable
and efficient software delivery. In the context of research software,
CICD is especially
used for automated testing of each commit (see also
testing).

Version control systems are necessary to keep track of software versions
while also allowing to organize the software development to a certain
extent. If you are not familiar with version control, we recommend
taking some basic training on it, e.g., by the software carpentry[^5].

**Use version control!**

[^1]: G. K. Sandve, A. Nekrutenko, J. Taylor, and E. Hovig, “Ten Simple Rules for Reproducible Computational Research,” PLOS Computational Biology, vol. 9, no. 10, Art. no. 10, Oct. 2013, doi: 10.1371/journal.pcbi.1003285.
[^2]: <https://git-scm.com/>, last access 2024-12-17
[^3]: <https://github.com/>, last access 2024-12-17
[^4]: <https://about.gitlab.com/>, last access 2024-12-18
[^5]: <https://swcarpentry.github.io/git-novice/index.html>, last access
    2024-12-17
