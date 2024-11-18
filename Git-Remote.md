# Git Remote

`git remote` is a command in Git used to manage connections to remote repositories. Allows you to view, add, rename, and delete references to remote repositories. Remote repositories are versions of your project that are stored on online servers, such as GitHub, GitLab, or Bitbucket. Here are some common operations you can perform with `git remote`:

1. **List remote repositories:** You can list the remote repositories linked to your local repository using:

    ```shell
    git remote
    ```

    This will list the names of the remote repositories, for example `origin`.

2. **View details of a remote repository:** You can view the URL of a remote repository and other details using:

    ```shell
    git remote show remote-repository-name
    ```

    For example, to view the details of the remote repository named `origin`:

    ```shell
    git remote show origin
    ```

3. **Add a new remote repository:** If you want to link your local repository with a remote repository, you can use:

    ```shell
    git remote add remote-repository-name remote-repository-url
    ```

    For example:

    ```shell
    git remote add upstream https://github.com/usuario/repo-fuente.git
    ```

    This creates a new reference called `upstream` that points to the specified remote repository.

4. **Rename a remote repository:** To change the name of a remote repository, you can use:

    ```shell
    git remote rename old-name new-name
    ```

    For example, to rename the remote repository from `origin` to `github`:

    ```shell
    git remote rename origin github
    ```

5. **Delete a remote repository:** If you want to delete a reference to a remote repository, you can use:

    ```shell
    git remote remove remote-repository-name
    ```

    For example:

    ```shell
    git remote remove github
    ```

    This will remove the reference to the remote repository, but will not remove any related commits or branches.

`git remote` is useful when you work on collaborative projects or when you want to interact with multiple remote repositories. You can easily add, remove, and manage these connections to remote repositories as needed to keep your project in sync and collaborate with other developers.