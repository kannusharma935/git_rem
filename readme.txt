git init-> Powers your folder to be managed by git , and initializes a new empty repo. It also creates a .git folder that has all the relevent logic to manage versions of your project.

Working area->Staged Area->Repository

Working Area- in working area what ever changes you do in a file are not currently getting tracked by git. It means that changes done or to be done in those files are not managed by git yet. A file which is in working area is considered to be not in staging area.When we do git status and we see bunch of untracked files then they are actually called to be in working area.
    In working area you just started making a new file.

staging Area- What all files are going to be part of next version that we will create. This staging area is place where git knows what changes will be done from the last version to the next version.

to add file to stage area->git add file name.
to remove file from stage area-> git rm --cached filename

Repository Area- This area actually contains of all the previous registered version.
And the files in this area, git already manages them and knows their version history.

In git version are managed using commit.

1 git commit= 1 version

commit- commit is a perticular version of the project. It captures a snapshot of the project'sstaged changes and creates a version out of it.

git commit- registers staging changes to a commit.

GIT LOG- list down all the commits of the Repository. if you want to exit out of git log prompt press 'q'.

git restore <filename>- it removes all files changes from the staging area to be commited. This can be useful, if we did some dirty piece of code and now no more want it. Instead of deleting every change line by line, we can restore it or you can restore last clean version of file.
this is for working area

git restore -- Staged <filename>- for staging area. It removes file from changes from stag area to working area.



 Diff b/w git rm and git restore.
 ans- if you want to move the whole file back to the untracked state, then we do git rm , otherwise if we just want the changes to be moved in working area or staging are then we do git restore.

 git diff commitid_a commitid_b -this command shows the diff b/w both commits in a file .


 Remote connection - It helps you to link two git repositories for uploading and downloading changes from each otherwise

 git remote add <name of remote> <link of the remote> :this command helps us to add a new link to the remote repo and give a name to it.

 git remote rm <name of remote> : this command deletes a remote connection

 git remote rename <oldname> <newname> : this command renames the remote connection

 Note: the name of the remote connection is alwas used to establish communication

 git add <file1> <file2> <file3>: this command will add multiple  file changes together is the staging area

 git add . : this command will add all files from working repo to staging area.
 