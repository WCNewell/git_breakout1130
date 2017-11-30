Last login: Thu Nov 30 10:29:00 on ttys001
➜  ~ ~/desktop/playground
➜  playground git:(master) ✗ rm -rf .git
➜  playground mkdir git_breakout1130
➜  playground cd git_breakout1130
➜  git_breakout1130 ..
➜  playground rm -rf bit_breakout1130
➜  playground take git_breakout1130
➜  git_breakout1130 git init
Initialized empty Git repository in /Users/clarknewell/Desktop/playground/git_breakout1130/.git/
➜  git_breakout1130 git:(master) rm -rf .git
➜  git_breakout1130 touch index.html
➜  git_breakout1130 touch app.js style.css
➜  git_breakout1130 git init
Initialized empty Git repository in /Users/clarknewell/Desktop/playground/git_breakout1130/.git/
➜  git_breakout1130 git:(master) ✗ git add -a
error: unknown switch `a'
usage: git add [<options>] [--] <pathspec>...

    -n, --dry-run         dry run
    -v, --verbose         be verbose

    -i, --interactive     interactive picking
    -p, --patch           select hunks interactively
    -e, --edit            edit current diff and apply
    -f, --force           allow adding otherwise ignored files
    -u, --update          update tracked files
    -N, --intent-to-add   record only the fact that the path will be added later
    -A, --all             add changes from all tracked and untracked files
    --ignore-removal      ignore paths removed in the working tree (same as --no-all)
    --refresh             don't add, only refresh the index
    --ignore-errors       just skip files which cannot be added because of errors
    --ignore-missing      check if - even missing - files are ignored in dry run
    --chmod <(+/-)x>      override the executable bit of the listed files

➜  git_breakout1130 git:(master) ✗ git add -A
➜  git_breakout1130 git:(master) ✗
➜  git_breakout1130 git:(master) ✗ git commit -m "adding coold stuff"
[master (root-commit) abd780e] adding coold stuff
 Committer: Clark Newell <clarknewell@Clarks-MacBook-Pro.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 3 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 app.js
 create mode 100644 index.html
 create mode 100644 style.css
➜  git_breakout1130 git:(master) git push
fatal: No configured push destination.
Either specify the URL from the command-line or configure a remote repository using

    git remote add <name> <url>

and then push using the remote name

    git push <name>

➜  git_breakout1130 git:(master) git remote -v
➜  git_breakout1130 git:(master) git remote add origin https://github.com/WCNewell/git_breakout1130.git
➜  git_breakout1130 git:(master) git remove -v
git: 'remove' is not a git command. See 'git --help'.

The most similar command is
	remote
➜  git_breakout1130 git:(master) git remote -v
origin	https://github.com/WCNewell/git_breakout1130.git (fetch)
origin	https://github.com/WCNewell/git_breakout1130.git (push)
➜  git_breakout1130 git:(master) git add poop https://github.com/WCNewell/git_breakout1130.git
fatal: pathspec 'poop' did not match any files
➜  git_breakout1130 git:(master) git add remote poop https://github.com/WCNewell/git_breakout1130.git
fatal: pathspec 'remote' did not match any files
➜  git_breakout1130 git:(master) git add remote poop https://github.com/WCNewell/git_breakout1130.git
fatal: pathspec 'remote' did not match any files
➜  git_breakout1130 git:(master) git remote add poop https://github.com/WCNewell/git_breakout1130.git
➜  git_breakout1130 git:(master) git remote remove poop
➜  git_breakout1130 git:(master) git push
fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin master

➜  git_breakout1130 git:(master) git push -u origin master
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 252 bytes | 252.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/WCNewell/git_breakout1130.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.
➜  git_breakout1130 git:(master) git push
Everything up-to-date
➜  git_breakout1130 git:(master) touch readme.md
➜  git_breakout1130 git:(master) ✗ open readme.md
➜  git_breakout1130 git:(master) ✗