# GIT

## Installation

Git can easily be installed on Linux with the available package manager. E.g. `apt install git`

For other systems, see the [download](https://git-scm.com/downloads) page.

## Configuration

Git can be configured via the CLI:

```shell
git config --global user.name "name"
git config --global user.email "example@mail.com"
```

## Using Git

| git command                | comment                                                                 |
| -------------------------- | ----------------------------------------------------------------------- |
| `git init`                 | initialize an existing directory as a Git repository                    |
| `git status`               | show modified files in working directory, staged for your next commit   |
| `git clone [url]`          | retrieve an entire repository from a hosted location via URL            |
| `git add [file]`           | add a file as it looks now to your next commit (stage)                  |
| `git diff`                 | diff of what is changed but not staged                                  |
| `git diff --staged`        | diff of what is staged but not yet committed                            |
| `git commit -m “[msg]”`    | commit your staged content as a new commit snapshot                     |
| `git branch`               | list your branches. a * will appear next to the currently active branch |
| `git branch [branch-name]` | create a new branch at the current commit                               |
| `git checkout`             | switch to another branch and check it out into your working directory   |
| `git merge [branch]`       | merge the specified branch’s history into the current one               |
| `git log`                  | show all commits in the current branch’s history                        |

---

#tools 

## Resources

- [GitHub cheat-sheet](https://education.github.com/git-cheat-sheet-education.pdf)
