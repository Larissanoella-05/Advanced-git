**Part 1 *GETTING STARTED***

```bash
1. Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ touch test{1..4}.md

 Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git add test1.md && git commit -m "chore: Create initial file"
[main (root-commit) c0a7ae4] chore: Create initial file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test1.md

 Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git add test2.md && git commit -m "chore: Create another file"
[main 96a44c9] chore: Create another file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test2.md

 Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git add test3.md && git commit -m "chore: Create third and fourth files"
[main 514e615] chore: Create third and fourth files
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test3.md
```

```bash
2. Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git status
On branch main
Your branch is based on 'origin/main', but the upstream is gone.
  (use "git branch --unset-upstream" to fixup)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test4.md

nothing added to commit but untracked files present (use "git add" to track)

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git log
commit 514e615e33438eb9a484d4a2fb754310b789ff08 (HEAD -> main)
Author: larissanoellaa-05 <s.noella@alustudent.com>
Date:   Thu Feb 27 16:29:11 2025 +0200        

    chore: Create third and fourth files      

commit 96a44c911ca1ea53a42e8b0c76e66dfb819ee01f
Author: larissanoellaa-05 <s.noella@alustudent.com>
Date:   Thu Feb 27 16:29:01 2025 +0200        

    chore: Create another file

commit c0a7ae4c770af390cf92d05c42360a305a46b5da
Author: larissanoellaa-05 <s.noella@alustudent.com>
Date:   Thu Feb 27 16:28:49 2025 +0200        

    chore: Create initial file

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git add test4.md

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git commit --amend
hint: Waiting for your editor to close the fil
[main f1717d8] chore: Create third and fourth files
 Date: Thu Feb 27 16:29:11 2025 +0200
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test3.md
 create mode 100644 test4.md
```

2.

```jsx
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git rebase -i HEAD~2
hint: Waiting for your editor to close the fil
hint: Waiting for your editor to close the fil
[detached HEAD 2f0c3b9] chore: Create second file
 Date: Thu Feb 27 16:29:01 2025 +0200
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test2.md
Successfully rebased and updated refs/heads/main.

3.
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git rebase -i --root
hint: Waiting for your editor to close the fil
hint: Waiting for your editor to close the fil
[detached HEAD c0ab087] chore: Create initial file
 Date: Thu Feb 27 16:28:49 2025 +0200
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test1.md
 create mode 100644 test2.md
Successfully rebased and updated refs/heads/main.
```

3.

4.

```jsx
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git reset HEAD~

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git git status
git: 'git' is not a git command. See 'git --help'.

The most similar command is
        init

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$  git status
On branch main
Your branch is based on 'origin/main', but the upstream is gone.
  (use "git branch --unset-upstream" to fixup)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test3.md
        test4.md

nothing added to commit but untracked files present (use "git add" to track)

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git add test3.md 

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git commit -m"Create Third File"
[main 2c42382] Create Third File
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test3.md

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git add .

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git commit -m"Create Fourth File"
[main 52ba936] Create Fourth File
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test4.md
```

5.

```jsx
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git rebase -i --root
hint: Waiting for your editor to close the fil
hint: Waiting for your editor to close the fil
[detached HEAD 1a9b596] Create Third File and  Fourth File
 Date: Thu Feb 27 16:45:31 2025 +0200
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test3.md
 create mode 100644 test4.md
Successfully rebased and updated refs/heads/main.
```

6.

```jsx
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ touch unwanted.txt

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git add unwanted.txt 

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git commit -m"Unwanted commit"
[main 1767593] Unwanted commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 unwanted.txt

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git rebase -i --root
hint: Waiting for your editor to close the fil
Successfully rebased and updated refs/heads/main.
```

7.

```jsx
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git rebase -i --root
hint: Waiting for your editor to close the fil
Successfully rebased and updated refs/heads/main.
```

8.

