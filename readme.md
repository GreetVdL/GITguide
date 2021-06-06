<!--![laptop image](./images/tutorial.jpg)-->
<p align="center"><img src="./images/tutorial.jpg" width="70%"></p>

# A GIT guide written in Markdown 📓

## Cheat sheets 👀

---> [Markdown cheatsheet](https://www.markdownguide.org/cheat-sheet)

---> [GIT cheatsheet](https://education.github.com/git-cheat-sheet-education.pdf)

---

## GIT guide for local-GitHub connected setup 🚀

1. Make a local folder with your files in it and open the folder in _VSCode_.

`$ code .`

2. Let GIT track the entire folder.

`$ git init`

`$ git add .`

`$ git commit -m "initial commit"`

3. If you make changes, commit them.

`$ git commit -am "commit message"`

- When new files were added, add them first: `$ git add .` `$ git commit -m "commit message"`

4. Create a new GitHub repository.

5. Make the remote connection. You can have multiple remotes so each requires a name. The primary remote is typically named origin.

`$ git remote add origin <URLFROMGITHUB>`

6. Push to your remote to sync them.

`$ git push -u origin main`

- If you have only one remote connected and one branch 'main', you can omit the remote and branch names. `$ git push` The **upstream** flag -u refers to the repository that one will be pulling from by default. Now you can use the git pull and git push commands without arguments.

7. If you make remote changes, pull them in.

`$ git pull <REMOTENAME> <BRANCHNAME>`

- If you have only one remote connected and one branch 'main', you can omit the remote and branch names. `$ git pull`

---

## GIT guide for merging 🌉

1. First, move into the branch you want to merge into.

`$ git checkout <BRANCHNAME>`

2. Tell GIT what branch you want to merge into the branch you are currently in.

`$ git merge <BRANCHNAME>`

3. You can delete the branch that just has been merged.

`$ git branch -d <BRANCHNAME>`

4. You can also delete the branch on your remote on GitHub.

`$ git push <REMOTENAME> --delete <BRANCHNAME>`

---

## Other useful commands 💡

- clone a repo and set the new name of the cloned directory:

`$ git clone <URL> <NEWDIRECTORYNAME>`

- See the status of changes to a repository

`$ git status`

- See what has been changed

`$ git diff`

- Set a new GitHub repo as origin to your clone:

`$ git remote set-url origin <new-repo-url>`<br/>

- Rename the local master branch to main:

`git branch -m master main`

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
