# Git  Notes
## commands
command for **creating a new user**: *$Git config --user.name "valor"*<br>
command for **adding email user**: *$Git config --email "valor"*<br>
command for **adding a new repository** git= *$git init (debe iniciarse en el directorio en el que se iniciara el proyecto)*<br>

### work space

**Working directory** is where the working area is first located<br>
After the files are edited saves can be saved and added to the staging area (**command for adding to the staging area**= *$agit add -A*<br>
The last step is commiting files to the repository, **command for commiting**: *$Git commit -m ""message"*<br>

### commands for removing commits and stagging files<br>
**Command for reverting files on stage**: *$git rm --cached NAMEOFFILE*<br>
**Command for removing commits**:*$git reset CommitId* (head must be placed on the commmit for removing and the commitId should be the previous id that wants to be reseted to)



# GIt HUb

## SSH keyh generation
**encrypted ssh key generator command**:  sshckeygen command: *$ssh-keygen -t ed25519* (bst protocol recommended by github) *-C "moseshawkdev@gmail.com"*
Press enter when asking to generate file.<br>
ask for a enterphrase (optional)<br>
**command for reading the generated file** , first for move to .ssh directiory, *$cd .ssh*, and *$cat id_ed25519.pub*<br>
**command for confirming ssh key working**: *$eval "$(ssh-agent) -S)"*<br>
**command for adding public key to private** *$ ssh-add ~/.ssh/id_ed25519*<br>
**command for veryfing comunication with github**: *$ssh -T git@github.com*

## Adding repositorys to remote (github)

**command for adding local git to remote** *git remote add origin git@github.com:MosesHawk/Kodemia-Notes.git*<br>
**command for uploading commits to the remote repository**: *git push* first time with -set upstream <br>
**complete command for uploading commits to remote**: *git push --set origin master* <--this is the name of the branch that is holding the commit<br>
