# Git on the Command Line

We can use the git version control application from the command line. Here aer some useful commands to get started.

-`git init` - this command will create a git repository in the current folderdir

- `git status` - this will give you the current status of your git repository
- `git add .` - Us ethis command to "stage" all of your current changes so that they are ready to be committed
- `git commit -m "your msg"` - this command will take all of the staged changes and create a snapshot of the current state of your repository. Using commits is how we generate a "commit history" for our repository
- `git pull` - Use this commmand to grab any changes form your remote repository (eg. github.com) and pull them down onto your local repository (the one on your computer)
- `git push` - This command will take whatever commits you have on your computer and push them to the remote repository on github.com

There are a lot of things learn whin it comes to working with git, but these commands are the day-to-day ones that you will do as you work with version control.

**Tip** You should make frequent, small commits when workin on your project

## Git CLI
The on-line tools for GitHub is called GitHub CLI; learn more at cli.github.com; need to download release for your machine. Check your release under Release Notes in the upper right corner.

To determine your version: click on start (window icon); select Settings (from side menu icons: gear); select System; select About. Under Device specifications see: System type: xx-bit operating system

Download your cli version and install, close and reopen your VS Code so it recongizes the new install.

Back to home page and press Manual (upper right corner)

## Remote Repositories

```shell
gh repo create my-first-repository
``` 
use to create repo on github.com. will create the origin (github.com) repo base the the current repository you have open in VS Code.

`gh auth login` can be used to log into github.com if you need to

`git push -u origin master` **first time you push to name the branch**: master, on github (origin). the -u is the local branch (check out lower left corner of your blue status line). -u long version is --set upstream

If you get an error: fatal ..not repository..., check that you are actually in your repository on your machine. Actually get into your repository: use File/Open folder, browse to the folder and select. Then connect your local repository to the newly created repository on github.com (created eariler with gh repo create command).

`git remote add origin https://github.com/xxxx/my-first-repository` where xxx is your username (dwelchnait).

problems with origin connection for your local repository

try `git remote remove origin` then check with `git remote -v` then re-add using `git remote add origin https://github.com/xxxxx/my-first-repository.git`






