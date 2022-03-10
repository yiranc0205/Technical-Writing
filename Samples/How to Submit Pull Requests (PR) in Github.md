# Task Overview
This documentation guides you how to submit *pull requests (PR)* in Github.

# Prerequisites
1. Fork project repository to origin repository on Github website.

2. Clone origin repository to your PC.
```bash
$ git clone <origin code>
```

3. Add upstream repository to local repository.
```bash
$ git remote add upstream <upstearm code>
```

4. Verify the new upstream repository.
```shell
$ git remote -v
```

5. Fetch the latest upstream to local repository.
```bash
$ git fetch
```

# Steps
## Work in Local Repository
1. Create a branch based on *master*.
```bash
$ git checkout master
$ git checkout -b <branch name>
```
	
2.  Set upstream of working branch to *upstream/master*.
```bash
$ git branch --set-upstream-to=upstream/master <branch name>
```

3. Do your work on working branch.

4. Add your work to index.
```bash
$ git add .
```
or
```bash
$ git add <file name>
```

5. Commit your work to working branch.
```bash
$ git commit -m '<commit massage>'
```

6. Pull the latest updates of *upstream/master* to working branch.
```bash
$ git pull
```
or (when needed)
```bash
$ git pull --rebase
```

7. Solve conflicts (optional). 

8. Push working branch to *origin*.
```bash
$ git push origin HEAD
```

## PR in Github
1. Enter upstream project repository on Github website.
2. Click *pull requests* - *New pull request* - *compare across forks*.
3. Select **head** repository and branch. Usually, base repository and branch is default.
4. Click *Create pull request*.
5. Write a description of your work.
6. Confirm your PR and click *Create pull request*.
7. Wait for the review.
8. Revise your work according to the review (optional). You can use the following commands to keep a clean commit history.
```bash
$ git reset --soft <commit id>
```
or
```bash
$ git commit --amend
```


## After your PR is merged
1. Pull the latest updates of *upstream/master* to *master*.
```bash
$ git checkout master
$ git pull
```

2. Delete working branch.
```bash
$ git branch -b <branch name>
```

# Result
Now you have successfully submitted a PR!