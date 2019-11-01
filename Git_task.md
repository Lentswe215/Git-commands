---Your initial commit---

1. lentswe@lentswe-HP-250-G3-Notebook-PC:~$ mkdir git-basic-exercises
2. lentswe@lentswe-HP-250-G3-Notebook-PC:~$ cd git-basic-exercises
3. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ ls -a
.  ..
4. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git init
Initialized empty Git repository in /home/lentswe/git-basic-exercises/.git/
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ ls -a
.  ..  .git
5. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git status
On branch master

No commits yet   

nothing to commit (create/copy files and use "git add" to track)
6. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ touch README.md
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ ls -a
.  ..  .git  README.md
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	README.md

nothing added to commit but untracked files present (use "git add" to track)

7. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git log
fatal: your current branch 'master' does not have any commits yet
8. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git add README.md
9. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   README.md
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-baxercises$

10. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git reset README.md
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	README.md

nothing added to commit but untracked files present (use "git add" to track)

11. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git add README.md
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git commit -m "initial commit"
[master (root-commit) a074d99] initial commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 README.md

12. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git log
commit a074d996fca348eb7db9acf813094c2b2912e8d7 (HEAD -> master)
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Tue Oct 29 13:32:46 2019 +0200

    initial commit
________________________________________________________________________________________________________________________________________________
---More commits---
1. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ nano README.md
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ cat README.md
We are live from Jeppestown, Johannbesburg
4. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git add README.md
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git commit -m "second commit"
[master 07344f3] second commit
 1 file changed, 1 insertion(+)
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git log
commit 07344f3afa01c9e2614e9ee26f308f15b053855b (HEAD -> master)
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Tue Oct 29 14:55:23 2019 +0200

    second commit

commit cdacc2c67204888ab48e1b8374df6839e1ab31bf
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Tue Oct 29 14:52:41 2019 +0200

    initial commit
5. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git commit -m "third commit"
[master b82f61f] third commit
 1 file changed, 1 insertion(+)
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git log
commit b82f61f20405939d9571a513847eb1723bc5ec0b (HEAD -> master)
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Tue Oct 29 14:57:23 2019 +0200

    third commit

commit 07344f3afa01c9e2614e9ee26f308f15b053855b
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Tue Oct 29 14:55:23 2019 +0200

    second commit

commit cdacc2c67204888ab48e1b8374df6839e1ab31bf
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Tue Oct 29 14:52:41 2019 +0200

    initial commit
________________________________________________________________________________________________________________________________________________
---Check this out---

3.  lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git checkout 07344f3afa01c9e2614e9ee26f308f15b053855b
Note: checking out '07344f3afa01c9e2614e9ee26f308f15b053855b'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by performing another checkout.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -b with the checkout command again. Example:

  git checkout -b <new-branch-name>

HEAD is now at 07344f3 second commit

4. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ cat README.md
We are at Umuzi doing the thing that makes the pots not be done
5.  lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git checkout master
Switched to branch 'master'
6. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ cat README.md
We are at Umuzi doing the thing that makes the pots not be done
Coding is the one i love
________________________________________________________________________________________________________________________________________________

---Branching---

1. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git branch
* master
2. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git branch milkshake-flavours
3. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git branch
* master
  milkshake-flavours
4. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git checkout milkshake-flavours
Switched to branch 'milkshake-flavours'
5. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ nano milkshakes.md
6. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git status
On branch milkshake-flavours
Untracked files:
  (use "git add <file>..." to include in what will be committed)

	milkshakes.md

nothing added to commit but untracked files present (use "git add" to track)
7. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git add milkshakes.md
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git commit -m "added initial flavours"
[milkshake-flavours ca614ad] added initial flavours
 1 file changed, 4 insertions(+)
 create mode 100644 milkshakes.md
8. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git log
commit ca614ad9d61d39b82a3965690ec0eb5ff153dd30 (HEAD -> milkshake-flavours)
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:59:14 2019 +0200

    added initial flavours

commit 35eb3d5824ecbd5b610c906b4870fe29f11cfcaa (master)
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:54:47 2019 +0200

    third commit

commit bd7ea682a8ab037dc0df8176e3c9d916780bdeaa
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:53:41 2019 +0200

    second commit

commit dc7ca1a095d20c045219fe861d5911d03f2fbaad
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:51:30 2019 +0200

    initial commit
9. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git checkout masterSwitched to branch 'master'
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git log
commit 35eb3d5824ecbd5b610c906b4870fe29f11cfcaa (HEAD -> master)
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:54:47 2019 +0200

    third commit

