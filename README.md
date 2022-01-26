# Github CLI Extension for Gitflow

`gh-flow` is an extension that adds Gitflow like commands to the Github CLI, replacing the local merging of branches with Github Pull Requests. It also adds tagging and creating Github releases to the `release` command.

## Usage

```text
gh flow init                             Will create a new develop branch based on the main branch.

gh flow feature start <FEATURE NAME>     Start working on a new feature. Will create a new branch called feature/<FEATURE NAME>.
gh flow feature publish <FEATURE NAME>   Will create a new Pull Request based on the feature branch with the label "feature".
gh flow feature finish <FEATURE NAME>    Will mark the Pull Request with a "ready for review" label.

gh flow [bug|hotfix] start <BUG NAME>    Start working on a new bug. Will create a new branch called bug/<BUG NAME>.
gh flow [bug|hotfix] publish <BUG NAME>  Will create a new Pull Request based on the feature branch with the label "bug".
gh flow [bug|hotfix] finish <BUG NAME>   Will mark the Pull Request with a "ready for review" label.

gh flow support start <SUPPORT NAME>     Start working on a new support case. Will create a new branch called support/<SUPPORT NAME>.
gh flow support publish <SUPPORT NAME>   Will create a new Pull Request based on the support branch with the label "support".
gh flow support finish <SUPPORT NAME>    Will mark the Pull Request with a "ready for review" label.

gh flow release start <RELEASE NAME>     Start working on a new release. Will create a new branch called release/<RELEASE NAME>.
gh flow release publish <RELEASE NAME>   Will create a new Pull Request based on the release branch with the label "release".
gh flow release finish <RELEASE NAME>    Will checkout the main branch that includess the release, tag the release, and create a new release based on the tag.
```
