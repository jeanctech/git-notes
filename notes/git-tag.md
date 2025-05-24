# Git Tag

In Git, a Tag is a specific reference to a point in the history of the repository. Tags are used to mark specific versions of your project, such as release versions or important milestones, and are commonly used to indicate stable versions of software. Tags are immutable, meaning they cannot be changed after they are created.

Here's how to work with tags in Git:

1. **Create a lightweight tag:**

     A lightweight tag is simply a name associated with a specific commit. To create a lightweight tag, use the following command:

     ```shell
     git tag tag-name
     ```

     For example, to tag the current commit as "v1.0", you could do:

     ```shell
     git tag v1.0
     ```

2. **Create an annotated tag:**

     An annotated tag is a tag that includes a descriptive message. This is useful for providing additional information about the label. To create an annotated tag, use the `-a` command:

     ```shell
     git tag -a tag-name -m "Tag message"
     ```

     For example:

     ```shell
     git tag -a v1.0 -m "Version 1.0 released October 22, 2023"
     ```

3. **See tags:**

     You can list all the tags in your repository using the command:

     ```shell
     git tag
     ```

4. **View detailed information of a label:**

     You can view detailed information about a tag, including the commit it is associated with, using the following command:

     ```shell
     git show tag-name
     ```

     For example:

     ```shell
     git show v1.0
     ```

5. **Share tags:**

     Tags are not automatically pushed to remote repositories when you `git push`. To share tags, you must use the following command:

     ```shell
     git push origin tag-name
     ```

     For example:

     ```shell
     git push origin v1.0
     ```

     This will send the tag to the remote repository called "origin".

6. **Remove tags:**

     To remove a tag, use the following command:

     ```shell
     git tag -d tag-name
     ```

     You should also delete the tag in the remote repository if you have already shared it. To delete a tag in the remote repository, use:

     ```shell
     git push origin --delete tag-name
     ```

Tags are useful for marking important versions of your project and make it easy to identify milestones in the history of the repository.
