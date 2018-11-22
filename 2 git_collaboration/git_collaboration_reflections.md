# Git for Team Collaboration

One more time? Okay! Git won't go amiss :smile: 

Version control is software that helps me to control different versions of my project. (pretty easy!)

One new term is SHA that is exactly id of commit. It was attractive to read about Plumbing and Porcelain command in git. All of the commands we use are user-friendly porcelain.

`git log --stat` display files that were changed and show what was changed

`git log -p` shows actual changes in commit

`git rm --cached` removes files from staging area

if we want to ignore some files to be commited create file `.gitignore` and place there all you want git to ignore.

`git branch -d nameOfTheBranch` delete branch, cant delete branch we are currently on 

`git reset --hard HEAD^` if merge on wrong branch, it undo changes

`git revert` create new commit that undos previous commit and `git reset` delete commits

To mind this course was better and easier. But here is no new info, but I refresh how to solve merge conflicts in branching, it was the hardest moment in git, but is behind now.

![image of completed course first](https://github.com/yulyasystem/kottans-frontend/blob/master/2%20git_collaboration/what-is-version-control.png)
The second course **GitHub & Collaboration** dive into remotes repositories on GitHub.

`git remote add origin url_is_here` points to the project on GitHub

marker `origin\master` called *tracking branch* and is telling us that the remote `origin` has a `master` branch. **Advice :** work in local repo and push changes to remote.
 
`git fetch` retrieves commits from remote repo but does not not merge automatically remote and local branches. we should write `git merge`. I think fetch is part of pull, and it can be used when I have changes in local and remote repo and want to mannualy merge branches.

`git shortlog` show how many commits each contributor added to the project

`--grep` flag filter commits, just like in command line `git log --grep "yulia"` will show all commits with this word :)

**best practices for writting commits:**

* to make frequent and small commits,try to avoid word 'and' cause one feature and another is not logical change.

* write understandable, clear, descriptive messages

* update README.md


**What was new for me?**

`git rebase` combines several commits in one larger, move commits to have new base. `git rebase -i HEAD~3` will squash the last 3 commits in one. `HEAD` indicates current location. to push changes after rebase it is necessary to `git push -f` `-f` flag means *fixup* combine comitts changes and drop the commit message

![image of completed course second](https://github.com/yulyasystem/kottans-frontend/blob/master/2%20git_collaboration/git-collaboration.png)

This course is all about collaboration with team members. I will intend advices for writing good commit messages. 

## Git Hooks :open_mouth:
On the Udacity course was extra material about git hooks and I get interested. **git hooks** are scripts which trigger when you perform a specific action in Git. I think it help to optimize working procces, make something work automatically. They are stored in `hooks` subderictory. To my mind it is a powerful tool and I wanna intend t in future.

