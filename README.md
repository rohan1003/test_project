1.	 git init project1
	git init project 2
	
2.	cd project1
	vi a.txt
	git add a.txt
	git commit -m 'c0'

3.	git checkout -b staging
	Switched to a new branch 'staging'
	
4.	vi test1.txt
	git add test1.txt
	git commit -m 'c1 first commit in staging'
[staging 43315d8] c1 first commit in staging
 1 file changed, 1 insertion(+)
 create mode 100644 test1.txt

5.	 git remote add origin https://github.com/rohan1003/test_project.git
	
	git push --all origin
Username for 'https://github.com': rohan1003
Password for 'https://rohan1003@github.com': 
Counting objects: 6, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (6/6), 480 bytes | 0 bytes/s, done.
Total 6 (delta 0), reused 0 (delta 0)
To https://github.com/rohan1003/test_project.git
 * [new branch]      master -> master
* [new branch]      staging -> staging

6.	cd ..
	cd project2

7.	git clone https://github.com/rohan1003/test_project.git
Cloning into 'test_project'...
remote: Counting objects: 6, done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 6 (delta 0), reused 6 (delta 0), pack-reused 0
Unpacking objects: 100% (6/6), done.
Checking connectivity... done.


8.	git checkout --track origin/staging
Branch staging set up to track remote branch staging from origin.
Switched to a new branch 'staging'


9.	vi test1.txt
	 git commit -a -m 'c2 in project2 modify test1'
[staging de283d2] c2 in project2 modify test1
 1 file changed, 1 insertion(+), 1 deletion(-)


10.	git push origin staging
Username for 'https://github.com': rohan1003
Password for 'https://rohan1003@github.com': 
Counting objects: 6, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 301 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/rohan1003/test_project.git
   43315d8..de283d2  staging -> staging


11.	cd ..
	cd ..
	cd project1


12.	git checkout staging


13.	vi test1.txt
	git commit -a -m 'c3 back in pro2’'
[staging 9a58c95] c3 back in pro1
 1 file changed, 1 insertion(+), 1 deletion(-)


14.	 git push origin staging
Username for 'https://github.com': rohan1003
Password for 'https://rohan1003@github.com': 
To https://github.com/rohan1003/test_project.git
 ! [rejected]        staging -> staging (fetch first)
