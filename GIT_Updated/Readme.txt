=== GIT & GITHUB ===

Q1. Git
Ans: Git is a version control system.

Version control system(VCS) solves all of the below issues that we have faced:

Problem 1: 
We will lost our code when hard disk failure or computer crash.
Sol:
Sync it up from cloud.
Means, In VCS, the code is saved on cloud. Cloud is basically some remote machine which is much more stable than local computer and it's garrenty that we'll loose our code from cloud.


Problem 2:
Hard for multiple people to work on same code.
Sol:
Multiple people work on same code with their individula computers. Golden copy is maintained on cloud. Code merge happens using mergetool.
Mergetool here to resolve the conflict of code.


Problem 3:
Difficult to track changes revert back to previous version.
Sol:
In VCS, we have all changes trackdown.
VCS maintains version history, we can revert to any of the previous state of our code.


-> There are multiple VCS in market:
git, subversion, mercurial.
But git is by far better VCS

Why
- It's Distributed VCS where the version history is maintained on computer system.
- Github - Very popular website to host code is based on git


Q2. What is Github?
Ans:
Github is a website that allows us to store our code on the cloud. It is not juts a cloud storage but a full VCS powered by git.


== Pull Request Flow Diagram ==

Github code Repo -> Fork(copy) the code -> Guthub private Repo -> X person will make changes accordingly to make any changes -> After changes done they will push the code -> Git Private Repo -> Pull Request(To the code)


== Other Features of Github ==

1. Issues -> Issue Tracking
2. Wiki -> Write documentation for our code
3. Pulse 
4. Graphs -> Pulse and Graphs will give us statistics


== Basic Commands: Add, Commit, Push ==

1. Create/ Import Repo
2. Clone/ Download Repo

-> For cloning repo we have below cmd:

git clone <https://github.com/url_name>

Below are some cmds (in double quotes) will helps us:

-> "ls" (To check the list of folders in the directory)

-> "cd" <folder_name> (with this we'll go inside of folder)

-> "cd .." (with this we can back from current folder)

-> "git status" (will show status)

-> "git add <file_name>" (When we need a file in the directory.
This will add file to staging area. Later on staging area will be used to commit files when we run "git commit" cmt)

-> "git commit -m '<Need to provide msg>' "
(git commit cmd adds changes to local version control database. We have still not pushed these changes to remote server i.e. github)

-> "git log" (It will show us logs of commit)

-> "git push" (It will now push commited changes to remote server i.e. github)

-> "git difftool" (It will shows difference between our local changes and previous version of file)


NOTE:
Git cmd line interface is preferred our GUI plugins that come with many IDEs. This is because cmds give us much more power and flexibility.



== Undoing/Reverting/Resetting code changes ==

1. For Undo uncommited changes -> "git checkout --"
2. For Undo commited changes -> "git revert"
3. Resetting changes -> "git reset"

