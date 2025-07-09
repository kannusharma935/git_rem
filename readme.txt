git init-> Powers your folder to be managed by git , and initializes a new empty repo. It also creates a .git folder that has all the relevent logic to manage versions of your project.

Working area->Staged Area->Repository

Working Area- in working area what ever changes you do in a file are not currently getting tracked by git. It means that changes done or to be done in those files are not managed by git yet. A file which is in working area is considered to be not in staging area.When we do git status and we see bunch of untracked files then they are actually called to be in working area.
    In working area you just started making a new file.

staging Area- What all files are going to be part of next version that we will create. This staging area is place where git knows what changes will be done from the last version to the next version.
git add file name