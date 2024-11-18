# Git Reset

In Git, the `git reset` command is used to undo changes or to move the head reference (HEAD) and branch pointers to a specific commit. It can be a useful operation, but it can also be dangerous if used incorrectly, as it can change the commit history in your repository. Here I explain the three most common ways to use `git reset`:

1. **`git reset --soft`:**
    - This command will undo the changes made in the last commit and move the current branch to the last commit. However, it will leave the changes made in the staging (registration) area.
    - Useful if you need to recommit to the same changes after reviewing them or making additional modifications.
    - Example:

      ```shell
      git reset --soft HEAD~1
      ```

2. **`git reset --mixed` - Default Value:**
    - This command will undo the changes made in the last commit and move the current branch to the last commit. The changes will be removed from the staging area and returned to the Git state (working directory).
    - Useful when you want to undo a commit and make different changes before committing again.
    - Example:

      ```shell
      git reset --mixed HEAD~1
      ```

3. **`git reset --hard`:**
    - This command will undo the changes made in the last commit and move the current branch to the last commit. Additionally, it will delete all changes made, including those in the staging area and Git state.
    - Be careful when using `git reset --hard`, as it may cause permanent data loss. Use with caution.
    - Example:

      ```shell
      git reset --hard HEAD~1
      ```

Note that `HEAD~1` refers to the commit before the current HEAD, but you can specify any other commit if you wish.

**Important:** If you have already committed your changes and pushed them to a remote repository, be careful when using `git reset`, as this will change the commit history. It is not recommended to modify commit history on shared branches as it may cause problems for other contributors.

If you are unsure whether you should use `git reset` in your specific situation, consider creating a backup of your current branch or consulting with other contributors before doing so.