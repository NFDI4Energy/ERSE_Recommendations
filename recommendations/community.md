## Your software is useful to others only if they know about it

#### Background

In the previous recommendations, we discussed various points on how to
build high-quality reusable software. Having external users increases
the scientific impact of the software and improves its quality by making
it more thoroughly tested with various scenarios and edge cases.
Finally, every user of your software is a potential future collaborator.
While "Open" already discusses the first points as
publishing the code open source and registering it in a registry, there
are more ways to get attention to your ERS. Therefore, we will provide
recommendations on increasing the number of users and overall reach of
your ERS.

#### Recommendations

The natural step to increase the visibility of your software is to
publish a paper about it. While we discussed in
documentation that software papers are not a
replacement for documentation, they are great for increasing visibility
and motivating your software. Consequently, a software paper should not
contain too much technical details from the documentation. Instead, it
should explain why the software is important, discuss its high-level
capabilities, and convey its scope and vision. We recommend
JOSS[^1] as a modern software journal. If you want to discuss
domain-specific aspects in more detail, it can also be helpful to
publish your software in a conventional domain-specific journal, e.g.,
as it was done for *pandapower*[^2] and *renewables.ninja*[^3].

The second essential step is the active engagement with the community.
Especially in the early stage of the software project, it is a good
approach to contact domain experts and actively collect early feedback.
First, this makes them aware of your software. Second, it prevents the
developed tool from missing the needs of the researchers working in the
field. Later in the process, you can actively present your software
project at a conference, e.g., at the \"Open Source Modelling and
Simulation of Energy Systems (OSMSES)\"[^4] conference.

If your software project uses GitHub/GitLab, their issue system is a
great way to receive feedback of any kind. Feature requests provide
direct information about what the users need, and questions about your
software indicate where the documentation can be improved. In general,
the software repository should be structured in a way that facilitates
engagement with the community. Create a `CONTRIBUTING` file to
communicate to the community how they can contribute to the software
project, including, for example, how to report bugs, style
recommendations, or the code of conduct. Contact information should
always be available if external researchers want to contact the
maintainers.

In summary, when developing reusable software, you should care about
users and actively engage with them to improve software quality and
maximize scientific impact.

**Grow your community!**

[^1]: A. M. Smith et al., “Journal of Open Source Software (JOSS): Design and first-year review,” PeerJ Computer Science, vol. 2018, no. 2, Art. no. 2, 2018, doi: 10.7717/peerj-cs.147.
[^2]: L. Thurner et al., “Pandapower—An Open-Source Python Tool for Convenient Modeling, Analysis, and Optimization of Electric Power Systems,” IEEE Transactions on Power Systems, vol. 33, no. 6, Art. no. 6, Nov. 2018, doi: 10.1109/TPWRS.2018.2829021.
[^3]: S. Pfenninger and I. Staffell, “Long-term patterns of European PV output using 30 years of validated hourly reanalysis and satellite data,” Energy, vol. 114, pp. 1251–1265, Nov. 2016, doi: 10.1016/j.energy.2016.08.060.
[^4]: <https://www.osmses2024.org/home>, last access 2025-01-02
