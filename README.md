# Gym-Git-Exercise-Solutions

## Exercise 1

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

## Exercise 3

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git branch -m main  
```

## Exercise 4

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git add . 
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git commit -m "Initial Commit"
[main f6305a9] Initial Commit
 2 files changed, 39 insertions(+), 1 deletion(-)
 create mode 100644 index.html
```

## Exercise 5

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git remote add origin https://github.com/alain-michael/Gym-Git-Exercise-Solutions.git    
```

## Exercise 6

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

## Exercise 7

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git branch dev
```

## Exercise 8

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git branch test dev
```

## Exercise 9

```powershell
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git switch dev
Switched to branch 'dev'
M       README.md
PS C:\Users\mbric\Documents\Sook\Gym-Git-Exercise-Solutions> git branch -d test
Deleted branch test (was f6305a9).
```