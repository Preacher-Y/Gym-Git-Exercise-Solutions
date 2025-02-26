# _*The Gym Git Exercise Solutions*_

## *Bundle 1*

### _Execises 1_
```bash 
gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git branch -m "main" "master"                          
gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git branch -m "master" "main"                          
gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git push

Everything up-to-date
gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git add . 

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git commit -m "after changing name from master to main"
[main f23f7e8] after changing name from master to main
 1 file changed, 6 insertions(+), 1 deletion(-)

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git checkout -b dev
Switched to a new branch 'dev'

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git checkout -b test
Switched to a new branch 'test'

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git push origin dev
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 342 bytes | 342.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/Preacher-Y/Gym-Git-Exercise-Solutions/pull/new/dev
remote: 
To https://github.com/Preacher-Y/Gym-Git-Exercise-Solutions
 * [new branch]      dev -> dev

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git push origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/Preacher-Y/Gym-Git-Exercise-Solutions/pull/new/test
remote: 
To https://github.com/Preacher-Y/Gym-Git-Exercise-Solutions
 * [new branch]      test -> test

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git branch  --delete test
error: Cannot delete branch 'test' checked out at '/Users/gymintore/Gym-Git-Exercise-Solutions'

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git checkout dev
Switched to branch 'dev'

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git branch -D test
Deleted branch test (was f23f7e8).

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git push origin 
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git push origin dev
Everything up-to-date

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git push origin -delete test
error: did you mean `--delete` (with two dashes)?

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git push origin --delete test
To https://github.com/Preacher-Y/Gym-Git-Exercise-Solutions
 - [deleted]         test
```

### _Execises 2_
```bash
gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git stash clear

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git pull
Already up to date.

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git push origin
Everything up-to-date

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git add home.html

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git stash
Saved working directory and index state WIP on main: 521ab43 readme up date

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html

nothing added to commit but untracked files present (use "git add" to track)

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git add .

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git stash
Saved working directory and index state WIP on main: 521ab43 readme up date

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git add . 

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git stash 
Saved working directory and index state WIP on main: 521ab43 readme up date

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git stash list
stash@{0}: WIP on main: 521ab43 readme up date
stash@{1}: WIP on main: 521ab43 readme up date
stash@{2}: WIP on main: 521ab43 readme up date

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (a3e54b9a27103a6307729bf1a0dd4c582d2145f7)

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git stash pop stash@{0}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   team.html

Dropped stash@{0} (ff2f0e7382c07b8d72eed7a44a24ba0c35a22373)

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git commit -m - a "bombclat"
error: pathspec 'a' did not match any file(s) known to git
error: pathspec 'bombclat' did not match any file(s) known to git

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git commit -a -m "bombclat"
[main 1148a92] bombclat
 2 files changed, 34 insertions(+)
 create mode 100644 about.html
 create mode 100644 team.html

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git stash pop stash@{2}     
fatal: log for 'stash' only has 1 entries

gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git stash pop stash@{0}
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

Dropped stash@{0} (55c9805f22e538a14265811830c3b3eda35f4a9d)
gymintore@Intores-iMac Gym-Git-Exercise-Solutions % git reset 
```

## *Bundle 2*

### _Exercise 1_

``` bash
 gymumutuzo@Umutuzos-iMac Gym-Git-Exercise-Solutions % git switch -C  ft/bundle-2
   Switched to a new branch 'ft/bundle-2'
   gymumutuzo@Umutuzos-iMac Gym-Git-Exercise-Solutions % git status
   On branch ft/bundle-2
   Untracked files:
     (use "git add <file>..." to include in what will be committed)
           bunde2/
   
   nothing added to commit but untracked files present (use "git add" to track)
   gymumutuzo@Umutuzos-iMac Gym-Git-Exercise-Solutions % git add. 
   git: 'add.' is not a git command. See 'git --help'.
   
   The most similar command is
           add

gymumutuzo@Umutuzos-iMac Gym-Git-Exercise-Solutions % git add .

gymumutuzo@Umutuzos-iMac Gym-Git-Exercise-Solutions % git status
  On branch ft/bundle-2
  Changes to be committed:
    (use "git restore --staged <file>..." to unstage)
          new file:   bunde2/services.html
  
  gymumutuzo@Umutuzos-iMac Gym-Git-Exercise-Solutions % git commit -m  "Creating a PullRequest" 
  [ft/bundle-2 9b30f3a] Creating a PullRequest
   1 file changed, 11 insertions(+)
   create mode 100644 bunde2/services.html
  gymumutuzo@Umutuzos-iMac Gym-Git-Exercise-Solutions % git push  
  fatal: The current branch ft/bundle-2 has no upstream branch.
  To push the current branch and set the remote as upstream, use
  
      git push --set-upstream origin ft/bundle-2
  
  To have this happen automatically for branches without a tracking
  upstream, see 'push.autoSetupRemote' in 'git help config'.

gymumutuzo@Umutuzos-iMac Gym-Git-Exercise-Solutions % git push --set-upstream origin ft/bundle-2
  Username for 'https://github.com': Preacher-Y
  Password for 'https://Preacher-Y@github.com': 
  Enumerating objects: 5, done.
  Counting objects: 100% (5/5), done.
  Delta compression using up to 8 threads
  Compressing objects: 100% (3/3), done.
  Writing objects: 100% (4/4), 690 bytes | 690.00 KiB/s, done.
  Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
  remote: 
  remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
  remote:      https://github.com/Preacher-Y/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
  remote: 
  To https://github.com/Preacher-Y/Gym-Git-Exercise-Solutions.git
   * [new branch]      ft/bundle-2 -> ft/bundle-2
  branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'
```
