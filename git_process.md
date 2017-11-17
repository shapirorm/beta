# Person 1: Create and setup new repository

1. Create a repository: https://help.github.com/articles/create-a-repo/
2. Change to base directory on local computer
3. Clone repository to base directory using https:
  - git clone https://github.com/cseanburns/beta.git
  - also see here: 
    - https://www.atlassian.com/git/tutorials/setting-up-a-repository
4. Modify source files, code, or add new files
5. Stage/add source files
  - git add .
5. Commit changes:
  - git commit -m "notes"
6. Then push:
  - git push origin master

# Person 2: Fork, add/modify, commit

1. Fork repository on GitHub
2. Clone repository on local computer:
  - git clone https://github.com/cseanburns/beta.git
3. Make code changes or add new files
4. Stage and commit:
  - git add . && git commit -m "comment"
5. Push changes to repository on GitHub (will need to enter credentials):
  - git push origin master
6. Visit your repo on GitHub
8. Click: New Pull Request
9. Click: Create Pull Request
10. Submit pull request. Person 1 will need to review and accept.

# Person 1: Accept pull request

1. Accept on GitHub

# Person 2: Syncs with Upstream

Person 2 needs to continue to make changes but must sync repo with Person 1 
first.

1. Inform git on local machine that there is an upstream repo:
  - git remote add upstream https://github.com/shapirorm/beta.git
2. View list of remote repos:
  - git remote -v
3. Sync your forc on local machine with upstream:
  - git fetch upstream
4. Make sure you're on correct branch:
  - git checkout master
5. Merge your fork with upstream:
  - git merge/upstream
6. Check status:
  - git status
5. Push back to GitHub
  - git push

---

## Various commands and process notes

1. git pull   # update
2. git branch # displays current branch
3. git branch feature1 # completely copies master branch to feature1
4. git checkout feature1
5. make code changes now
6. git status # view changes
7. git add -A # stage changes
8. git commit -m "comment" # add comment
9. git branch # display current branch
10. git checkout master # switch back to master
11. git pull  # check to see if any changes to master; there were changes
12. git checkout feature1 # switch back to feature1
13. git merge master # try to merge with master
14. if conflict, then try to fix code if there were any changes
15. git status # check status
16. git add -A # state again
17. git commit -m "comment"
18. git push ...
19. check github (main repo) and review pull request
20. then can merge pull request on github, now into master branch; may delete 
feature1 now
21. git checkout master # switch back to master
22. git pull # to update master branch
