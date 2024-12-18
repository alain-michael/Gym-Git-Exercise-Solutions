# Gym-Git-Exercise-Solutions

## Bundle 1

## Exercise 1

### Task 1


```powershell
PS C:\Users\mbric\Documents\Sook> mkdir Gym-Git-Exercise-Solutions
   

Directory: C:\Users\mbric\Documents\Sook


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        12/16/2024     12:53                Gym-Git-Exercise-Solutions


PS C:\Users\mbric\Documents\Sook> cd .\Gym-Git-Exercise-Solutions\
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> ls
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git init
```

### Task 3

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git branch -m main  
```

### Task 4

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git add . 
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git commit -m "Initial Commit"
[main f6305a9] Initial Commit
 2 files changed, 39 insertions(+), 1 deletion(-)
 create mode 100644 index.html
```

### Task 5

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git remote add origin https://github.com/alain-michael/Gym-Git-Exercise-Solutions.git    
```

### Task 6

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git push
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 676 bytes | 338.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/alain-michael/Gym-Git-Exercise-Solutions.git
   52914fd..f6305a9  main -> main
branch 'main' set up to track 'origin/main'.
```

### Task 7

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git branch dev
```

### Task 8

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git branch test dev
```

### Task 9

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git switch dev
Switched to branch 'dev'
M       README.md
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git branch -d test
Deleted branch test (was f6305a9).
```

## Exercise 2

### Task 1

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git stash -u
Saved working directory and index state WIP on dev: 0a40e6e Added terminal logs to README.md
```

### Task 2

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git stash -u
Saved working directory and index state WIP on dev: 0a40e6e Added terminal logs to README.md
```

### Task 3

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git stash -u
Saved working directory and index state WIP on dev: 0a40e6e Added terminal logs to README.md
```

### Task 4

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git stash pop "stash@{1}"
```

### Task 5

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git stash pop "stash@{2}"
```
### Task 6

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git stash pop "stash@{3}"
```
### Task 7

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git add .
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git commit -m "Exercise 2"
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git push
```
### Task 8

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git reset --hard
HEAD is now at b20fb3a Step 6 of Git Exercises
```

## Bundle 2

## Exercise 1

### Task 1

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git checkout -b ft/bundle-2           
Switched to a new branch 'ft/bundle-2'
```

### Task 3

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git add services.html
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git commit -m "Task 3"
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git push origin ft/bundle-2
```

## Exercise 2

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git switch main
Switched to branch 'main'
Your branch is behind 'origin/main' by 6 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git pull
Updating f6305a9..236cc01
Fast-forward
 README.md     | 132 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++-
 about.html    |  11 +++++
 home.html     |  11 +++++
 services.html |  11 +++++
 team.html     |  11 +++++
 5 files changed, 174 insertions(+), 2 deletions(-)
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 services.html
 create mode 100644 team.html
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git branch ft/service-redesign               
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git switch ft/service-redesign
Switched to branch 'ft/service-redesign'
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git diff main
diff --git a/services.html b/services.html
index dbdabfe..39f691c 100644
--- a/services.html
+++ b/services.html
@@ -9,7 +9,7 @@
     <h1>Services Page</h1>
     <a href="index.html">Home</a>
     <a href="about.html">About</a>
-    <a href="team.html">Our Team</a>
-    <a href="services.html">Our Services</a>
+    <a href="team.html">Team</a>
+    <a href="services.html">Services</a>
   </body>
 </html>
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git merge
Already up to date.
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git merge main
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git add .
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git commit -m "Resolved merge conflicts"
[ft/service-redesign 4e93b0d] Resolved merge conflicts
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git push
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.
Writing objects: 100% (1/1), 224 bytes | 224.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/alain-michael/Gym-Git-Exercise-Solutions.git
   1dba6c6..4e93b0d  ft/service-redesign -> ft/service-redesign
```

## Bundle 3

### Exercise 1

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git switch -c ft/team-page
Switched to a new branch 'ft/team-page'
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git add team.html
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git commit -m "Changes to team.html"
[ft/team-page 8c82fb4] Changes to team.html
 1 file changed, 5 insertions(+), 1 deletion(-)
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 468 bytes | 156.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/alain-michael/Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote:
To https://github.com/alain-michael/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git switch main
Switched to branch 'main'
Your branch is behind 'origin/main' by 4 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git branch ft/contact-page
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git switch ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git log
commit 8c82fb409b16a57fd732abeb0a802a724d4bf09c (HEAD -> ft/team-page, origin/ft/team-page)
Author: amuhirwa <a.muhirwa@alustudent.com>
Date:   Wed Dec 18 10:32:33 2024 +0200

    Changes to team.html

