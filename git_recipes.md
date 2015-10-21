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

### git add

### git commit
### git log

### git
