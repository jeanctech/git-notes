# Pull Request - Github

A "PR" or "Pull Request" is a key feature of GitHub that allows developers to collaborate on open source or private projects. A PR is used to propose changes to a repository and request that the repository owners review them and, if deemed appropriate, merge them into the main project. Here's how to create a PR on GitHub:

1. **Clone the Repository:**
    Before creating a PR, you need to have a local copy of the repository you want to contribute to. You can clone the repository to your computer using the `git clone` command if you haven't already.

    ```shell
    git clone repository-url
    ```

2. **Create a Local Branch:**
    It is good practice to create a local branch to work on the feature or fix you want to implement. This keeps your main branch clean and isolated from your changes. You can create a new branch and switch to it with the following commands:

    ```shell
    git checkout -b branch-name
    ```

3. **Make your Local Changes:**
    Make any necessary changes to your local branch, whether to fix bugs, add new features, or perform any other task that requires code changes.

4. **Confirm your Changes:**
    Once you've made your changes, commit the changes to your local branch using `git commit`. Be sure to include descriptive confirmation messages.

    ```shell
    git add .
    git commit -m "Message describing the changes"
    ```

5. **Push your Branch to the Remote Repository:**
    In order for others to review your changes, you must push your branch and changes to the remote repository on GitHub. Use the `git push` command to do this:

    ```shell
    git push origin branch-name
    ```

6. **Create the Pull Request on GitHub:**
    Go to your repository page on GitHub and select the "Pull Requests" tab. Then, click the “New Pull Request” button. GitHub will show you a comparison of the branches and changes made.

7. **Complete the PR:**
    Add a title and description for the PR, explaining your changes and why they should be merged. You can mention specific people to review your changes.

8. **Request Review:**
    After creating the PR, ask reviewers to review your changes. Reviewers can comment, approve, or request additional changes.

9. **Resolve Comments:**
    If reviewers make comments or request changes, make the necessary adjustments to your local branch, and then commit and push the changes again. The PR will be updated automatically.

10. **PR Fusion:**
     Once the PR has been reviewed and approved, a repository maintainer (or yourself if you have permissions) can merge it. This will push your changes into the main branch of the project.

Creating a PR on GitHub is a fundamental process for collaborating on projects and allows teams to review and approve changes in a controlled manner. It is a common practice in collaborative software development and essential in open source projects.