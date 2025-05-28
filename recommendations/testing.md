## Testing your software means increasing trust in your research!

#### Background

Appropriate testing ensures your software works correctly. With testing,
bugs can be found, and the software's functionality can be guaranteed.
Especially when software is constantly changed, testing can help to
ensure that changes do not break functionalities.

You are likely already intuitively testing your software, for example,
by using sanity checks on the software output, e.g., expecting values in
a particular order of magnitude (MWh instead of kWh) or making sure that
the efficiency is \<1 or checking the consistency of results with
conservation equations, such as conservation of mass, energy, or
momentum. Other examples include adding `assert` statements to, e.g.,
make sure that input data has a specific structure, testing a function
with dummy data before integrating it into a larger script, and
exploring edge cases, e.g., "how will my model handle a mass flow rate
of zero?".

You are likely performing these tests manually on an "as needed" basis.
While this is efficient practice during the development phase, manual
testing typically leads to a more extensive testing effort in the long
run[^1], and ad hoc, intuitive testing by the
developer can have blind spots[^2]. In addition,
automated testing provides benefits such as the ability to make changes
quickly and securely and perform major refactorings without the entire
software immediately losing several levels of quality.

#### Recommendations

We recommend you elevate your intuitive, manual testing to a systematic,
automated testing procedure, for example, as described
in[^2].

We recommend considering a test strategy and testing your software based
on it. A test strategy describes the testing approach, including what
aspects, methods, and techniques of the software are to be
tested[^3]. It should be identified early and
specify how the software's testing process is designed[^3]. Using a strategy helps ensure that the code
has been extensively and thoroughly tested, including all relevant
functions.

In your strategy, we recommend determining what exactly needs to be
tested (properties and behavior) and defining minimal requirements for
that (e.g., test coverage, which defines the degree to which the code is
checked through tests[^3]). Requirements defined at
the beginning of the software project should be mapped to the tests and
thus checked for functionality. Similar to documentation (see
documentation), tests should be considered as a
contribution to the software project and should be planned accordingly.
It is important not to neglect testing due to missing resources later
on.

While testing, the reusability and reproducibility of the code should be
considered. Thus, we recommend providing data for testing and
information such as API versions, dependencies, and comparability to
other software if applicable. Templates and standards, e.g., use testing
packages for your respective type of test and programming language, as
*pytest*[^4] for Python, can help you when writing your tests.

We recommend taking into account different types of tests: unit,
integration, and end-to-end tests. Unit tests are designed to test the
functionality of specific components or modules, their restrictions and
constraints, while integration tests focus on the interfaces and
interaction of components[^3]. For example, a unit
test could test the performance of a photovoltaic system under different
solar irradiance conditions and, thus, the functionality of the power
calculation function. Integration tests would, e.g., focus on
interactions between a controller of the plant and the plant itself,
such as sending and responding to control signals. End-to-end tests
consider the software as a whole, which helps to ensure that the overall
software behaves as expected, considering the data flow over all tasks.
An example of end-to-end testing is testing the entire system, including
all controllers and components, from an end-user perspective. Ideally,
all testing is completely automated using the
CICD capabilities
of GitHub/GitLab. This way, you can ensure that every single version of
your software is tested.

In the energy domain, software is sometimes used by people who did not
develop it (people without IT knowledge). Therefore, we recommend having
the software tested by potential users who were not involved in its
development. By involving potential users early in the development
process and having them test the installation, it is possible to ensure
that the software can be used by the people it is intended for. Testing
is essential if the software will be used in the field. Since we are
considering software for a safety-critical system, well-designed testing
is significant in energy research.

**Test your software based on a test strategy!**

[^1]: M. Patrick, J. Elderfield, R. O. J. H. Stutt, A. Rice, and C. A. Gilligan, “Software testing in a scientific research group,” in Proceedings of the 31st Annual ACM Symposium on Applied Computing, Pisa Italy: ACM, Apr. 2016, pp. 1454–1459. doi: 10.1145/2851613.2851783.
[^2]: R. Mischke, K. Schaffert, D. Schneider, and A. Weinert, “Automated and manual testing as part of the research software development process of RCE,” Apr. 12, 2022, arXiv: arXiv:2204.05600. doi: 10.48550/arXiv.2204.05600.
[^3]: G. A. Center, “DLR Software Engineering Initiative,” DLR Software Engineering Initiative. Accessed: Mar. 25, 2024. [Online]. Available: https://rse.dlr.de/
[^4]: <https://docs.pytest.org/en/stable/>, last access 2025-01-17
