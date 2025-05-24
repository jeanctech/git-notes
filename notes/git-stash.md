# Git Stash

`git stash` is a command in Git that is used to temporarily save changes to your local working directory that have not yet been committed in a commit. This is useful when you are working on a branch and need to temporarily switch to another branch or need to perform some kind of action that requires your working directory to be clean.

The `git stash` command takes changes to your working directory, saves them to a stash, and then reverts your working directory to the most recent state of the last commit. This allows you to make temporary changes without committing them to a commit. You can then apply the changes stored in the changes stack back to your working directory when necessary.

Here are some common `git stash` commands:

1. **Save changes to a stash:**

    ```shell
    git stash save "Descriptive message"
    ```

    This saves the changes to your working directory and stores them in a new stash with a descriptive message.

2. **List the stashes:**

    ```shell
    git stash list
    ```

    Shows a list of all stashes stored in your repository.

3. **Apply a stash:**

    ```shell
    git stash apply stash@{n}
    ```

    Where `stash@{n}` is the stash you want to apply. By default, `n` is 0 for the most recent stash. You can apply a specific stash to your working directory.

4. **Apply and remove a stash:**

    ```shell
    git stash pop stash@{n}
    ```

    This applies the stash and removes it from the changes stack.

5. **Delete a stash:**

    ```shell
    git stash drop stash@{n}
    ```

    Removes a specific stash from the changes stack. If you do not specify a stash, the most recent stash will be removed.

6. **Clear all stashes:**

    ```shell
    git stash clear
    ```

    Removes all stashes stored in the changes stack.

`git stash` is a useful tool to temporarily handle uncommitted changes in Git and allows you to switch between branches or perform other tasks without losing your changes. However, keep in mind that it is important to apply and remove stashes when you no longer need them to avoid unnecessary accumulation of temporary changes in your repository.
