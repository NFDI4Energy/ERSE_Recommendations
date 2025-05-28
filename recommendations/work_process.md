## Being organized boosts your software project

#### Background

This recommendation discusses how research software development teams
should organize themselves. The most important aspect here is that there
is no one-size-fits-all solution. A one-person PhD software project
should be organized differently than a large team developing software
with thousands of potential users.

#### Recommendations

The main recommendation is to explicitly define the software project's
scope and purpose early in the process. What is the software's general
use case (see
architecture)? How many users are envisioned (see
community)? Is the software intended for research only
or for usage by industry as well? What is its expected lifespan? Will
complete reimplementation be an option, e.g., for going commercial?

Also, you should get a good understanding of the available team to
create the software. How many people are working on the software project
permanently? What are their skills?

Explicit answers to these questions are required to make wise decisions
about organizing the software project and the team. For example,
defining the software's scope helps to decide what to implement and what
not. The team size, on the other hand, is the most important factor for
defining the development process. Do we need code reviews? Do we need
people responsible for specific tasks like testing, documentation?
Especially, large teams must define and enforce the process explicitly
to not end in chaos, like outdated documentation (see
documentation) or failing pipelines (see
testing).

Generally, you can think of software development organization as a scale
from a high degree of agility (e.g., extreme programming[^1]) to a
high degree of planning (e.g., waterfall model[^2]).
Consider which degree is desirable for your project, depending on the
answers to the precious questions. Most research projects have a high
degree of uncertainty, resulting in frequent changes in software
requirements. This would naturally suit a more agile organization.

Another critical question is the developers' software engineering
experience. Especially in energy research, the skill levels vary
significantly, as we pointed out in our introduction. We researchers are not expected to have the
skills of a full-time professional developer. However, we **are**
software developers, which mandates certain minimum skill requirements.
Therefore, we should perform a skill assessment of all team members and
actively provide training to fill the gaps.

Further, it is important to assign clear responsibilities. Primarily the
software project lead should be clear. It should be someone who actively
participates in the software project and does not have too many other
responsibilities. For example, an experienced research assistant is
often a better choice than a professor who does not have the time to
participate actively.

Unorganized software projects result in low-quality software, so we
should explicitly discuss and define our work process. Since there are
no general rules, we need clear leadership and a clear vision of our
software project's scope and purpose.

**Organize yourself and your team!**

[^1]: K. Beck, “Embracing change with extreme programming,” Computer, vol. 32, no. 10, pp. 70–77, Oct. 1999, doi: 10.1109/2.796139.
[^2]: K. Petersen, C. Wohlin, and D. Baca, “The Waterfall Model in Large-Scale Development,” in Product-Focused Software Process Improvement, F. Bomarius, M. Oivo, P. Jaring, and P. Abrahamsson, Eds., Berlin, Heidelberg: Springer, 2009, pp. 386–400. doi: 10.1007/978-3-642-02152-7_29.


