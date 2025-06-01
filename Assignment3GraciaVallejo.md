## Configuration

<pre> ### Set username and email (Global) ```bash git config --global user.name "jogvallejo" git config --global user.email "99jose@live.com.mx" ``` > 

✅ These are set globally so Git can identify the user for all repositories on the system. This is recommended unless you're using different identities for different projects. 

### Set core editor for Git

```bash git config --global core.editor "code --wait" ``` > 
✅ This sets Visual Studio Code as your default editor for Git messages (like when merging or rebasing interactively). 
### View global Git configuration ```bash git config --global --list ```
 **Result:** ```bash credential.helperselector.selected=manager user.email=99jose@live.com.mx user.name=jogvallejo core.editor=code --wait ``` 
 ### View local Git configuration (within repo) ```bash git config --local --list ``` **Result:** ```bash core.repositoryformatversion=0 core.filemode=false core.bare=false core.logallrefupdates=true core.symlinks=false core.ignorecase=true remote.origin.url=https://github.com/jogvallejo/Class-Software-Assurance-JGV.git remote.origin.fetch=+refs/heads/*:refs/remotes/origin/* branch.main.remote=origin branch.main.merge=refs/heads/main ``` </pre>
 To https://github.com/jogvallejo/Class-Software-Assurance-JGV.git
   0accfe8..5221c99  main -> main

   andre@LAPTOP-PJVB052T MINGW64 ~/Documents/github/Class-Software-Assurance-JGV/Class-Software-Assurance-JGV (main)
$ git branch            # View local branches
git branch new-feature
git branch            # View again after creation
git checkout new-feature
git branch -a         # View all local + remote branches
git checkout main
git branch -d new-feature
git branch            # Confirm deletion
* main
* main
  new-feature
Switched to branch 'new-feature'
  main
* new-feature
  remotes/origin/HEAD -> origin/main
  remotes/origin/main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
Deleted branch new-feature (was 5221c99).
* main

andre@LAPTOP-PJVB052T MINGW64 ~/Documents/github/Class-Software-Assurance-JGV/Class-Software-Assurance-JGV (main)
$ git branch
* main

andre@LAPTOP-PJVB052T MINGW64 ~/Documents/github/Class-Software-Assurance-JGV/Class-Software-Assurance-JGV (main)
$ git branch new-feature
git branch
* main
  new-feature

andre@LAPTOP-PJVB052T MINGW64 ~/Documents/github/Class-Software-Assurance-JGV/Class-Software-Assurance-JGV (main)
$ git checkout new-feature
Switched to branch 'new-feature'

andre@LAPTOP-PJVB052T MINGW64 ~/Documents/github/Class-Software-Assurance-JGV/Class-Software-Assurance-JGV (new-feature)
$ git branch -a
  main
* new-feature
  remotes/origin/HEAD -> origin/main
  remotes/origin/main

andre@LAPTOP-PJVB052T MINGW64 ~/Documents/github/Class-Software-Assurance-JGV/Class-Software-Assurance-JGV (new-feature)
$ git checkout main
git branch -d new-feature
git branch
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
Deleted branch new-feature (was 5221c99).
* main