error: failed to push some refs to 'https://github.com/rohan1003/test_project.git'
{We are trying to push in a branch which already has some changes and we don't have info. We first need to fetch those changes only then we can push it again}


15.	git checkout master
Switched to branch 'master'


16.	git merge staging
Updating 9a90707..9a58c95
Fast-forward
 test1.txt | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 test1.txt


17.	git branch testing
	git checkout testing



18.	vi test1.txt
	commit -a -m 'ca A is an alphabet
'

19.	vi test1.txt
	commit -a -m 'cb B is an alphabet
'
	vi test1.txt
	commit -a -m 'cc C is an alphabet
'
	vi test1.txt
	commit -a -m 'cd D is an alphabet
'
	vi test1.txt
	commit -a -m 'ce E is an alphabet
'
	vi test1.txt
	commit -a -m 'cf F is an alphabet
'
	vi test1.txt
	commit -a -m 'cg G is an alphabet
'
	vi test1.txt
	commit -a -m 'ch H is an alphabet
'


20.	git push origin testing
Username for 'https://github.com': rohan1003
Password for 'https://rohan1003@github.com': 
Counting objects: 31, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (20/20), done.
Writing objects: 100% (30/30), 2.58 KiB | 0 bytes/s, done.
Total 30 (delta 0), reused 0 (delta 0)
To https://github.com/rohan1003/test_project.git
* [new branch]      testing -> testing


21.	git checkout master


22.	vi test1.txt
	git commit -a -m 'commit1 1 is a number'
[master 65a7fbf] commit1 1 is a number
 1 file changed, 1 insertion(+), 1 deletion(-)


23.	vi test1.txt
	git commit -a -m 'commit2 2 is a number'
[master 65a7fbf] commit2 2 is a number
 1 file changed, 1 insertion(+), 1 deletion(-)

	vi test1.txt
	git commit -a -m 'commit3 3 is a number'
[master 65a7fbf] ‘commit 3 3 is a number’
 1 file changed, 1 insertion(+), 1 deletion(-)

	vi test1.txt
	git commit -a -m 'commit4 4 is a number'
[master 65a7fbf] commit4 4 is a number
 1 file changed, 1 insertion(+), 1 deletion(-)

	vi test1.txt
	git commit -a -m 'commit5 5 is a number'
[master 65a7fbf] commit5 5 is a number
 1 file changed, 1 insertion(+), 1 deletion(-)

	vi test1.txt
	git commit -a -m 'commit6 6 is a number'
[master 65a7fbf] commit6 6 is a number
 1 file changed, 1 insertion(+), 1 deletion(-)

	vi test1.txt
	git commit -a -m 'commit7 7 is a number'
[master 65a7fbf] commit7 7 is a number
 1 file changed, 1 insertion(+), 1 deletion(-)

	vi test1.txt
	git commit -a -m 'commit8 8 is a number'
[master 65a7fbf] commit8 8 is a number
 1 file changed, 1 insertion(+), 1 deletion(-)

	
24.	 git push origin master
Username for 'https://github.com': rohan1003
Password for 'https://rohan1003@github.com': 
Counting objects: 29, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (16/16), done.
Writing objects: 100% (24/24), 2.00 KiB | 0 bytes/s, done.
Total 24 (delta 0), reused 0 (delta 0)
To https://github.com/rohan1003/test_project.git
   9a90707..68f31f4  master -> master


25.	 git rebase testing

Applying: commit1 1 is a number
Using index info to reconstruct a base tree...
M	test1.txt
Falling back to patching base and 3-way merge...
Auto-merging test1.txt
CONFLICT (content): Merge conflict in test1.txt
Failed to merge in the changes.
Patch failed at 0001 commit1 1 is a number.


When you have resolved this problem, run "git rebase --continue".
If you prefer to skip this patch, run "git rebase --skip" instead.
To check out the original branch and stop rebasing, run "git rebase --abort".

 git add test1.txt
 git rebase --continue
Applying: commit1 1 is a number
Applying: commit2 2 is a number
Using index info to reconstruct a base tree...
M	test1.txt
Falling back to patching base and 3-way merge...
Auto-merging test1.txt
CONFLICT (content): Merge conflict in test1.txt
Failed to merge in the changes.
Patch failed at 0002 commit2 2 is a number
When you have resolved this problem, run "git rebase --continue".
If you prefer to skip this patch, run "git rebase --skip" instead.
To check out the original branch and stop rebasing, run "git rebase --abort".

 git add test1.txt
 git rebase --continue
Applying: commit2 2 is a number
Applying: commit3 3 is a number
Using index info to reconstruct a base tree...
M	test1.txt
Falling back to patching base and 3-way merge...
Auto-merging test1.txt
CONFLICT (content): Merge conflict in test1.txt
Failed to merge in the changes.
Patch failed at 0003 commit3 3 is a number

When you have resolved this problem, run "git rebase --continue".
If you prefer to skip this patch, run "git rebase --skip" instead.
To check out the original branch and stop rebasing, run "git rebase --abort".

 git add test1.txt
 git rebase --continue
Applying: commit3 3 is a number
Applying: commit4 4 is a number
Using index info to reconstruct a base tree...
M	test1.txt
Falling back to patching base and 3-way merge...
Auto-merging test1.txt
CONFLICT (content): Merge conflict in test1.txt
Failed to merge in the changes.
Patch failed at 0004 commit4 4 is a number

When you have resolved this problem, run "git rebase --continue".
If you prefer to skip this patch, run "git rebase --skip" instead.
To check out the original branch and stop rebasing, run "git rebase --abort".

 git add test1.txt
 git rebase --continue
Applying: commit4 4 is a number
Applying: commit5 5 is a number
Using index info to reconstruct a base tree...
M	test1.txt
Falling back to patching base and 3-way merge...
Auto-merging test1.txt
CONFLICT (content): Merge conflict in test1.txt
Failed to merge in the changes.
Patch failed at 0005 commit5 5 is a number

When you have resolved this problem, run "git rebase --continue".
If you prefer to skip this patch, run "git rebase --skip" instead.
To check out the original branch and stop rebasing, run "git rebase --abort".

 git add test1.txt
 git rebase --continue

Applying: commit5 5 is a number
Applying: commit6 6 is a number
Using index info to reconstruct a base tree...
M	test1.txt
Falling back to patching base and 3-way merge...
Auto-merging test1.txt
CONFLICT (content): Merge conflict in test1.txt
Failed to merge in the changes.
Patch failed at 0006 commit6 6 is a number

When you have resolved this problem, run "git rebase --continue".
If you prefer to skip this patch, run "git rebase --skip" instead.
To check out the original branch and stop rebasing, run "git rebase --abort".

 git add test1.txt
 git rebase --continue
Applying: commit6 6 is a number
Applying: commit7 7is a number
Using index info to reconstruct a base tree...
M	test1.txt
Falling back to patching base and 3-way merge...
Auto-merging test1.txt
CONFLICT (content): Merge conflict in test1.txt
Failed to merge in the changes.
Patch failed at 0007 commit7 7is a number

When you have resolved this problem, run "git rebase --continue".
If you prefer to skip this patch, run "git rebase --skip" instead.
To check out the original branch and stop rebasing, run "git rebase --abort".

 git add test1.txt
git rebase --continue
Applying: commit7 7is a number
Applying: commit8 8is a number
Using index info to reconstruct a base tree...
M	test1.txt
Falling back to patching base and 3-way merge...
Auto-merging test1.txt
CONFLICT (content): Merge conflict in test1.txt
Failed to merge in the changes.
Patch failed at 0008 commit8 8is a number

When you have resolved this problem, run "git rebase --continue".
If you prefer to skip this patch, run "git rebase --skip" instead.
To check out the original branch and stop rebasing, run "git rebase --abort".

 git add test1.txt
 git rebase --continue
Applying: commit8 8is a number
	

26.	cd ..
	cd project2
	cd test_project


27.	git fetch
remote: Counting objects: 51, done.
remote: Compressing objects: 100% (34/34), done.
remote: Total 51 (delta 1), reused 50 (delta 0), pack-reused 0
Unpacking objects: 100% (51/51), done.
From https://github.com/rohan1003/test_project
   9a90707..68f31f4  master     -> origin/master
* [new branch]      testing    -> origin/testing
	
	git checkout --track origin/testing
Branch testing set up to track remote branch testing from origin.
Switched to a new branch 'testing'

28.	git checkout master

29.	git merge testing
Updating 9a90707..5e9e8ed
Fast-forward
 test1.txt | 4 ++++
 1 file changed, 4 insertions(+)
 create mode 100644 test1.txt

30. 	Now after merge, master and testing point to the same commit
	Before that we  first fetch the changes from the remote repo and start tracking the testing branch.


