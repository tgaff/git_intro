• git status
• git init
• git commit
• git add
• git checkout branch
• git remote
• git clone
• git log

# working with remotes
### adding a remote
Allows you to use to push and fetch/pull from a foreign repository.
* git link = copy this from a github or bitbucket repo (on the right side)
* remote-name = This is a _place name_.  Usually `origin` or `upstream`.
```sh
git remote add [remote-name] [git link]
git remote add upstream git@github.com:tgaff/git_intro.git
```

### pushing to a remote
Takes the commits on your branch and puts them on the remote.
* remote-name = This is a _place name_.  Usually `origin` or `upstream`.
* branch-name = at first `master` later we'll have others
```sh
git push [remote-name] [branch-name]
git push origin master # push branch master to origin
```

### cloning a remote repository
Gets a remote repo and stores its commits in a subdirectory of your current directory.
* git link = copy this from a github repo (on the right side)
```sh
git clone [git link]
git clone git@github.com:tgaff/git_intro.git
```

### setup a new repository (empty, without cloning)
Turns the current directory into a new git repo.
```sh
git init
```

### git checkout
Switches the branch (or commit) that you're on.
* branch-name = at first `master` later we'll have others
```sh
git checkout [branch-name]
git checkout master
git checkout fix_spacing_bug
```

### git status
See what changes are and are not staged.  Also see the current branch and any _actions_ that may be in progress.
```sh
git status
```

### git add
Add a file or files to the current _staged_ list.
* file or path = either a file name or shell wildcard
* -A = All
```sh
git add [file or path]
git add README.md
git add views/*
git add .
git add -A
```

### git commit
Commit the currently _staged_ changes.
* message = A summary of the changes you are committing.
```sh
git commit # will open a text editor to type the message
git commit -m "[message]"
git commit -m 'Added birthday to user schema'
```

### git log
Displays the list of commits that are part of the branch.
* branch-name = at first `master` later we'll have others
```sh
git log
git log --stat # displays the files associated with each entry
git log [branch-name] # displays commits on a specific branch
git log master
```
