# Continuous Integration

`C`ontinuous `I`ntegration (CI) is the process of automating the build and testing of code every time a team member commits changes to version control. CI encourages developers to share their code and unit tests by merging their changes into a shared version control repository after every small task completion. Committing code triggers an automated build system to grab the latest code from the shared repository and to build, test, and validate the full main branch.

## Automated Build

We do continuous build and testing of code, every time a change is committed.

- ✔️ **Do** have Build definitions as Code (yaml/yml)
    > *The definition is versioned with your code and follows the same branching structure as your code.*
- ✔️ **Do** have a PR (`P`ull `R`equest) build for PR into main branch
    > *The build should be fast and run all unit tests but do not produce any binaries as output.*
- ✔️ **Do** publish source symbols
    > *Indexing source code enables you to use your .pdb symbol files to debug an app on a machine other than the one you used to build the app.*
- 💭 **Consider** enabling continuous code quality integration like e.g. SonarCloud
    > *SonarCloud provides the capability to not only show health of an application but also to highlight issues newly introduced. With a Quality Gate in place, you can fix the leak and therefore improve code quality systematically.*
- 💭 **Consider** using WhiteSource Bolt to discover and remediate OSS risk
    > *White Source provides a convenient solution for companies that need to manage their open source assets to ensure license compliance and reduce risk.*
- ❌ **Do not** publish any packages or deploy binaries to any environment
    > *Use a release pipeline instead for a reliable and controlled delivery process.*

## Automated Build Tests

Automated testing enables developers to make changes, refactor, and add features to existing code bases with confidence, knowing that they’re not about to completely break existing code.

- ✔️ **Do** enable Code Coverage
    > *Having a code base with deep test coverage is one of the base requirements for achieving continuous delivery and it all starts with the build process.*
- 💭 **Consider** parallelizing test execution for large codebases
    > *To minimize test execution time, test execution can be parallelized as each test must be self-contained.*
- ❌ **Do not** run tests that require access to external resources like SQL
    > *Tests must be fast, self-contained and predictable, testing external resources should be the responsibility of integration tests and is part of the release pipeline.*
