# Ssh Authentication - Github

Ssh authentication in Git is used to establish a secure connection between your computer and a remote Git server, such as GitHub, GitLab, or Bitbucket. Ssh authentication relies on the use of Ssh keys to verify the user's identity and allow access to remote repositories. Below are general steps to configure SSH authentication in Git.

1. Generate an Ssh key pair

    On your computer, open a terminal and run the following command to generate an SSH key pair (public and private key). If you already have an SSH key pair, you can skip this step:

    ```shell
    ssh-keygen -t rsa -b 4096 -C "your_mail@example.com"
    ```

    Replace "your_mail@example.com" with your email address. You can leave the password blank if you do not want to protect your private key with a password.

2. Add your Ssh key to an Ssh agent (optional but recommended):

    You can use an Ssh agent to manage your keys more securely and avoid having to enter the private key password every time you connect to the remote server. Run the following commands:

    ```shell
    eval "$(ssh-agent -s)"
    ssh-add ~/.ssh/id_rsa
    ```

    Make sure `~/.ssh/id_rsa` is the location of your private key if you used a different path.

3. Copy your public key to the clipboard:

    You can use the following command to copy your public key to the clipboard:

    ```shell
    pbcopy < ~/.ssh/id_rsa.pub
    ```

4. Add the public key to your account on the remote Git server:

    Sign in to your account on the remote Git server (for example, GitHub, GitLab, or Bitbucket) and look for the SSH key configuration section. Then, paste the public key that you copied in the previous step into the corresponding field and save it.

5. Verify Ssh configuration:

    To verify that your Ssh configuration is working correctly, run the following command:

    ```shell
    ssh -T git@github.com
    ```

    Make sure to replace `github.com` with the URL of the remote Git server you are using. You should receive a message confirming that you have been successfully authenticated.

With Ssh authentication configured, you can perform Git operations (clone, push, pull, etc.) on remote repositories without entering passwords, improving security and convenience.