commit 0ec0a8ecf7a9f97d3bb0c5c6ddc72b0c3361c9c9 (origin/ft/service-redesign, ft/service-redesign)
Author: amuhirwa <a.muhirwa@alustudent.com>
Date:   Wed Dec 18 10:30:24 2024 +0200

    Done with Bundle 2

commit 4e93b0d65e950ea7c8f321c2d9c5dd27683cb791
Merge: 1dba6c6 a730656
Author: amuhirwa <a.muhirwa@alustudent.com>
Date:   Wed Dec 18 08:20:23 2024 +0200
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git checkout ft/contact-page                            
Switched to branch 'ft/contact-page'
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git cherry-pick 8c82fb409b16a57fd732abeb0a802a724d4bf09c
[ft/contact-page 5c58529] Changes to team.html
 Date: Wed Dec 18 10:32:33 2024 +0200
 1 file changed, 5 insertions(+), 1 deletion(-)
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git add .
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git commit -m "New changes to the contact page" 
[ft/contact-page ae655b3] New changes to the contact page
 1 file changed, 11 insertions(+)
 create mode 100644 contact.html
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git push
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 906 bytes | 226.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/alain-michael/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote:
To https://github.com/alain-michael/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git switch -c ft/faq-page
Switched to a new branch 'ft/faq-page'
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git add .   
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git commit -m "Faq Page"
[ft/faq-page 9c4474f] Faq Page
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 417 bytes | 208.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/alain-michael/Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
remote:
To https://github.com/alain-michael/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git revert 8c82fb409b16a57fd732abeb0a802a724d4bf09c
[ft/faq-page a9aa36a] Revert "Changes to team.html"
 1 file changed, 1 insertion(+), 5 deletions(-)
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git add .
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git status             
On branch ft/faq-page
Your branch is ahead of 'origin/ft/faq-page' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 350 bytes | 116.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/alain-michael/Gym-Git-Exercise-Solutions.git
   9c4474f..a9aa36a  ft/faq-page -> ft/faq-page
```

### Exercise 2

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git branch ft/home-page-redesign ft/faq-page
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git switch main
Switched to branch 'main'
M       README.md
Your branch is behind 'origin/main' by 11 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git add .
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git commit -m "Changed team.html"
[main 1a64f36] Changed team.html
 2 files changed, 6 insertions(+), 1 deletion(-)
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git pull
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
Auto-merging team.html
CONFLICT (content): Merge conflict in team.html
Automatic merge failed; fix conflicts and then commit the result.
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git pull
error: Pulling is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git pull
error: You have not concluded your merge (MERGE_HEAD exists).
hint: Please, commit your changes before merging.
fatal: Exiting because of unfinished merge.
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git push
Enumerating objects: 11, done.
Counting objects: 100% (11/11), done.
Delta compression using up to 8 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 603 bytes | 301.00 KiB/s, done.
Total 5 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 3 local objects.
To https://github.com/alain-michael/Gym-Git-Exercise-Solutions.git
   542b878..facd142  main -> main
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git switch ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git rebase main
Successfully rebased and updated refs/heads/ft/home-page-redesign.
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git add .
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git commit -m "Added heading to home.html"
[ft/home-page-redesign 096effb] Added heading to home.html
 1 file changed, 1 insertion(+), 1 deletion(-)
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 333 bytes | 333.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/alain-michael/Gym-Git-Exercise-Solutions/pull/new/ft/home-page-redesign
remote:
To https://github.com/alain-michael/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.
```

## Bundle 4
### Exercise 1

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git checkout main
Switched to branch 'main'
Your branch is behind 'origin/main' by 3 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git remote add git-copy https://github.com/alain-michael/GIT-Copy.git
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git remote
git-copy
origin
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git pull
error: Your local changes to the following files would be overwritten by merge:
        home.html
Please commit your changes or stash them before you merge.
Aborting
Updating facd142..5fe678c
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git pull
Updating facd142..5fe678c
Fast-forward
 README.md | 184 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 home.html |   2 +-
 2 files changed, 185 insertions(+), 1 deletion(-)
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git add .
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git commit -m "Bundle 4 Exercise 1"
[main 920cd0b] Bundle 4 Exercise 1
 1 file changed, 13 insertions(+), 7 deletions(-)
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git push --all
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 582 bytes | 582.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/alain-michael/Gym-Git-Exercise-Solutions.git
   0a40e6e..b20fb3a  dev -> dev
   5fe678c..920cd0b  main -> main
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git push git-copy
Enumerating objects: 66, done.
Counting objects: 100% (66/66), done.
Delta compression using up to 8 threads
Compressing objects: 100% (64/64), done.
Writing objects: 100% (66/66), 14.32 KiB | 2.05 MiB/s, done.
Total 66 (delta 34), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (34/34), done.
To https://github.com/alain-michael/GIT-Copy.git
 * [new branch]      main -> main
```