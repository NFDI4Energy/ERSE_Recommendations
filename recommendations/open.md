## Research should be publicly available, and your software is part of it

#### Background

Only openly available research software allows other researchers to
reproduce your research results. Since research software is mainly
publicly funded, it is also fair to make it publicly available. This
also enables others to reuse the software, providing additional benefits
like further testing of the software and contributing by creating
extensions and compatible software. Besides making the software open
source, it is also important to register it so other researchers can
find it. These aspects are essential to make a research software
FAIR[^1].

#### Recommendations

We recommend developing your research software open source. By directly
starting the development as open source, challenges can be avoided when
switching to open source later. Further, it allows other researchers to
use your software and actively contribute as early as possible,
improving your software's quality and encouraging cooperation. To
develop the software open source, a suitable license is required. By
choosing a license early each time another software is included, the
compatibility of licenses can be checked directly. Some open source
licenses are incompatible since they put certain conditions on the reuse
of the code, which can conflict between licenses[^2].
When choosing a license, you should check your institution's policy,
which often already proposes a specific license. Also, various guides
help to choose a license[^3].

Cooperation and joint research projects with industry are common in
energy research. Sometimes, industry partners are critical of developing
open source because they want to keep their intellectual property.
Generally, we recommend discussing this topic as early as possible to
find reasonable compromises. Often, certain parts can be developed open
source while others remain closed source. Since open source is open to
all researchers and all industries, it can also improve the exchange
between industry and research.

When you develop open source, there are specific approaches to make your
code more easily reusable by others. First, the repository should follow
programming-language-specific best practices. This can be achieved by
starting with templates for the repository[^4]. Additionally, citing
your software can be made easy by including a CFF file[^5] in your
repository[^6]. Within the repository, it should be
indicated if the software will be maintained, if support is available
and if the developers are open to joining research projects, including
the software. We recommend using the features of the software platform
(GitHub/GitLab) to interact with potential users, e.g., by using issues.

Besides making the source code available, the software should also be
findable. Therefore, we recommend registering the software in a
domain-specific registry like the Open Energy Platform. Getting a DOI
for the software is also helpful, e.g., by archiving versions of the
software on Zenodo[^7][^8].

Energy research is highly interdisciplinary[^9]. Therefore, we recommend adding a very
general description to your software, allowing all researchers to
understand its goals. This way, more researchers can identify whether
the software is useful for them, increasing its reusability. GitHub also
allows you to provide keywords to your repository, which again improves
findability.

Platforms like GitHub and GitLab make it easy to publish your software
under an open source license. Open source research software enables
reproducibility and allows reusability, which can also improve your code
quality. Therefore, we recommend:

**Develop open source & make your software findable!**

[^1]: M. Barker et al., “Introducing the FAIR Principles for research software,” Sci Data, vol. 9, no. 1, Art. no. 1, Oct. 2022, doi: 10.1038/s41597-022-01710-x.
[^2]: X. Cui et al., “An Empirical Study of License Conflict in Free and Open Source Software,” in 2023 IEEE/ACM 45th International Conference on Software Engineering: Software Engineering in Practice (ICSE-SEIP), May 2023, pp. 495–505. doi: 10.1109/ICSE-SEIP58684.2023.00050.
[^3]: e.g., <https://choosealicense.com/>, last access 2024-12-17
[^4]: e.g., cookie-cutter templates at
    <https://cookiecutter.io/templates>, last access 2024-12-17
[^5]: <https://citation-file-format.github.io>, last access 2024-12-17
[^6]: S. Druskat et al., Citation File Format, Aug. 09, 2021. doi: 10.5281/zenodo.5171937.
[^7]: <https://zenodo.org/>, last access 2024-12-17
[^8]: European Organization For Nuclear Research and OpenAIRE, “Zenodo.” CERN, 2013. doi: 10.25495/7GXK-RD71.
[^9]: R. J. W. Tijssen, “A quantitative assessment of interdisciplinary structures in science and technology: Co-classification analysis of energy research,” Research Policy, vol. 21, no. 1, Art. no. 1, Feb. 1992, doi: 10.1016/0048-7333(92)90025-Y.


