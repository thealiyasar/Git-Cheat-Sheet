# Create a Repositor

| Command                     | Description                                   |
| --------------------------- | --------------------------------------------- |
| `$ git init [project name]` | From scratch -- Create a new local repository |
| `$ git clone my_url`        | Download from an existing repository          |

---

# Observe a Repository

| Command                         | Description                                            |
| ------------------------------- | ------------------------------------------------------ |
| `$ git status`                  | List new or modified files not yet committed           |
| `$ git dif`                     | Show the changes to files not yet staged               |
| `$ git diff --cached`           | Show the changes to staged files                       |
| `$ git diff HEAD`               | Show all staged and unstaged file changes              |
| `$ git diff commit1 commit2`    | Show the changes between two commit ids                |
| `$ git blame [file]`            | List the change dates and authors for a file           |
| `$ git show [commit]:[file]`    | Show the file changes for a commit id and/or file      |
| `$ git log`                     | Show full change history                               |
| `$ git log -p [file/directory]` | Show change history for file/directory including diffs |

---

# Working With Branches

| Command                                          | Description                                                 |
| ------------------------------------------------ | ----------------------------------------------------------- |
| `$ git branch`                                   | List all local branches                                     |
| `$ git branch -av`                               | List all branches, local and remote                         |
| `$ git checkout my_branch`                       | Switch to a branch, my_branch, and update working directory |
| `$ git branch new_branch`                        | Create a new branch called new_branch                       |
| `$ git branch -d my_branch`                      | Delete the branch called my_branch                          |
| `$ git checkout branch_b & $ git merge branch_a` | Merge branch_a into branch_b                                |
| `$ git tag my_tag`                               | Tag the current commit                                      |

---

# Make a Change

| Command                             | Description                                        |
| ----------------------------------- | -------------------------------------------------- |
| `$ git add [file]`                  | Stages the file, ready for commit                  |
| `$ git add .`                       | Stage all changed files, ready for commit          |
| `$ git commit -m 'commit message'`  | Commit all staged files to versioned history       |
| `$ git commit -am 'commit message'` | Commit all your tracked files to versioned history |
| `$ git reset [file]`                | Unstages file, keeping the file changes            |
| `$ git reset --hard`                | Revert everything to the last commit               |

---

# Synchronize

| Command               | Description                                     |
| --------------------- | ----------------------------------------------- |
| `$ git fetch`         | Get the latest changes from origin (no merge)   |
| `$ git pull`          | Fetch the latest changes from origin and merge  |
| `$ git pull --rebase` | Fetch the latest changes from origin and rebase |
| `$ git push`          | Push local changes to the origin                |
