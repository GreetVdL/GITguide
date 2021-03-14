![laptop image](./images/laptop.jpg)

# A GIT guide written in Markdown


## Cheat sheets

---> [Markdown cheatsheet](https://www.markdownguide.org/cheat-sheet)

---> [GIT cheatsheet](https://education.github.com/git-cheat-sheet-education.pdf)

## GIT guide for local-Github connected setup

1. Make a local folder with your files in it and open the folder in VSCode.

`$ code .`

2. Let GIT track the entire folder.

`$ git init`

`$ git add .`

`$ git commit -m "initial commit"`

3. If you make changes, commit them.

`$ git commit -am "commit message"`

  - When new files where added, add them first: `$ git add .` `$ git commit -m "commit message"`

4. Create a new GitHub repository.

5. Make the remote connection. You can have multiple remotes so each requires a name. The primary remote is typically named origin.

`$ git remote add origin <URLFROMGITHUB>`

6. Push to your remote to sync them.

`$ git push -u origin main`

  - If you have only one remote connected and one branch 'main', you can omit the remote and branch names. `$ git push` **Upstream** would refer to the main repo that other people will be pulling from, e.g. your GitHub repo. The -u option automatically sets that upstream for you, linking your repo to a central one. That way, in the future, Git "knows" where you want to push to and where you want to pull from, so you can use git pull or git push without arguments. 

7. If you make remote changes, pull them in.

`$ git pull <REMOTENAME> <BRANCHNAME>`

 - If you have only one remote connected and one branch 'main', you can omit the remote and branch names. `$ git pull`

## Other useful commands

- See the status of changes to a repository

`$ git status`

- See what has been changed

`$ git diff`

- Set a URL to a remote

`$ git remote set-url <REMOTENAME> <URL>`

- View remote addresses

`$ git remote -v`

- See a list of your commits

`$ git log`

- See a list of your local branches

`$ git branch –l`

- See a list of your remote branches

`$ git branch –r`

- See a list of all your branches, locally and remote

`$ git branch –a`

- Make a new branch

`$ git branch <BRANCHNAME>`

- Go into a branch

`$ git checkout <BRANCHNAME>`

- Rename a branch you're currently on

`$ git branch -m <NEWBRANCHNAME>`



