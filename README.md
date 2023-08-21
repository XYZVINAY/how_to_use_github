#  BASIC COMMAND LINE OF GIT
### *FOR FIRST COMMIT*
- git init
  - *The command git init is used to initialize a new Git repository. This command creates a new .git subdirectory in the current working directory and sets up the necessary files and directories for Git to start tracking changes.*
## FOR CONNECT GIT TO GITHUB
- git config --global user.name "VINAY"
 - *to set the name of the user who made the commits in the repository.* 
- git config --global user.mail "email@gmail.com"
   - *to set the email address of the user who made the commits in the repository.*
- git remote add origin git@github.com:path_name
    - *Where you want to push*
    - for eg. *git remote add origin git@github.com:vinayprabhakarx/Machine-Learning.git*
- git branch -M main
    - *In which branch to push*
    - The -M option is used to force the rename even if the new branch name already exists. This command is useful when you want to change the name of your primary branch from master to main
- git push -u origin main
  - The -u option is used to set the upstream branch for the current branch. This means that in future, you can simply use git push instead of git push -u origin main
  #### SSH key genrate
  - ssh-keygen -t ed25519 -C "your_email@gmail.com"
    - *The commands you provided are used to generate an SSH key.*
  -  clip < ~/.ssh/id_ed25519.pub **_or_**
  - cat < ~/.ssh/id_ed25519.pub
    - *used to display the public key in the terminal.*
      - After generating an SSH key, you need to add the public key to your GitHub account. follow steps
        - Go to your GitHub account settings and click on “SSH and GPG keys”.
        - Click on “New SSH key”.
        - Give a title to the key and paste the public key in the “Key” field.
        - Click on “Add SSH key”.
## FOR ADD, COMMIT, PUSH, FULL AND DELETE CMD
1. git status
- used to display the current status of the Git repository
2. git add "file name"
- used to stage single file in the Git repository.
3. git add --a
-  used to stage all changes made to the Git repository.
4. git add .
- used to stage all changes made to the Git repository. This command adds all changes to the staging area
5. git commit -m " here any message write, what the changes here "
  -used to commit the changes made to the Git repository. This command creates a new commit with a message that describes the changes made in the commit.
6. git log
- to check commit status
7. git commit -a -m " message"
- used to commit all changes made to the Git repository. This command creates a new commit with a message that describes the changes made in the commit.
- The -a option is used to stage all changes before committing them.
8. git diff --stage
- This command shows the differences between the working directory and the staging area.
9. git push 
- used to push the changes made in the local branch to the remote repository. This command pushes the changes made in the local branch to the remote repository named origin.
10. git pull 
 - used to fetch and merge changes from the remote repository to the local repository. This command updates the local repository with the changes made in the remote repository.
11. rm -rf .git
- used to remove the Git repository from the current working directory. This command deletes the .git directory and all its contents. (*WARNING! THIS CMD USE WITH CAUTION NOR THEN USE YOUR ALL FILE OF GIT REPO*)
