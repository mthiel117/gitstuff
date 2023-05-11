# Common Git Commands

## Setup

### Identity and default branch name

``` bash
git config --global user.name "Bob Smith"
git config --global user.email "bsmith@example.com"
git config --global init.defaultBranch main
```

## Restore to previous state

Find Commit Hash

``` bash
git log --oneline
```

Restore a file to previous commit

``` bash
git restore --source <commit hash> <filename>

# Example
git restore --source 0b293b4 file1.txt
```

## Clone repo to local host

``` bash
# Example to clone this repo
git clone https://github.com/mthiel117/gitstuff.git
```

## Diff between branches

``` bash
git diff <branch1>..<branch2>

# example
git diff main..update-hostnames
```