commit bd7ea682a8ab037dc0df8176e3c9d916780bdeaa
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:53:41 2019 +0200

    second commit

commit dc7ca1a095d20c045219fe861d5911d03f2fbaad
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:51:30 2019 +0200

    initial commit
10. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git branch history
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git checkout history
Switched to branch 'history'
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git log
commit 35eb3d5824ecbd5b610c906b4870fe29f11cfcaa (HEAD -> history, master)
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:54:47 2019 +0200

    third commit

commit bd7ea682a8ab037dc0df8176e3c9d916780bdeaa
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:53:41 2019 +0200

    second commit

commit dc7ca1a095d20c045219fe861d5911d03f2fbaad
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:51:30 2019 +0200

    initial commit
11. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ history > history.txt
12. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git add history.txtlentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git commit -m "added history"
[history 4460013] added history
 1 file changed, 688 insertions(+)
 create mode 100644 history.txt
13. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git checkout milkshake-flavours
Switched to branch 'milkshake-flavours'
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git log
commit ca614ad9d61d39b82a3965690ec0eb5ff153dd30 (HEAD -> milkshake-flavours)
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:59:14 2019 +0200

    added initial flavours

commit 35eb3d5824ecbd5b610c906b4870fe29f11cfcaa (master)
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:54:47 2019 +0200

    third commit

commit bd7ea682a8ab037dc0df8176e3c9d916780bdeaa
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:53:41 2019 +0200

    second commit

commit dc7ca1a095d20c045219fe861d5911d03f2fbaad
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:51:30 2019 +0200

    initial commit
14. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ nano README.md
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git add README.md
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git commit -m "random readme changes"
[milkshake-flavours ab6b0ba] random readme changes
 1 file changed, 1 insertion(+)
15. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git checkout history
Switched to branch 'history'
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ cat README.md
We are at Umuzi doing the thing that makes the pots not be done
Coding is the one i love
16. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ rm README.md
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ echo "booya" > README.md
17. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git add README.md
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git cfommit -m "rewrote readme"
git: 'cfommit' is not a git command. See 'git --help'.

The most similar command is
	commit
18. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git checkout master
Switched to branch 'master'
________________________________________________________________________________________________________________________________________________

---Just make sure we are still on track---

1. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git checkout master
Switched to branch 'master'
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ ls
README.md
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git log
commit 167b07348670f082f49e6771f52c85e22204fb57
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Fri Nov 1 12:07:02 2019 +0200

    third commit

commit 0be749140fab141cd7191c84a5550a583e7fdd07
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Fri Nov 1 12:06:24 2019 +0200

    second commit

commit 669f9d3ef44cb8289b3e6e55de044bf04dd05450
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Fri Nov 1 12:05:36 2019 +0200

    initial commit

2. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git checkout milkshake-flavours
Switched to branch 'milkshake-flavours'
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ ls
milkshakes.md  README.md
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git log
commit 914e55c7b8b87f21647b1ba50b2606d5c40cb4c9 (HEAD -> milkshake-flavours)
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Fri Nov 1 12:11:38 2019 +0200

    added initial flavours

commit 167b07348670f082f49e6771f52c85e22204fb57
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Fri Nov 1 12:07:02 2019 +0200

    third commit

commit 0be749140fab141cd7191c84a5550a583e7fdd07
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Fri Nov 1 12:06:24 2019 +0200

    second commit

commit 669f9d3ef44cb8289b3e6e55de044bf04dd05450
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Fri Nov 1 12:05:36 2019 +0200

    initial commit

3. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git checkout history
Switched to branch 'history'
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ ls
history.txt  README.md
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git log
commit d25933ccae5d8856c0be819a4b8ab400889e8377 (HEAD -> history)
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Fri Nov 1 12:15:39 2019 +0200

    rewrote readme

commit f4726d12715c4ca958dc6a1ad004f0913622e4c9
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Fri Nov 1 12:09:17 2019 +0200

    added initial flavours

commit 167b07348670f082f49e6771f52c85e22204fb57
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Fri Nov 1 12:07:02 2019 +0200

    third commit

commit 0be749140fab141cd7191c84a5550a583e7fdd07
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Fri Nov 1 12:06:24 2019 +0200

    second commit

commit 669f9d3ef44cb8289b3e6e55de044bf04dd05450
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Fri Nov 1 12:05:36 2019 +0200

    initial commit
________________________________________________________________________________________________________________________________________________

---Merging---

1.lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ merge  

2. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ ls
milkshakes.md  README.md
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git log
commit ab6b0baf55b12b1000a63d74e71cc0abe5342181 (HEAD -> master, milkshake-flavours)
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 09:27:33 2019 +0200

    random readme changes

commit ca614ad9d61d39b82a3965690ec0eb5ff153dd30
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:59:14 2019 +0200

    added initial flavours

commit 35eb3d5824ecbd5b610c906b4870fe29f11cfcaa
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:54:47 2019 +0200

    third commit

commit bd7ea682a8ab037dc0df8176e3c9d916780bdeaa
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:53:41 2019 +0200

    second commit

commit dc7ca1a095d20c045219fe861d5911d03f2fbaad
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:51:30 2019 +0200

    initial commit

3. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git merge history
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
Automatic merge failed; fix conflicts and then commit the result.
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ ls
history.txt  milkshakes.md  README.md
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git log
commit ab6b0baf55b12b1000a63d74e71cc0abe5342181 (HEAD -> master, milkshake-flavours)
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 09:27:33 2019 +0200

    random readme changes

commit ca614ad9d61d39b82a3965690ec0eb5ff153dd30
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:59:14 2019 +0200

    added initial flavours

commit 35eb3d5824ecbd5b610c906b4870fe29f11cfcaa
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:54:47 2019 +0200

    third commit

commit bd7ea682a8ab037dc0df8176e3c9d916780bdeaa
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:53:41 2019 +0200

    second commit

commit dc7ca1a095d20c045219fe861d5911d03f2fbaad
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:51:30 2019 +0200

    initial commit
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git status
On branch master
You have unmerged paths.
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

Changes to be committed:

	new file:   history.txt

Unmerged paths:
  (use "git add <file>..." to mark resolution)

	both modified:   README.md

lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git add README.md
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git status
On branch master
All conflicts fixed but you are still merging.
  (use "git commit" to conclude merge)

Changes to be committed:

	modified:   README.md
	new file:   history.txt

lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git commit -m "Resolved merge conflict."
[master 51b0d76] Resolved merge conflict by incoporating both suggestions.
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git merge history
Already up to date.
4. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ ls 
history.txt  milkshakes.md  README.md
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git log
commit 51b0d76e06ca084ccf60fdf1f9a07a62ad1293cf (HEAD -> master)
Merge: ab6b0ba 4b3aafb
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 12:05:46 2019 +0200

    Resolved merge conflict.

commit 4b3aafbca7cd06b52970fd7ea42fed33ec30d7e4 (history)
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 09:44:27 2019 +0200

    rewrote readme

commit ab6b0baf55b12b1000a63d74e71cc0abe5342181 (milkshake-flavours)
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 09:27:33 2019 +0200

    random readme changes

commit 4460013d6210181bd95ee2a8472511d41f53dcba
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 09:16:36 2019 +0200

    added history

commit ca614ad9d61d39b82a3965690ec0eb5ff153dd30
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:59:14 2019 +0200

    added initial flavours

commit 35eb3d5824ecbd5b610c906b4870fe29f11cfcaa
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:54:47 2019 +0200

    third commit

commit bd7ea682a8ab037dc0df8176e3c9d916780bdeaa
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:53:41 2019 +0200

    second commit

commit dc7ca1a095d20c045219fe861d5911d03f2fbaad
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:51:30 2019 +0200

    initial commit
5. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git checkout history
Switched to branch 'history'
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git log
commit 4b3aafbca7cd06b52970fd7ea42fed33ec30d7e4 (HEAD -> history)
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 09:44:27 2019 +0200

    rewrote readme

commit 4460013d6210181bd95ee2a8472511d41f53dcba
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 09:16:36 2019 +0200

    added history

commit 35eb3d5824ecbd5b610c906b4870fe29f11cfcaa
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:54:47 2019 +0200

    third commit

commit bd7ea682a8ab037dc0df8176e3c9d916780bdeaa
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:53:41 2019 +0200

    second commit

commit dc7ca1a095d20c045219fe861d5911d03f2fbaad
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:51:30 2019 +0200

    initial commit
________________________________________________________________________________________________________________________________________________

---Pulling and remotes---

1. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ cd ../
5. lentswe@lentswe-HP-250-G3-Notebook-PC:~$ git clone https://github.com/Umuzi-org/tech-department.git
Cloning into 'tech-department'...
remote: Enumerating objects: 934, done.
remote: Counting objects: 100% (934/934), done.
remote: Compressing objects: 100% (528/528), done.
remote: Total 26250 (delta 467), reused 821 (delta 384), pack-reused 25316
Receiving objects: 100% (26250/26250), 26.31 MiB | 180.00 KiB/s, done.
Resolving deltas: 100% (13874/13874), done.
6. lentswe@lentswe-HP-250-G3-Notebook-PC:~$ cd tech-department
7. lentswe@lentswe-HP-250-G3-Notebook-PC:~/tech-department$ git branch
* master
lentswe@lentswe-HP-250-G3-Notebook-PC:~/tech-department$ git log
commit 21769f6b4852e45f0d87716ce347fee271d93d74 (HEAD -> master, origin/master, origin/HEAD)
Author: Ryan O'Connell <ryan@oconnell.org.za>
Date:   Thu Oct 31 10:54:02 2019 +0200

    deploy

commit ff1ebfc354a379ab5d91a001e20229a886a1c9aa
Merge: eb1695e9 fe89c8e8
Author: sheenarbw <sheena.oconnell@gmail.com>
Date:   Wed Oct 30 05:26:02 2019 +0200

    Merge pull request #115 from Umuzi-org/update/clean_code_directory
    
    changed clean code directory and edited week by week syllabus

commit fe89c8e87eddfb3501bfdddf75111556e7a2de74 (origin/update/clean_code_directory)
Author: Ryan O'Connell <ryan@oconnell.org.za>
Date:   Tue Oct 29 12:10:53 2019 +0200

    changed clean code directory and edited week by week syllabus 
8. lentswe@lentswe-HP-250-G3-Notebook-PC:~/tech-department$ git branch -a
* master
  remotes/origin/Big_O
  remotes/origin/HEAD -> origin/master
  remotes/origin/SQL_updates
  remotes/origin/add-topic-dotenv
  remotes/origin/coding_horrors_TDD_pitfalls
  remotes/origin/create/agile_and_scrum_topic
  remotes/origin/create/expressjs-exercise
  remotes/origin/create/team_onboarding
  remotes/origin/data_ethics_workshop
  remotes/origin/data_science_namechange
  remotes/origin/data_validation_python
  remotes/origin/database_intro
  remotes/origin/dataviz
  remotes/origin/delete_this_branch
  remotes/origin/dibwe_suggestions
  remotes/origin/ds_unit_tests
  remotes/origin/ethics-workshop
  remotes/origin/feat/find
  remotes/origin/feat/refactor-and-add-in-extra-resources
  remotes/origin/find-command
  remotes/origin/fix/data-specific_topics_to_projects
  remotes/origin/fix/ds-formatting-and-links
9. lentswe@lentswe-HP-250-G3-Notebook-PC:~/tech-department$ git checkout -b project/git-basic-exercises
Switched to a new branch 'project/git-basic-exercises'
10. lentswe@lentswe-HP-250-G3-Notebook-PC:~/tech-department$ git remote -v
origin	https://github.com/Umuzi-org/tech-department.git (fetch)
origin	https://github.com/Umuzi-org/tech-department.git (push)
_________________________________________________________________________________________________________________________________________________

---Multiple Repos---
1. lentswe@lentswe-HP-250-G3-Notebook-PC:~/tech-department$ git log
commit 21769f6b4852e45f0d87716ce347fee271d93d74 (HEAD -> project/git-basic-exercises, origin/master, origin/HEAD, master)
Author: Ryan O'Connell <ryan@oconnell.org.za>
Date:   Thu Oct 31 10:54:02 2019 +0200

    deploy

commit ff1ebfc354a379ab5d91a001e20229a886a1c9aa
Merge: eb1695e9 fe89c8e8
Author: sheenarbw <sheena.oconnell@gmail.com>
Date:   Wed Oct 30 05:26:02 2019 +0200
commit 21769f6b4852e45f0d87716ce347fee271d93d74 (HEAD -> project/git-basic-exerc
ises, origin/master, origin/HEAD, master)
Author: Ryan O'Connell <ryan@oconnell.org.za>
Date:   Thu Oct 31 10:54:02 2019 +0200

    deploy

commit ff1ebfc354a379ab5d91a001e20229a886a1c9aa
Merge: eb1695e9 fe89c8e8
Author: sheenarbw <sheena.oconnell@gmail.com>
Date:   Wed Oct 30 05:26:02 2019 +0200

    Merge pull request #115 from Umuzi-org/update/clean_code_directory
    
    changed clean code directory and edited week by week syllabus

commit fe89c8e87eddfb3501bfdddf75111556e7a2de74 (origin/update/clean_code_directory)
Author: Ryan O'Connell <ryan@oconnell.org.za>
Date:   Tue Oct 29 12:10:53 2019 +0200

    changed clean code directory and edited week by week syllabus

