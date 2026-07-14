# git basic Exercise
## bundle 1



## bundle2
### exercise1 
```
: 'branches' is not a git command. See 'git --help'.
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git branch
  dev
  main
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git commit -m "Added the service page"
 1 file changed, 11 insertions(+)
 create mode 100644 service.html
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git push origin ft/bundle-2
fatal: unable to access 'https://github.com/ngabo-112/Gym-Git-Exercise-Solutions/': Could not resolve host: github.comPS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git push origin ft/bundle-2
fatal: unable to access 'https://github.com/ngabo-112/Gym-Git-Exercise-Solutions/': Could not resolve host: github.comPS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git push origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 518 bytes | 518.00 KiB/s, done.
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/ngabo-112/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
To https://github.com/ngabo-112/Gym-Git-Exercise-Solutions
 * [new branch]      ft/bundle-2 -> ft/bundle-2
  dev
* ft/bundle-2
  main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git branch 
  dev
  ft/bundle-2
* main
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git pull origin main
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.

```
## bundle 3
### exercise 1
```
  dev
  ft/bundle-2
  ft/service-redesign
  main
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git add teams.html
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git commit -m "added the teams page"
[ft/team-page d840325] added the teams page
 1 file changed, 11 insertions(+)
 create mode 100644 teams.html
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git push origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 443 bytes | 221.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote: 
To https://github.com/ngabo-112/Gym-Git-Exercise-Solutions
 * [new branch]      ft/team-page -> ft/team-page
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git checkout main
Switched to branch 'main'
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git branch
  ft/bundle-2
  ft/team-page
* main
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git switch ft/team-page
Switched to branch 'ft/team-page'
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git log 
Author: ngabo-112 <ngabomiguel123@gmail.com>

    added the teams page

commit a8b3a2216ec39fea86bc66daf75c3a2f646f8008 (origin/main, origin/HEAD, main, ft/contact-page)
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git log --oneline -1
d840325 (HEAD -> ft/team-page, origin/ft/team-page) added the teams page
  dev
  ft/bundle-2
  ft/service-redesign
* ft/team-page
  main
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git switch ft/bundle-2
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git cherry-pick d840325
[ft/bundle-2 6a38a92] added the teams page
 create mode 100644 teams.html
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git add teams.html
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git commit -m "this is the heading "
 1 file changed, 1 insertion(+), 1 deletion(-)
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git commit --amend -m "asked me to make some changes"
[ft/bundle-2 efcc87e] asked me to make some changes
 Date: Tue Jul 14 07:01:04 2026 +0200
 1 file changed, 1 insertion(+), 1 deletion(-)
  dev
* ft/bundle-2
  ft/contact-page
  ft/service-redesign
  ft/team-page
  main
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git push origin ft/bundle-2
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 716 bytes | 179.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
   90242be..efcc87e  ft/bundle-2 -> ft/bundle-2
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git brancj
git: 'brancj' is not a git command. See 'git --help'.

The most similar command is
        branch
  dev
  ft/contact-page
  ft/service-redesign
  ft/team-page
  main
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git checkout ft/contact-page
Switched to branch 'ft/contact-page'
  dev
  ft/service-redesign
  ft/team-page
  main
Switched to a new branch 'ft/faq-page'
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git add faq.html
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git commit -m "added the faq.html"
[ft/faq-page 6bdfab1] added the faq.html
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git branch
  ft/bundle-2
  ft/contact-page
* ft/faq-page
  ft/service-redesign
  ft/team-page
  main
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git push origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 444 bytes | 222.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/ngabo-112/Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
remote: 
To https://github.com/ngabo-112/Gym-Git-Exercise-Solutions
 * [new branch]      ft/faq-page -> ft/faq-page
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git revert d840325
CONFLICT (rename/delete): teams.html renamed to faq.html in HEAD, but deleted in parent of d840325 (added the teams page).
CONFLICT (modify/delete): faq.html deleted in parent of d840325 (added the teams page) and modified in HEAD.  Version HEAD of faq.html left in tree.
error: could not revert d840325... added the teams page
hint: "git revert --continue".
hint: You can instead skip this commit with "git revert --skip".
hint: To abort and get back to the state before "git revert",
hint: run "git revert --abort".
hint: Disable this message with "git config set advice.mergeConflict false"
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git revert --abort
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git branch
  ft/bundle-2
* ft/faq-page
  ft/team-page
  main
git: 'ft/contact-page' is not a git command. See 'git --help'.
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git switch ft/contact-page
Switched to branch 'ft/contact-page'
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git revert d840325
On branch ft/contact-page
nothing to commit, working tree clean
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git branch 
  ft/bundle-2
* ft/contact-page
  ft/service-redesign
  ft/team-page
  main
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git revert d840325
On branch ft/contact-page
nothing to commit, working tree clean
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git branch
  ft/bundle-2
* ft/contact-page
  ft/faq-page
  ft/service-redesign
  main
git: 'loq' is not a git command. See 'git --help'.

The most similar command is
        log
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git log --online
fatal: unrecognized argument: --online
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git log --oneline
40807f1 added content on the main branch
f381bb8 Merge pull request #2 from ngabo-112/ft/bundle-2
90242be Added the service page
f7850cc Resolve merge conflict in README
329fdab  added the ReadMe.md
eb9d7b6 added about the index and team
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git branch   
* ft/contact-page
  ft/service-redesign
  ft/team-page
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> 
Switched to branch 'ft/faq-page'
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git status 
On branch ft/faq-page
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git switch ft/team-page
Switched to branch 'ft/team-page'
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git revert d840325
[ft/team-page e97a018] Revert "added the teams page"
 1 file changed, 11 deletions(-)
 delete mode 100644 teams.html
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> git push origin ft/team-page
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 252 bytes | 252.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/ngabo-112/Gym-Git-Exercise-Solutions
   d840325..e97a018  ft/team-page -> ft/team-page
PS C:\Users\USER\Documents\Gym-Git-Exercise-Solutions> 
```
### exercise 2 
```

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (ft/team-page)
$ git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/faq-page
  ft/service-redesign
* ft/team-page
  main

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (ft/team-page)
$ git checkout ft/faq-page
M       README.md
Switched to branch 'ft/faq-page'

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git switch main
M       README.md
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
$ git add .

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
$ git commit -m " changed the index.html"
[main 40482ad]  changed the index.html
 2 files changed, 190 insertions(+), 1 deletion(-)

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
$ git push origin main
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 2.21 KiB | 754.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/ngabo-112/Gym-Git-Exercise-Solutions
   a8b3a22..40482ad  main -> main

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
$ git branch 
  dev
  ft/bundle-2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
  ft/team-page

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
$ 

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
$ git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git rebase main
Successfully rebased and updated refs/heads/ft/home-page-redesign.

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git add .

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git commit -m "added a paragraph"
[ft/home-page-redesign 07e87a4] added a paragraph
 1 file changed, 1 insertion(+)

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git push origin ft/home-page-redesign
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 739 bytes | 369.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/ngabo-112/Gym-Git-Exercise-Solutions/pull/new/ft/home-page-redesign
remote: 
To https://github.com/ngabo-112/Gym-Git-Exercise-Solutions
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
```

