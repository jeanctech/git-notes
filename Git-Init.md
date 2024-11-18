# Git Init

`git init` is a command in Git used to initialize a new Git repository in an empty directory or create a new repository in an existing directory. When you run `git init`, Git creates a directory structure and hidden files in the specified directory so you can start tracking and managing versions of your source code. Here are the basic steps to use `git init`:

1. **Navigate to the project directory:** Open a terminal and navigate to the directory where you want to create a new Git repository.

2. **Run `git init`:** Once you are in the project directory, run the following command:

    ```shell
    git init
    ```

    This will create a hidden subdirectory called ".git" in the current directory, which will contain all the information needed to track the changes and history of the project.

3. **Add files and make commits:** From this point, you can start working on your project. You can add files with `git add` and commit with `git commit` to track changes. For example:

    ```shell
    git add file-name
    git commit -m "Commit message"
    ```

4. **Set up your information:** It is important to set up your username and email address in Git so that commits correctly reflect who made the changes. You can configure this information at the global level or at the project level. At a global level:

    ```shell
    git config --global user.name "Your Name"
    git config --global user.email "your_email@example.com"
    ```

These are the basic steps to initialize a Git repository with `git init`. Once you've done these steps, Git will be ready to track and manage your project's history in that directory.