# Redelivering Branches - Git

In Git, rejoining a branch usually means merging a child branch back into the main branch (such as `master` or `main`) after you've worked on it separately. This is common practice to incorporate feature changes, bug fixes, or other developments in an orderly manner. Reintegration is generally done through a merger.

Next, I will explain how to reintegrate a branch in Git:

Let's say you have a branch called `my-feature-branch` that you've been working on and you want to push it back into the `master` branch.

1. **Make sure you are on the Target Branch (e.g. `master`):**

    ```shell
    git checkout master
    ```

2. **Perform a Fusion to Reintegrate the Branch:**

    Use the `git merge` command to merge the child branch into the parent branch:

    ```shell
    git merge my-feature-branch
    ```

    This will push the changes from `my-feature-branch` to the `master` branch.

3. **Resolve Possible Conflicts:**

    If there are conflicts between the two branches (for example, simultaneous changes to the same lines in a file), Git will stop the merge and ask you to resolve the conflicts manually. You must edit the conflicting files, save your changes, and then perform a commit to complete the merge.

4. **Confirm the Merger:**

    Once you've resolved the conflicts, perform a commit to complete the merge:

    ```shell
    git commit -m "Merge my-feature-branch into master"
    ```

    This will log the merge in the commit history of the `master` branch.

5. **Delete the Secondary Branch (Optional):**

    If you no longer need the child branch, you can delete it with the following command:

    ```shell
    git branch -d my-feature-branch
    ```

    Make sure you're done with the branch before deleting it.

These are the basic steps to check back a branch into Git. Reintegration is a common practice in software development to push feature changes or bug fixes to the main branch in a controlled and organized manner.
