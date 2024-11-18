# Github Fork

A Fork on GitHub refers to the creation of an independent copy of a
repository in your GitHub account. You can fork a repository to create your own version of the project without affecting the original repository. This is useful if you want to contribute to or make changes to the project without having direct write access to the original repository. Here are the steps to fork a repository on GitHub:

1. Sign in to your GitHub account: Make sure you are signed in to your GitHub account in your browser.

2. Find the repository you want to fork: Use the GitHub search bar or navigate to the repository you are interested in.

3. Fork the repository:
    - On the repository page, click the "Fork" button located in the upper right corner of the screen. This will create a copy of the repository in your account.

4. Wait for the fork to complete: GitHub will copy the original repository to your account. Depending on the size of the repository and the speed of your Internet connection, this process may take a while.

5. Work on your forked repository: You can now work on your own version of the repository. You can clone the forked repository to your local computer, make changes, create branches, and collaborate with other users.

6. Sync with the original repository (optional): If you want to keep your forked repository up to date with the original repository, you can set up a remote upstream and merge changes from the original repository into your fork. This is especially useful if you plan to contribute to the original project.

To sync with the original repository, you can follow these steps:

- Add a remote for the original repository to your forked repository:

    ```shell
    git remote add upstream https://github.com/usuario/original-repo.git
    ```

- Get the latest updates from the original repository:

    ```shell
    git fetch upstream
    ```

- Merge changes from the original repository into your main branch:

    ```shell
    git merge upstream/main
    ```

- You can then push your updated changes to your forked repository on GitHub.

Remember that forks are a core feature of GitHub that allows contributors to make changes to open source projects and contribute to the software development community in an easy and collaborative way.