commit eb1695e931b47201fa80ed0f74ba499efa7c28d3
Merge: c93e4995 1578c83e
Author: sheenarbw <sheena.oconnell@gmail.com>
Date:   Sat Oct 26 08:13:47 2019 +0200

    Merge pull request #89 from Umuzi-org/update/git_for_teamwork
2. lentswe@lentswe-HP-250-G3-Notebook-PC:~/tech-department$ cd ../git-basic-exercises
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git log
commit 51b0d76e06ca084ccf60fdf1f9a07a62ad1293cf (HEAD -> master, origin/master, origin/history, history)
Merge: ab6b0ba 4b3aafb
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 12:05:46 2019 +0200

    Resolved merge conflict by incoporating both suggestions.

commit 4b3aafbca7cd06b52970fd7ea42fed33ec30d7e4
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 09:44:27 2019 +0200

    rewrote readme

commit ab6b0baf55b12b1000a63d74e71cc0abe5342181 (origin/milkshake-flavours, milkshake-flavours)
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 09:27:33 2019 +0200

    random readme changes

commit 4460013d6210181bd95ee2a8472511d41f53dcba
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 09:16:36 2019 +0200

    added history

commit ca614ad9d61d39b82a3965690ec0eb5ff153dd30
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:59:14 2019 +0200

    added initial flavours

commit 35eb3d5824ecbd5b610c906b4870fe29f11cfcaa
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:54:47 2019 +0200

    third commit

commit bd7ea682a8ab037dc0df8176e3c9d916780bdeaa
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:53:41 2019 +0200

    second commit

commit dc7ca1a095d20c045219fe861d5911d03f2fbaad
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:51:30 2019 +0200

    initial commit
3.  lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ cd
     lentswe@lentswe-HP-250-G3-Notebook-PC:~$ mkdir this-will-be-another-repo

4. lentswe@lentswe-HP-250-G3-Notebook-PC:~$ cd this-will-be-another-repo
lentswe@lentswe-HP-250-G3-Notebook-PC:~/this-will-be-another-repo$ git init
Initialized empty Git repository in /home/lentswe/this-will-be-another-repo/.git/
5. lentswe@lentswe-HP-250-G3-Notebook-PC:~/this-will-be-another-repo$ touch README.md
lentswe@lentswe-HP-250-G3-Notebook-PC:~/this-will-be-another-repo$ git add README.md
lentswe@lentswe-HP-250-G3-Notebook-PC:~/this-will-be-another-repo$ git commit -m "initial commit"
[master (root-commit) 56a1afc] initial commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 README.md
6. lentswe@lentswe-HP-250-G3-Notebook-PC:~/this-will-be-another-repo$ cd ../git-basic-exercises
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git log
commit 51b0d76e06ca084ccf60fdf1f9a07a62ad1293cf (HEAD -> master, origin/master, origin/history, history)
Merge: ab6b0ba 4b3aafb
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 12:05:46 2019 +0200

    Resolved merge conflict.

commit 4b3aafbca7cd06b52970fd7ea42fed33ec30d7e4
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 09:44:27 2019 +0200

    rewrote readme

commit ab6b0baf55b12b1000a63d74e71cc0abe5342181 (origin/milkshake-flavours, milkshake-flavours)
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 09:27:33 2019 +0200

    random readme changes

commit 4460013d6210181bd95ee2a8472511d41f53dcba
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 09:16:36 2019 +0200

    added history

commit ca614ad9d61d39b82a3965690ec0eb5ff153dd30
Author: Lentswe Mamonong <ephraimmamonong@gmail.com>
Date:   Thu Oct 31 08:59:14 2019 +0200

    added initial flavours
________________________________________________________________________________________________________________________________________________--

---gitignore---

1. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ touch ignore-me.db
2. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	ignore-me.db

nothing added to commit but untracked files present (use "git add" to track)
3. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ nano .gitignore
5. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	.gitignore

nothing added to commit but untracked files present (use "git add" to track)
6. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ mkdir large-directory-that-should-be-local-only
7. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ cd large-directory-that-should-be-local-only/
lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises/large-directory-that-should-be-local-only$ nano README.md
8.  lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises/large-directory-that-should-be-local-only$ cd ..
9. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ nano .gitignore
10. lentswe@lentswe-HP-250-G3-Notebook-PC:~/git-basic-exercises$ git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	.gitignore

nothing added to commit but untracked files present (use "git add" to track)

