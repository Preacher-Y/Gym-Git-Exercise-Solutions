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


