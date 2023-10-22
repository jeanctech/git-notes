# Collaborative Flow on Github

The collaborative workflow on GitHub involves multiple developers working together on a source code project using Git and GitHub. This process is based on collaboration, code review, and conflict management efficiently. Here I present a common collaborative workflow:

1. **Creating a remote repository:**
    - A collaborator (may be the project owner) creates a repository on GitHub and makes it public or private as needed.

2. **Clone the repository:**
    - Each collaborator clones the remote repository on their local computer using the `git clone` command. For example:
      ```shell
      git clone https://github.com/usuario/repo.git
      ```

3. **Create a branch for the job:**
    - Each contributor creates a local branch to work on a specific feature or fix. This helps keep work isolated and makes it easier to collaborate without affecting the main branch (usually called `main` or `master`).

      ```shell
      git checkout -b my-function
      ```

4. **Make changes:**
    - Each contributor makes changes to their local branch and makes regular commits to save their work. Use `git add` to prepare changes and `git commit` to commit them.

5. **Synchronize with remote repository:**
    - Before sharing your changes, make sure your local branch is in sync with the remote repository. Use `git pull` to get the latest updates and then `git push` to push your changes to the remote repository.

6. **Request a code review:**
    - Once you've finished your work on a branch, create a Pull Request (PR) on GitHub. In the pull request, provide details about what you've done and request a code review.

7. **Code Review:**
    - Other contributors or reviewers will review your code, make comments and suggest changes if necessary. This promotes code quality and effective collaboration.

8. **Resolve conflicts:**
    - If conflicts occur during code review, you will need to resolve them before your branch can be merged into the master branch. Use `git rebase` or `git merge` to address conflicts and then make a new commit.

9. **Approve and merge:**
    - Once the code review is complete and conflicts are resolved, a contributor with write permissions (often the project owner) will approve and merge the pull request into the master branch.

10. **Delete branches:**
     - After a branch has been successfully merged, you can delete it locally and in the remote repository if you no longer need it.

      ```shell
      git branch -d my-function # Delete locally
      git push origin --delete my-function # Delete in the remote repository
      ```

This is a basic collaborative workflow on GitHub. Depending on the project and team, other strategies may be used, such as using feature-specific branches, automated testing, or more elaborate review flows. The goal is to maintain an organized and efficient collaborative development process.
