Here’s a list of commonly used Git commands along with their descriptions to help you understand how they work:

### Git Commands with Descriptions

1. **`git init`**
   - **Description**: Initializes a new Git repository in the current directory. This creates a `.git` subdirectory where all the Git-related data will be stored.

2. **`git clone <repository-url>`**
   - **Description**: Creates a local copy of a remote repository. This command downloads the repository and its history.

3. **`git status`**
   - **Description**: Displays the current state of the working directory and staging area, showing which changes are staged, unstaged, or untracked.

4. **`git add <file>`**
   - **Description**: Stages changes in the specified file for the next commit. You can also use `git add .` to stage all changes in the current directory.

5. **`git commit -m "<message>"`**
   - **Description**: Commits the staged changes to the repository with a descriptive message, indicating what changes were made.

6. **`git log`**
   - **Description**: Displays the commit history for the current branch, showing commit IDs, authors, dates, and messages.

7. **`git branch`**
   - **Description**: Lists all branches in the repository. The current branch will be highlighted.

8. **`git checkout <branch-name>`**
   - **Description**: Switches to the specified branch. You can also create a new branch and switch to it using `git checkout -b <branch-name>`.

9. **`git merge <branch-name>`**
   - **Description**: Merges changes from the specified branch into the current branch. This combines the histories of both branches.

10. **`git pull <remote> <branch>`**
    - **Description**: Fetches and merges changes from the specified branch of the remote repository into the current branch.

11. **`git push <remote> <branch>`**
    - **Description**: Uploads local commits to the specified branch of the remote repository.

12. **`git restore <file>`**
    - **Description**: Restores a file in the working directory to its last committed state, effectively discarding any uncommitted changes.

13. **`git rm <file>`**
    - **Description**: Removes a file from the working directory and stages the removal for the next commit.

14. **`git config --global user.name "<Your Name>"`**
    - **Description**: Sets the global username for commits. This information will appear in each commit.

15. **`git config --global user.email "<you@example.com>"`**
    - **Description**: Sets the global email address for commits, which will also appear in each commit.

16. **`git diff`**
    - **Description**: Shows the differences between the working directory and the staging area, or between different commits.

17. **`git reset <commit>`**
    - **Description**: Resets the current branch to a specific commit, potentially changing the state of the working directory and staging area.

18. **`git tag <tag-name>`**
    - **Description**: Creates a tag for a specific commit, usually used for marking release points.

### Example Workflow

1. **Initialize a new repository**:
   ```bash
   git init
   ```

2. **Add a new file**:
   ```bash
   touch example.txt
   git add example.txt
   ```

3. **Commit changes**:
   ```bash
   git commit -m "Add example file"
   ```

4. **Create a new branch**:
   ```bash
   git checkout -b feature-branch
   ```

5. **Make changes and commit**:
   ```bash
   echo "Hello, Git!" >> example.txt
   git add example.txt
   git commit -m "Update example file"
   ```

6. **Merge back to the main branch**:
   ```bash
   git checkout master
   git merge feature-branch
   ```

7. **Push changes to the remote repository**:
   ```bash
   git push origin master
   ```

Feel free to ask if you need more details or examples on any specific command!
