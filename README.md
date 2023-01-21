# Git Commands Project :

# Steps & Screenshots :

1. Created Shopping Folder :

```
C:\Dev\Antwalk Training\Git Commands Project> mkdir Shopping
```
  
2. Initialised empty Git Repo using "**git init**" inside Shopping folder :

```
C:\Dev\Antwalk Training\Git Commands Project> cd Shopping
C:\Dev\Antwalk Training\Git Commands Project\Shopping> git init
```

3. Adding remote origin using "**git remote add origin**" after creating repo on GitHub :

```
C:\Dev\Antwalk Training\Git Commands Project\Shopping [main]> git remote add origin git@github.com:swairik/Git-Commands-Project.git
```

4. Created yard.txt & groceries.txt

```
C:\Dev\Antwalk Training\Git Commands Project\Shopping [main]> touch yard.txt groceries.txt
```

5. Committed empty files using "**git add .**" and "**git commit**" :

```
C:\Dev\Antwalk Training\Git Commands Project\Shopping [main +2 ~0-0 !]> git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        groceries.txt
        yard.txt
nothing added to commit but untracked files present (use "git add" to track)
C:\Dev\Antwalk Training\Git Commands Project\Shopping [main +2~0-0 !]> git add.
C:\Dev\Antwalk Training\Git Commands Project\Shopping [main +2 0-0 ~]> git commit -m "create yard and groceries lists" 
[main (root-commit) e291859] create yard and groceries lists
  2 files changed, 0 insertions(+), 0 deletions(-)
  create mode 100644 groceries.txt
  create mode 100644 yard.txt
C:\Dev\Antwalk Training\Git Commands Project\Shopping [main]> git log 
commit e2918591efcbd48bd0f9c1a111562cbb2bb19b58 (HEAD -> main)
Author: Swairik <swairikdey1001@gmail.com>
Date: Sun Jan 22 00:51:40 2023 +0530
    create yard and groceries lists
```

6. Added text to files :

```
C:\Dev\Antwalk Training\Git Commands Project\Shopping [main]> git status On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified: groceries.txt 
        modified: yard.txt
```

7. Committed groceries.txt file :

```
C:\Dev\Antwalk Training\Git Commands Project\Shopping [main +0 ~2 -0 !]> git add groceries.txt
C:\Dev\Antwalk Training\Git Commands Project\Shopping [main +0 ~1 -0 | +0 ~1 -0 !]> git commit -m "add ingredients for tomato soup"
[main 85bd431] add ingredients for tomato soup
 1 file changed, 3 insertions(+)
```

8. Committed yard.txt :

```
C:\Dev\Antwalk Training\Git Commands Project\Shopping [main +0 ~1 -0 !]> git add yard.txt
C:\Dev\Antwalk Training\Git Commands Project\Shopping [main +0 ~1 -0 ~]> git commit -m "add items needed for garden box"
[main 5bfaf71] add items needed for garden box
 1 file changed, 2 insertions(+)
```

9. Updated both files and committed them :

```
﻿
C:\Dev\Antwalk Training\Git Commands Project\Shopping [main]> git status On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory) 
        modified: groceries.txt
        modified: yard.txt
        
no changes added to commit (use "git add" and/or "git commit -a")
C:\Dev\Antwalk Training\Git Commands Project\Shopping [main +0 ~2-0 !]> git add.
C:\Dev\Antwalk Training Git Commands Project\Shopping [main +0~2-0 ~]> git commit -m "add items needed to grow potatoes"
[main dccbd83] add items needed to grow potatoes
 2 files changed, 2 insertions(+), 1 deletion(-)
```

10. Git log to show all commits :

```
C:\Dev\Antwalk Training\Git Commands Project\Shopping [main]> git log
commit dccbd83c3dee2edf2d20687b8aefa0d014b935cc (HEAD -> main)
Author: Swairik <swairikdey1001@gmail.com>
Date:   Sun Jan 22 00:58:22 2023 +0530

    add items needed to grow potatoes

commit 5bfaf7129bb473afacb681ab1061939639bb5e7d
Author: Swairik <swairikdey1001@gmail.com>
Date:   Sun Jan 22 00:56:16 2023 +0530

    add items needed for garden box

commit 85bd4314692ff64643929f806cafce535f20cdaa
Author: Swairik <swairikdey1001@gmail.com>
Date:   Sun Jan 22 00:54:46 2023 +0530
    add ingredients for tomato soup

commit e2918591efcbd48bd0f9c1a111562cbb2bb19b58
Author: Swairik <swairikdey1001@gmail.com>
Date:   Sun Jan 22 00:51:40 2023 +0530
```

11. Pushing to repo on GitHub using "**git push**" :

```
C:\Dev\Antwalk Training\Git Commands Project\Shopping [main]> git push -u origin main
Enumerating objects: 13, done.
Counting objects: 100% (13/13), done.
Delta compression using up to 8 threads
Compressing objects: 100% (11/11), done.
Writing objects: 100% (13/13), 1.19 KiB | 406.00 KiB/s, done.
Total 13 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:swairik/Git-Commands-Project.git
 * [new branch]      main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.
```
