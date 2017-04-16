# Contributing
Thanks for your interest in this resource! By participating in this project, you agree to abide by FreeCodeCamp-Sacramento's [code of conduct](https://github.com/FreeCodeCamp-Sacramento/freecodecamp-sacramento.github.io#code-of-conduct).

## How to Contribute

#### Set up
1. Install [Git](https://git-scm.com/) or your favorite Git client
2. (Optional) [Set up ssh keys](https://help.github.com/articles/connecting-to-github-with-ssh/) for Github

#### Forking the Project
1. (Optional) Create a parent directory to hold all of your projects.
2. Go to the top level git-resources repository: [https://github.com/FreeCodeCamp-Sacramento/git-resources](https://github.com/FreeCodeCamp-Sacramento/git-resources)
3. Click the "Fork" Button in the upper right hand corner of the interface [more info here](https://help.github.com/articles/fork-a-repo/)
4. After the repository has been forked, you will be taken your copy of the repository at `your-username/git-resources`

#### Cloning the Project
1. Open up your favorite Terminal Emulator/Command Line
2. Clone your fork of `git-resources`
```
git clone git@github.com:your-username/git-resources.git
```
**make sure you replace `your-username` with your Github username**

This will download this repository into your projects directory.

#### Set up your upstream
1. Change directory to the new `git-resources` directory (cd git-resources)
2. Add a remote to the original repository:
```
$ git remote add upstream https://github.com/FreeCodeCamp-Sacramento/git-resources.git
```

Congratulations! You now have a copy of this repository

#### Maintaining your fork
Now that you have a copy of your fork, this is what you have to do to keep it current

##### Rebase from upstream
Do this prior to every time you create a branch for a pull request (PR):

1. Make sure you are on the `master` branch
  > ```
  > $ git status
  > On branch master
  > Your branch is up-to-date with 'origin/master'.
  > ```

  >If your aren't on `master`, resolve outstanding files / commits and checkout the `master` branch

  > ```
  > $ git checkout master
  > ```

2. Do a pull with rebase against upstream
  > ```
  > $ git pull --rebase upstream master
  > ```

  > This will pull down all of the changes to the official master branch, without making an additional commit in your local repo.

3. (*Optional*) Force push your updated master branch to your GitHub fork

  > ```
  > $ git push origin master --force
  > ```

  > This will overwrite the master branch of your fork.

#### Create A Branch
Before you start working, you will need to create a separate branch specific to the issue / feature you're working on. You will push your work to this branch.

##### Naming Your Branch
Name the branch something like `fix/xxx` or `add-resource/xxx` where `xxx` is a short description of the changes or addition you are attempting to add. For example: `add-resource/article-merge-vs-rebase` could be a branch where you add an article to the resources.

##### Adding Your Branch
To create a branch on your local machine (and switch to this branch):
```
$ git checkout -b [name_of_your_new_branch]
```

and to push to GitHub:
```
$ git push origin [name_of_your_new_branch]
```

**If you need more help with branching, take a look at *[this](https://github.com/Kunena/Kunena-Forum/wiki/Create-a-new-branch-with-git-and-manage-branches)*.**

## Other Resources
- [FreeCodeCamp's Contribution Guide](https://github.com/freeCodeCamp/freeCodeCamp/blob/staging/CONTRIBUTING.md#contribution-guidelines) which formed the basis of this guide.
