---
name: Standard pull request
about: 'Use this template for all code related pull requests.'
assignees: '[TODO: add individual repo maintainers here]'
---

## Pull request description

<!--- 
    Describe the changes and motivation behind them here, if it is not obvious
    from the related issues. Does it have new features, breaking changes, etc. 
-->

### PR meta checklist
- [ ] Pull request is targeting the `main` branch.
- [ ] Pull request is linked to all related issues, if any.
- [ ] I have read the _CONTRIBUTING.md_ document.

### Content checklist
- [ ] My code follows the code style of this project and [ATC Coding Rules](https://github.com/atc-net/atc-coding-rules) guidelines.
- [ ] My change requires a change to the documentation.
  - [ ] I have updated the documentation accordingly.
- [ ] I have updated the appropriate sub section in the _CHANGELOG.md_.
- [ ] My PR includes changes that are:
    - [ ] Fixes (bug fixes) to existing functionality. No new features or breaking changes included.
    - [ ] New minor features. No breaking changes included.
    - [ ] Braking changes. Might also include additions.
- [ ] I have updated the verison in `version.json` to SEMVER rules according changes my PR includes (if necessary).
- [ ] I have added, updated or removed tests to according to my changes.
  - [ ] All tests passed.
