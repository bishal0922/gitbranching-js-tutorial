# Git Tutorial

[Website Tutorial](https://learngitbranching.js.org/?locale=en_US)

## Solutions

</br>

**Introduction to Git commits**

```git
git commit
git commit
```

**Branching in Git**

```
git checkout -b "yourBranch" OR
git branch "yourBranch"
git checkout "yourBranch"
```

**Merging in Git**

```
git checkout -b bugFix
git commit
git checkout main
git commit
git merge bugFix
```

**Rebase Introduction**
```
git checkout -b bugFix
git commit
git checkout main
git commit
git checkout bugFix
git rebase main
```

**Detach yo' HEAD**

```
git checkout C4 OR
click on the C4
```

**Relative Refs (^)**

```
git checkout bugFix^ OR
git checkout bugFix
git checkout C4
git checkout HEAD^
```

**Relative Refs 2**

```
git branch -f main C6
git branch -f bugFix HEAD~2
git checkout HEAD~1
```

**Reversing Changes in Git**
```
git checkout pushed
git revert pushed (revert because it's a remote branch)
git branch -f local HEAD^^
```

**Cherry Pick Intro**
```
git cherry-pick C3 C4 C7
```

**Interactive Rebase Intro**
```
git rebase -i HEAD~4
then order them C3 C5 C4
```

**Grabbing just one commit**
```
git rebase -i main (only keep c4)
git rebase bugFix main 
```

**Juggling Commits**
```
git rebase -i main
git commit --amend
git rebase -i main
git branch -f main
```

**Juggling Commits #2**

```
git checkout main
git cherry-pick C2
git commit --amend
git cherry pick C3
```




