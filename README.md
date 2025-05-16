✅**Activity 1: Research Git**

🔁 Types of Version Control Systems
Local Version Control System (LVCS)

Stores versions on a single computer.

Example: RCS

Centralized Version Control System (CVCS)

All versions are stored on a central server.

Requires internet connection to collaborate.

Example: Subversion (SVN)

Distributed Version Control System (DVCS)

Every user has a full local copy of the repository including its history.

Enables offline work and safer collaboration.

✅ Git is a DVCS.

📸 Snapshots in Git
Git doesn’t track file differences (deltas) like older systems.

Instead, Git takes snapshots of the entire file system when a commit is made.

Unchanged files are referenced rather than stored again.

📁 What is a Repository?
A repository (repo) is a data structure used by Git to store:

Files

Directories

Change history

Branches and tags

🔹 Local Repository:
Exists on your machine.

Created with git init.

🔹 Remote Repository:
Hosted online (e.g., GitHub).

You push and pull between the local and remote repo.

💾 What is a Commit?
A commit saves a snapshot of the staged files in the Git history. It includes:

A unique ID (SHA hash)

Author info

Commit message

Timestamp

🗂️ What is the Working Directory?
The folder on your machine where your project files live.

Files in the working directory may be:

Tracked (under version control)

Untracked (new files)

Modified (changed since the last commit)

🧾 What is the Staging Area?
The staging area (or index) is where you prepare changes before committing.

git add moves changes into the staging area.

git commit takes everything from staging and saves it in the repository.

![image](https://github.com/user-attachments/assets/c3ba86e8-bea5-4970-bf5f-f7101020f844)

Chat GPT Results
