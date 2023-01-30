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

**Git Tags**
```
git checkout HEAD^^
git tag v0 C1
git checkout C2
git tag v1 C2
```

**Git Describe**
```
git commit
```

**Rebasing over 9000 Times**
```
git rebase main bugFix
git rebase bugFix side
git reabase side another
git rebase another main
```

**Multiple Parents**
```
git branch bugWork main^^2^
```

**Branch Spaghetti**
```
git checkout two
git cherry-pick C5 C4 C3 C2
git checkout one
git cherry-pick C4 C3 C2
git branch -f three C2
```

**Clone Intro**
```
git clone
```

**Remote Branches**
```
git commuit
git checkout o/main
git commit
```

**Git Fetich'**
```
git fetch
```

**Git pullin'**
```
git fetch
git merge o/main OR
git pull
```

**Faking teamwork**
```
git clone
git fakeTeamwork 2
git commit
git pull
```

**Git Pushin'**
```
git commit
git commit
git push
```

**Diverged History**
```
git clone
git fakeTeamwork 1
git commit
git pull --rebsae
git push
```

**Locked Main**
```
git reset --hard o/main
git checkout -b feature C2
git push origin feature
```

**Push Main**
```
git checkout main
git pull
git rebase main side1
git rebase side1 side2
git rebase side2 side3
git branch -f main side3
git push origin main
```


