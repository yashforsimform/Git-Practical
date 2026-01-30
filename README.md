# Git-Practical

Git Practical Exam

steps:- 
1. Created Project setup branch with the name "TE-T189_Project_Setup"
2. Created develop branch from project setup branch
    - git checkout -b develop
3. created commit-msg.txt in .git/hook folder.
    - defined action for commit message.
3. created new branch "feature/one" from "develop"
    - git checkout -b feature/one
4. Perfomed multiple commits in feature/one 
    - echo "text" > file.name
    - git add file.name
    - git commit -m "msg"
    - 3# times
    
5. made PR from feature/one to develop
    -  we can do this from github, opening pull request section and tap on creat pull request, selecting from and compare.
6. while pr is in review creat feature/two from develop
7. Now commit something in your current branch and push it, In the meantime, your previous PR has been merged to develop
    - echo "text" > file.name
    - git add file.name
    - git commit -m "msg"

8. To make our feature/two up-to-date with develop, we will do rebase
    - git rebase develop

9. Create a PR for the current branch given your branch should be up to date with develop branch
    - now from github create PR, and merge it in develop

10. For any new build release add a version tag to that specific commit to keep track of each version.
    - after merging both Prs, just name it as release v1.0.0
    - git tag v1.0.0

11. Create 2 another branch (3rd and 4th) from develop, push read me changes to 3rd brach.

12. Cherry pick 3rd branch's commit to 4th branch.
    - git cherry-pick #abc1234

13. Change commit message in 4th branch
    - git commit --amend -m "new msg"

14. add 3 commit to 4th branch and delete last commit.
    - echo "text" > file.name
    - git add file.name
    - git commit -m "msg"

15. delete commit 
    - git reset --hard HEAD~1