```jsx
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (ft/branch)
$ ls
test1.md  test2.md  test3.md  test4.md  test5.md

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (ft/branch)
$ git log
commit b24ffe9604acfd0fd2675d5efa16473bb5b06173 (HEAD -> ft/branch)
Author: larissanoellaa-05 <s.noella@alustudent.com>
Date:   Thu Feb 27 17:18:15 2025 +0200

    Implemented test 5

commit fb5fdd422b3a9334c6b7e9375ff73f3ac54601b1 (main)
Author: larissanoellaa-05 <s.noella@alustudent.com>
Date:   Thu Feb 27 16:28:49 2025 +0200

    chore: Create initial file
    
    chore: Create second file

commit 97d1ca21b7538058ca394a50eaf0bf0d197d4954
Author: larissanoellaa-05 <s.noella@alustudent.com>
Date:   Thu Feb 27 16:45:31 2025 +0200

    Create Third File and  Fourth File

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (ft/branch)
$ switch main
bash: switch: command not found

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (ft/branch)
$ git switch main 
Switched to branch 'main'
Your branch is based on 'origin/main', but the upstream is gone.
  (use "git branch --unset-upstream" to fixup)

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git cherry-pick b24ffe9604acfd0fd2675d5efa16473bb5b06173
[main 9b8ce66] Implemented test 5
 Date: Thu Feb 27 17:18:15 2025 +0200
 1 file changed, 2 insertions(+)
 create mode 100644 test5.md
```

```jsx

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git adog
* 9b8ce66 (HEAD -> main) Implemented test 5
| * b24ffe9 (ft/branch) Implemented test 5
|/  
* fb5fdd4 chore: Create initial file
* 97d1ca2 Create Third File and  Fourth File

```

```jsx

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git adog
* 9b8ce66 (HEAD -> main) Implemented test 5
| * b24ffe9 (ft/branch) Implemented test 5
|/  
* fb5fdd4 chore: Create initial file
* 97d1ca2 Create Third File and  Fourth File
```

```jsx
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git reflog
9b8ce66 (HEAD -> main) HEAD@{0}: cherry-pick: Implemented test 5
fb5fdd4 HEAD@{1}: checkout: moving from ft/branch to main
b24ffe9 (ft/branch) HEAD@{2}: commit: Implemented test 5
fb5fdd4 HEAD@{3}: checkout: moving from main to ft/branch
fb5fdd4 HEAD@{4}: rebase (finish): returning to refs/heads/main
fb5fdd4 HEAD@{5}: rebase (pick): chore: Create initial file
97d1ca2 HEAD@{6}: rebase (pick): Create Third File and Fourth File
dce5720 HEAD@{7}: rebase (start): checkout dce5720355652f4e876d0bc0a1e1d7f688332b4d
1a9b596 HEAD@{8}: rebase (finish): returning to refs/heads/main
1a9b596 HEAD@{9}: rebase: fast-forward        
c0ab087 HEAD@{10}: rebase: fast-forward       
4e87208 HEAD@{11}: rebase (start): checkout 4e872084529beb606480aefd8e29464c480abd8f        
1767593 HEAD@{12}: commit: Unwanted commit    
1a9b596 HEAD@{13}: rebase (finish): returning to refs/heads/main
1a9b596 HEAD@{14}: rebase (squash): Create Third File and Fourth File
2c42382 HEAD@{15}: rebase: fast-forward       
:
```

## Part 2:**Branching Basics (10 Challenges)**

```jsx
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git switch -c ft/new-feature
Switched to a new branch 'ft/new-feature'  
```

```jsx
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (ft/new-feature)
$ vi feature.txt

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (ft/new-feature)
$ git add feature.txt 
warning: in the working copy of 'feature.txt', LF will be replaced by CRLF the next time Git touches it

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (ft/new-feature)
$ git commit -m"Implemented core functionality for new feature"
[ft/new-feature 121324b] Implemented core functionality for new feature
 1 file changed, 1 insertion(+)
 create mode 100644 feature.txt
```

```jsx
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ vi readme.txt

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git add readme.txt 
warning: in the working copy of 'readme.txt', LF will be replaced by CRLF the next time Git touches it

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git commit -m"Updated project readme"
[main d766601] Updated project readme
 1 file changed, 2 insertions(+)
 create mode 100644 readme.txt
```

```jsx
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git push
Enumerating objects: 11, done.
Counting objects: 100% (11/11), done.
Delta compression using up to 8 threads       
Compressing objects: 100% (8/8), done.        
Writing objects: 100% (11/11), 967 bytes | 241.00 KiB/s, done.
Total 11 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), done.   
To https://github.com/Larissanoella-05/Advanced-git.git
 * [new branch]      main -> main

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git switch ft/new-feature 
Switched to branch 'ft/new-feature'

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (ft/new-feature)
$ git push
fatal: The current branch ft/new-feature has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/new-feature

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (ft/new-feature)
$ git push --set-upstream origin ft/new-feature
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads       
Compressing objects: 100% (2/2), done.        
Writing objects: 100% (3/3), 312 bytes | 312.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/new-feature' on GitHub by visiting:
remote:      https://github.com/Larissanoella-05/Advanced-git/pull/new/ft/new-feature       
remote:
To https://github.com/Larissanoella-05/Advanced-git.git
 * [new branch]      ft/new-feature -> ft/new-feature
branch 'ft/new-feature' set up to track 'origin/ft/new-feature'.

```