## bundle 4
### exercise 1
```

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (ft/team-page)
$ git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/faq-page
  ft/service-redesign
* ft/team-page
  main

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (ft/team-page)
$ git checkout ft/faq-page
M       README.md
Switched to branch 'ft/faq-page'

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git switch main
M       README.md
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
$ git add .

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
$ git commit -m " changed the index.html"
[main 40482ad]  changed the index.html
 2 files changed, 190 insertions(+), 1 deletion(-)

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
$ git push origin main
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 2.21 KiB | 754.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/ngabo-112/Gym-Git-Exercise-Solutions
   a8b3a22..40482ad  main -> main

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
$ git branch 
  dev
  ft/bundle-2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
  ft/team-page

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
$ 

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
$ git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git rebase main
Successfully rebased and updated refs/heads/ft/home-page-redesign.

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git add .

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git commit -m "added a paragraph"
[ft/home-page-redesign 07e87a4] added a paragraph
 1 file changed, 1 insertion(+)

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git push origin ft/home-page-redesign
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 739 bytes | 369.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/ngabo-112/Gym-Git-Exercise-Solutions/pull/new/ft/home-page-redesign
remote: 
To https://github.com/ngabo-112/Gym-Git-Exercise-Solutions
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
$ git fetch main 
fatal: 'main' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
$ git fetch origin main
fatal: unable to access 'https://github.com/ngabo-112/Gym-Git-Exercise-Solutions/': Could not resolve host: github.com

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
$ git fetch origin main
remote: Enumerating objects: 9, done.
remote: Counting objects: 100% (9/9), done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 5 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (5/5), 2.83 KiB | 58.00 KiB/s, done.
From https://github.com/ngabo-112/Gym-Git-Exercise-Solutions
 * branch            main       -> FETCH_HEAD
   40482ad..2d70c3c  main       -> origin/main

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
$ git pull origin main
From https://github.com/ngabo-112/Gym-Git-Exercise-Solutions
 * branch            main       -> FETCH_HEAD
Updating 40482ad..2d70c3c
Fast-forward
 faq.html     | 11 +++++++++++
 service.html |  4 +++-
 2 files changed, 14 insertions(+), 1 deletion(-)
 create mode 100644 faq.html

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
$ git push origin main
Everything up-to-date

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
$ git remote add git-copy https://github.com/ngabo-112/git-exercise-clone.git

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
$ git remote 
git-copy
origin

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
$ git add index.html

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
$ git commit -m "added on the git repository"
[main ecaa349] added on the git repository
 1 file changed, 1 insertion(+)

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
$ git push git-copy main
Enumerating objects: 56, done.
Counting objects: 100% (56/56), done.
Delta compression using up to 4 threads
Compressing objects: 100% (51/51), done.
Writing objects: 100% (56/56), 10.83 KiB | 461.00 KiB/s, done.
Total 56 (delta 22), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (22/22), done.
To https://github.com/ngabo-112/git-exercise-clone.git
 * [new branch]      main -> main

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 347 bytes | 86.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/ngabo-112/Gym-Git-Exercise-Solutions
   2d70c3c..ecaa349  main -> main

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
$ git remote rm git-copy

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
$ git remote
origin

USER@DESKTOP-6F4ICRN MINGW64 ~/Documents/Gym-Git-Exercise-Solutions (main)
```