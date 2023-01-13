# Git  Notes
## commands
command for **creating a new user**: *$Git config --user.name "valor"*
command for **adding email user**: *$Git config --email "valor"*
command for **adding a new repository** git= *$git init (debe iniciarse en el directorio en el que se iniciara el proyecto)*

### work space

**Working directory** is where the working area is first located
After the files are edited saves can be saved and added to the staging area (**command for adding to the staging area**= *$agit add -A*
The last step is commiting files to the repository, **command for commiting**: *Git commit -m ""message"*

### commands for removing commits and stagging files
**Command for reverting files on stage**: *git rm --cached NAMEOFFILE*
**Command for removing commits**:*git reset CommitId* (head must be placed on the commmit for removing and the commitId should be the previous id that wants to be reseted to)
Da