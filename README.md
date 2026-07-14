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