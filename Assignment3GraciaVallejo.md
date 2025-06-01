# Assignment #3 – Jose O. Gracia Vallejo

## Configuration

### Set Git global configuration

```bash
git config --global user.name "jogvallejo"
git config --global user.email "99jose@live.com.mx"
git config --global core.editor "code --wait"
```
View current Git configuration

```bash
git config --global --list
git config --local --list
```

Result (Global):
```bash
user.name=jogvallejo
user.email=99jose@live.com.mx
core.editor=code --wait
```
Result (Local):

```bash
remote.origin.url=https://github.com/jogvallejo/Class-Software-Assurance-JGV.git

Working with a Local Repo
```
Create a new repo

```bash
mkdir test-repo
cd test-repo
git init
```
Clone a repo

```bash
git clone https://github.com/jogvallejo/Class-Software-Assurance-JGV.git
cd Class-Software-Assurance-JGV
```
Check repo status

```bash
git status
```
Result:

```bash
On branch main
nothing to commit, working tree clean
```
Stage and commit changes

```bash
echo "Test file" > test.txt
git add test.txt
git commit -m "Add test.txt for assignment"
```
Delete a versioned file

```bash
git rm test.txt
git commit -m "Remove test.txt from repo"
```
Example .gitignore
Create a .gitignore file:

```bash
echo "*.log" > .gitignore
echo "node_modules/" >> .gitignore
git add .gitignore
git commit -m "Add .gitignore to exclude logs and dependencies"
```
Working with a Remote
View remote

```bash
git remote -v
```
Result:

```bash
origin  https://github.com/jogvallejo/Class-Software-Assurance-JGV.git (fetch)
origin  https://github.com/jogvallejo/Class-Software-Assurance-JGV.git (push)
```
Fetch changes

```bash
git fetch
```
Pull changes

```bash
git pull
```
Result:

```bash
Already up to date.
```
Push local commits

```bash
git push
```
Result:

```bash
Everything up-to-date
```
Branches
View local branches

```bash
git branch
```
Result:

```bash
* main
```
Create and switch branches

```bash
git branch new-feature
git branch
git checkout new-feature
```
Result:

```bash
* new-feature
  main
```
View all branches

```bash
git branch -a
```
Result:


```bash
  main
* new-feature
  remotes/origin/HEAD -> origin/main
  remotes/origin/main
```
Delete local branch

```bash
git checkout main
git branch -d new-feature
git branch
```
Result:

```bash
Switched to branch 'main'
Deleted branch new-feature (was 5221c99).
* main