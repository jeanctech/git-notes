# Git Add and Git Commit

`git add` and `git commit` are two fundamental commands in Git used to manage changes to your repository. Here I explain how they work:

1. **`git add`**: This command is used to move changes from the working directory to the staging area, where the changes to be included in the next commit are selected.

    - To add a specific file to the staging area:
      ```shell
      git add file-name
      ```

    - To add all changes (new, modified and deleted files) to the staging area:
      ```shell
      git add .
      ```

    - To add all changes from a specific directory to the staging area:
      ```shell
      git add directory-name/
      ```

    After using `git add`, the selected changes are ready to be committed in the next commit.

2. **`git commit`**: This command is used to create a new commit containing the changes in the staging area. Each commit is identified with a descriptive message that explains what changes are being made.

    - To commit a message directly from the command line:
      ```shell
      git commit -m "Commit message"
      ```

    - If you omit the `-m` option, Git will open a text editor where you can type the commit message.

    - You can use `git commit` multiple times to create a series of commits that represent the changes made to the project.

After creating a commit, changes are recorded in the repository history and stored securely. Each commit has a unique identifier (hash) that makes it referenceable.

The typical workflow with `git add` and `git commit` involves adding changes, making regular commits with descriptive messages, and finally sharing the updated commits with other collaborators via `git push` to a remote repository, such as GitHub.

It's important to remember that commits are immutable in Git, meaning they cannot be modified once created. Therefore, it is essential to be descriptive and clear in commit messages so that other developers can understand the changes made to the project.
