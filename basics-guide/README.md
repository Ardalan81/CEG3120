# Project 0 Rubric

## Total Score: / 26

## Command Line Git ( / 15)


- **status**: Shows the current status of the working directory and staging area. It displays which changes have been staged, which haven't, and files that aren't being tracked by Git.
  - **Example**: `git status`

- **log**: Displays a history of commits on the current branch.
  - **Example**: `git log`

- **clone**: Creates a copy of an existing Git repository to your local machine.
  - **Example**: `git clone https://github.com/user/repo.git`

- **add**: Adds changes in the working directory to the staging area, preparing them for a commit.
  - **Example**: `git add file.txt`

- **rm (remove files from workspace examples)**: Removes files from the working directory and staging area.
  - **Example to untrack file**: `git rm --cached file.txt`
  - **Example to remove a file completely**: `git rm file.txt`

- **commit**: Records changes to the repository with a descriptive message.
  - **Example**: `git commit -m "Add new feature"`

- **push**: Uploads local repository changes to a remote repository like GitHub.
  - **Example**: `git push origin main`

- **fetch**: Downloads objects and refs from another repository. It fetches changes from the remote without merging them.
  - **Example**: `git fetch origin`

- **merge**: Combines changes from different branches into one.
  - **Example**: `git merge feature-branch`

- **pull**: Fetches changes from a remote repository and merges them into the current branch.
  - **Example**: `git pull origin main`

- **branch**: Lists, creates, or deletes branches.
  - **Example to list branches**: `git branch`
  - **Example to create a branch**: `git branch new-branch`

- **tag**: Creates, lists, or deletes tags.
  - **Example of creating tags**: `git tag v1.0`

- **checkout**: Switches to a different branch or restores files in the working directory to a previous state.
  - **Example**: `git checkout new-branch`

- **init**: Initializes a new Git repository in an existing directory.
  - **Example**: `git init`

- **remote**: Manages set repositories (remotes) to track and collaborate with.
  - **Example**: `git remote add origin https://github.com/user/repo.git`

## Git Files & Folders ( / 2)

- **.git folder**: A hidden folder that contains all metadata for the repository, such as commit history, branches, remote references, and configuration settings.

- **.gitignore file**: A file that specifies which files or directories to ignore and not track in the repository. Common entries might include:
  - `*.log` - Ignores all `.log` files
  - `node_modules/` - Ignores the `node_modules` folder
  - `.env` - Ignores environment variable files

## GitHub ( / 2)

- **Pull Requests**:
  - Pull request is a method for submitting changes to a repository.
  - **Different scenarios that creates pull request**:
    1. **Fork the repository**: Create your own copy of the repository to make changes.
    2. **Create a new branch**: Keep changes organized and separate from the `main` branch.
    3. **Make changes and commit them**: Use descriptive commit messages to explain what changes were made.
    4. **Push the branch to your fork**: Upload your changes to GitHub.
    5. **Open a Pull Request**: Compare your branch to the original repository and submit it for review.

## SSH ( / 2)

- **SSH authentication to repositories**:
  - **Why it matters**: Allows secure, password-less access to repositories.
  - **Steps**: Generate SSH keys using `ssh-keygen`, add the public key to your GitHub account, and clone the repository using SSH.
  - **Example**: `git clone git@github.com:user/repo.git`

- **SSH authentication to an AWS instance**:
  - **Why it matters**: Provides secure access to remote servers.
  - **Steps**: Use the `ssh` command with a `.pem` key file to connect to an AWS instance.
  - **Example**: `ssh -i "my-key.pem" ec2-user@ec2-**-**-**-**.amazonaws.com`

- **Using the config file in the `.ssh` folder**:
  - **Why it matters**: Simplifies SSH commands and saves time.
  - **Example `config` file**:
    ```plaintext
    Host myserver
        HostName ec2-**-**-**-**.amazonaws.com
        User ec2-user
        IdentityFile ~/.ssh/my-key.pem
    ```
  - **Connect using**: `ssh myserver`