```jsx
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (ft/new-feature)
$ git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'. 

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git pull
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.   
remote: Compressing objects: 100% (2/2), done 
remote: Total 2 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (2/2), 1007 bytes | 167.00 KiB/s, done.
From https://github.com/Larissanoella-05/Advanced-git
   d766601..ca5a231  main       -> origin/main
Updating d766601..ca5a231
Fast-forward
 feature.txt | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 feature.txt

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git branch -d ft/new-feature 
Deleted branch ft/new-feature (was 121324b).
```

```jsx
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git checkout -b ft/new-branch-from-commit HEAD~3
Switched to a new branch 'ft/new-branch-from-commit'
```

```jsx
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (ft/new-branch-from-commit)  
$ git switch main 
Switched to branch 'main'
Your branch is up to date with 'origin/main'. 

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git merge ft/new-branch-from-commit 
Already up to date.
```

```jsx
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)

$ git rebase ft/new-branch-from-commit
Successfully rebased and updated refs/heads/main.

```

```jsx

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git branch -m ft/new-branch-from-commit ft/improved-branch-name

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git adog
* 501184b (HEAD -> main) Implemented core functionality for new feature
| * ca5a231 (origin/main, origin/HEAD) Merge pull request #1 from Larissanoella-05/ft/new-feature
|/|
| * 121324b (origin/ft/new-feature) Implemented core functionality for new feature
* | d766601 Updated project readme
|/
* 9b8ce66 Implemented test 5
| * b24ffe9 (ft/branch) Implemented test 5
|/
* fb5fdd4 (ft/improved-branch-name) chore: Create initial file       
* 97d1ca2 Create Third File and  Fourth File
```

```jsx
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git checkout 9b8ce66
Note: switching to '9b8ce66'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.  

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:   

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 9b8ce66 Implemented test 5
```

## Part 3

```jsx
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git pull --rebase
dropping 501184b006c62cb862e825cd7431d1bedb92ac31 Implemented core functionality for new feature -- patch contents already upstream
Successfully rebased and updated refs/heads/main.   

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git stash
No local changes to save

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git add test6.md 

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git stash
Saved working directory and index state WIP on main: ca5a231 Merge pull request #1 from Larissanoella-05/ft/new-feature
```

```jsx
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git stash pop
On branch main
Your branch is up to date with 'origin/main'.       

Changes to be committed:
  (use "git restore --staged <file>..." to unstage) 
        new file:   test6.md

Dropped refs/stash@{0} (83275e4fa9de5c52fde6876b6ecb090390b5df26)
```

```jsx
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git switch -c ft/merge-conflicts
Switched to a new branch 'ft/merge-conflicts'

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (ft/merge-conflicts)
$ ls
feature.txt  test1.md  test3.md  test5.md
readme.txt   test2.md  test4.md  test6.md

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (ft/merge-conflicts)
$ git add test5.md 

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (ft/merge-conflicts)
$ git commit -m" changed test5 to merge conflicts"
[ft/merge-conflicts e422685]  changed test5 to merge conflicts
 2 files changed, 2 insertions(+), 1 deletion(-)    
 create mode 100644 test6.md

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (ft/merge-conflicts)
$ git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.       

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git add test5.md 

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
vanced-git (main)
$ git commit -m" changed test5 to main"
[main d53d01c]  changed test5 to main
 1 file changed, 1 insertion(+), 1 deletion(-)      

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git merge ft/merge-conflicts
Auto-merging test5.md
CONFLICT (content): Merge conflict in test5.md      
 1 file changed, 1 insertion(+), 1 deletion(-)      

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git merge ft/merge-conflicts
Auto-merging test5.md
CONFLICT (content): Merge conflict in test5.md      

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git merge ft/merge-conflicts
Auto-merging test5.md
CONFLICT (content): Merge conflict in test5.md      
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git merge ft/merge-conflicts
Auto-merging test5.md
CONFLICT (content): Merge conflict in test5.md      
vanced-git (main)
$ git merge ft/merge-conflicts
Auto-merging test5.md
CONFLICT (content): Merge conflict in test5.md      
$ git merge ft/merge-conflicts
Auto-merging test5.md
CONFLICT (content): Merge conflict in test5.md      
Auto-merging test5.md
CONFLICT (content): Merge conflict in test5.md      
Automatic merge failed; fix conflicts and then commiCONFLICT (content): Merge conflict in test5.md      
Automatic merge failed; fix conflicts and then commiAutomatic merge failed; fix conflicts and then commit the result.
t the result.

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/AdPc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main|MERGING)
$ git push
Enumerating objects: 12, done.
Counting objects: 100% (12/12), done.
Delta compression using up to 8 threads
Compressing objects: 100% (7/7), done.
Writing objects: 100% (10/10), 868 bytes | 217.00 KiB/s, done.
Total 10 (delta 4), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (4/4), completed with 1 local object.
To https://github.com/Larissanoella-05/Advanced-git.git
   ca5a231..2ddb087  main -> main
```

