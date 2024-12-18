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