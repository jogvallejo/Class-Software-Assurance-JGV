# Assignment #3 – Jose O. Gracia Vallejo

## Configuration

### Set Git global configuration

```bash
git config --global user.name "jogvallejo"
git config --global user.email "99jose@live.com.mx"
git config --global core.editor "code --wait"
View current Git configuration
bash
Copy
Edit
git config --global --list
git config --local --list
Result (Global):

bash
Copy
Edit
user.name=jogvallejo
user.email=99jose@live.com.mx
core.editor=code --wait
Result (Local):

bash
Copy
Edit
remote.origin.url=https://github.com/jogvallejo/Class-Software-Assurance-JGV.git
...
✅ Global config is applied across all repos on your machine. Use it when working consistently as the same user.
Local config overrides global settings for just one repo.

Working with a Local Repo
Create a new repo
bash
Copy
Edit
mkdir test-repo
cd test-repo
git init
Clone a repo
bash
Copy
Edit
git clone https://github.com/jogvallejo/Class-Software-Assurance-JGV.git
cd Class-Software-Assurance-JGV
✅ Cloning copies an existing remote repo to your local machine.
git init starts a brand-new, empty repo.

Check repo status
bash
Copy
Edit
git status
Result:

bash
Copy
Edit
On branch main
nothing to commit, working tree clean
Stage and commit changes
bash
Copy
Edit
echo "Test file" > test.txt
git add test.txt
git commit -m "Add test.txt for assignment"
Delete a versioned file
bash
Copy
Edit
git rm test.txt
git commit -m "Remove test.txt from repo"
Example .gitignore
Create a .gitignore file:

bash
Copy
Edit
echo "*.log" > .gitignore
echo "node_modules/" >> .gitignore
git add .gitignore
git commit -m "Add .gitignore to exclude logs and dependencies"
Exclude temporary files, OS files, compiled code, or dependencies.

Working with a Remote
View remote
bash
Copy
Edit
git remote -v
Result:

bash
Copy
Edit
origin  https://github.com/jogvallejo/Class-Software-Assurance-JGV.git (fetch)
origin  https://github.com/jogvallejo/Class-Software-Assurance-JGV.git (push)
Fetch changes
bash
Copy
Edit
git fetch
Pull changes
bash
Copy
Edit
git pull
Result:

bash
Copy
Edit
Already up to date.
Push local commits
bash
Copy
Edit
git push
Result:

bash
Copy
Edit
Everything up-to-date
Branches
View local branches
bash
Copy
Edit
git branch
Result:

bash
Copy
Edit
* main
Create and switch branches
bash
Copy
Edit
git branch new-feature
git branch
git checkout new-feature
Result:

bash
Copy
Edit
* new-feature
  main
View all branches
bash
Copy
Edit
git branch -a
Result:

bash
Copy
Edit
  main
* new-feature
  remotes/origin/HEAD -> origin/main
  remotes/origin/main
Delete local branch
bash
Copy
Edit
git checkout main
git branch -d new-feature
git branch
Result:

bash
Copy
Edit
Switched to branch 'main'
Deleted branch new-feature (was 5221c99).
* main