```jsx
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git mergetool

This message is displayed because 'merge.tool' is not configured.
See 'git mergetool --tool-help' or 'git help config' for more details.
'git mergetool' will now attempt to use one of the following tools:
opendiff kdiff3 tkdiff xxdiff meld tortoisemerge gvimdiff diffuse diffmerge ecmerge p4merge araxis bc codecompare smerge emerge vimdiff nvimdiff
No files need merging

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git config --global merge.tool vscode

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git config --global mergetool.vscode.cmd "code --wait $MERGED"

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git mergetool
No files need merging
```

```jsx
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git checkout 9b8ce66
Note: switching to '9b8ce66'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 9b8ce66 Implemented test 5

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git ((9b8ce66...))
$ git switch -
Previous HEAD position was 9b8ce66 Implemented test 5
Switched to branch 'main'
Your branch is up to date with 'origin/main'. 
```

```jsx
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git add .gitignore 

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git commit -m"Created gitignore"
[main 575f97c] Created gitignore
 1 file changed, 0 insertions(+), 0 deletions(-)    
 create mode 100644 .gitignore

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ ls
feature.txt  test1.md  test3.md  test5.md
readme.txt   test2.md  test4.md  test6.md

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ ls -a
./     .gitignore   test1.md  test4.md
../    feature.txt  test2.md  test5.md
.git/  readme.txt   test3.md  test6.md

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.  
  (use "git push" to publish your local commits)    

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   .gitignore

no changes added to commit (use "git add" and/or "git commit -a")

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git commit -m"added tmp in gitignore"
On branch main
Your branch is ahead of 'origin/main' by 1 commit.  
  (use "git push" to publish your local commits)    

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   .gitignore

no changes added to commit (use "git add" and/or "git commit -a")

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.  
  (use "git push" to publish your local commits)    

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   .gitignore

no changes added to commit (use "git add" and/or "git commit -a")

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git add .gitignore 

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git commit -m"added tmp in gitignore"
[main 8061a96] added tmp in gitignore
 1 file changed, 1 insertion(+)

```

```jsx
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git tag v1.0

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git adog
* 8061a96 (HEAD -> main, tag: v1.0) added tmp in gitignore
* 575f97c Created gitignore
*   2ddb087 (origin/main, origin/HEAD) Merge branch 'ft/merge-conflicts'
|\  
| * e422685 (ft/merge-conflicts)  changed test5 to merge conflicts
* | d53d01c  changed test5 to main
|/  
*   ca5a231 Merge pull request #1 from Larissanoella-05/ft/new-feature
|\
| * 121324b (origin/ft/new-feature) Implemented core
 functionality for new feature
* | d766601 Updated project readme
|/
* 9b8ce66 Implemented test 5
| * b24ffe9 (ft/branch) Implemented test 5
|/
* fb5fdd4 (ft/improved-branch-name) chore: Create initial file
* 97d1ca2 Create Third File and  Fourth File        

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git push
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 504 bytes | 168.00 KiB/s, done.
Total 5 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
To https://github.com/Larissanoella-05/Advanced-git.git
   2ddb087..8061a96  main -> main

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.       

nothing to commit, working tree clean

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git push origin v1.0
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Larissanoella-05/Advanced-git.git
 * [new tag]         v1.0 -> v1.0

```

```jsx
Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git tag
v1.0

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git tag -d <v1.0>
bash: syntax error near unexpected token `newline'  

Pc@DESKTOP-97PM30V MINGW64 ~/Desktop/Advanced-git/Advanced-git (main)
$ git tag -d v1.0
Deleted tag 'v1.0' (was 8061a96)
```

