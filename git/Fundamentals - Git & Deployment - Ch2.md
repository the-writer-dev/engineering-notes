## Ch2. Be fluent at Git #in-progress 
If you read the first chapter of Git tutorial, you are starting the journey! We will look into more about Git operations, which will be useful to your daily engineering flow once you get familiar with them. Let's start without further ado. 

### Branches
To switch branches, run 
```
git checkout <existing branch>
```
To create a new branch, run
```
git branch <new branch>
```
Be careful. This will create a new branch based on the current head. 

To create a branch based on a different branch, run 
```
git branch <new branch> <base branch>
```

To create a new branch and switch to that branch, run 
```
git checkout -b <new branch> <base branch>
```

### Operations in a branch
#### Stage changes 
To add all of the changes you make, run
```
git add .
```

To add a specific change, run
```
git add /path/to/file
```

#### Unstage changes 
To unstage all of the changes you make, run
```
git reset .
```

To unstage a specific change, run 
```
git reset /path/to/file
```

#### Stash changes 
Stash is used to temporarily save changes so you can work on something else and come back later.
To stash your changes, run 
```
git stash
```

To stash with message, run 
```
git stash push -m <message>
```

To retrieve the most stashed changes, run 
```
git stash pop
```

To retreive a specific stash, run
```
git stash pop@{number}
```

#### Clean untracked changes
Clean is used to remove untracked changes. To remove all of untracked changes, run 
```
git clean -f . 
```

#### Diff changes 
Diff is useful to quickly to see the difference between two sources. 
To see the difference between working directory and local repo, run
```
git diff 
```

To see the difference between staging and local repo, run
```
git diff --cached
```

### Commits
Commit captures the staged changes and persist into your repository. Once committed, you can run following commands.

#### Log commits
To see the history of commits, run
```
git log
```

To see the compacted history, run
```
git log --oneline
```

To see the visualized graph, run
```
git log --graph
```

#### Reset commits
Revert winds back the commits we pushed. 
Start by finding which commit you want to come back with `git log`. Then run, 
```
git reset --soft/--hard <git-sha>
```

Option soft will move back to the previous commit you chose and will not remove those changes. On the other hand, hard will remove completely so be careful.

#### Revert commits
Revert creates a new commit undoing changes you made in a specific commit. 
Start by finding which commit you want to come back with `git log`. Then run, 
```
git revert <git-sha>
```

#### Merge commits
Merge incorporates one branch into another one. Typically, it's used to integrate what you developed on a branch into the main branch. 

First, switch the target branch. Run
```
git checkout <target branch>
```

Then, run 
```
git merge <merging branch>
```

There are more Git commands, these have covered the daily development flow I've had for years. 






