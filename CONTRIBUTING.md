# Contributing

## Contributor License Agreement

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

## Code of Conduct

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Issues

All forms of feedback are welcome through issues - please follow the pre-defined templates where applicable.

## Pull Requests

Pull requests (PRs) to this repo are intended for internal team members.

## New (private) preview features

A new preview feature should be self-contained in a subdirectory under [`previews`](previews). It must have an excellent `README.md` file at the root which gives an introduction to the feature and any steps required for trying it.

Markdown files may be used for more articles. It is strongly recommended to follow a similar format and style as required for public preview.

Examples should live in [Azure/azureml-examples], preferablly either PRed or merged into the `main` branch (for continuous testing).

Create a PR to:

- [ ] create a new subdirectory under "previews"
    - [ ] create an excellent README.md for the new directory with:
        - [ ] H1 title of the preview (e.g. "# Pipelines" or "# Interactive jobs") and one sentence (or paragraph) value prop
        - [ ] H2 "## Overview"
        - [ ] H2 "## Installation and set up" - (this should refer to public install + feature flag)
        - [ ] H2 "## Getting started"
        - [ ] H2 "## Contents"
    - [ ] create a "docs" subdirectory
        - [ ] add one or more "how-to" articles corresponding to a user's job to be done which is enabled or made easier by this feature
- [ ] modify the root `README.md` to add a link to the preview subdirectory

Then, merge the PR. If you do not have access, contact a team member internally.

## Update (private) preview features

Create a PR to modify the preview subdirectory as needed. Merge the PR.

