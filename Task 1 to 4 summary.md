#This is a summary of Task 1 to 4 of my GitHub learning so far#

#----------DAY-ONE----------#

**Question1. What are git and GitHub?**
Answer1. Git is created by Linus Torvalds. Primarily for the contribution to the linux kernel development.
It is an open-source, free and distributed version control system.
Git has trunk-based development which like the name suggests involves branches in the repository. Primarily used for creating sub-branches. We can create a new branch even while working on the current branch and can also merge the new branch with the master branch if required at any point of time. GitHub is a website used for project creation that’ve version control on them. GitHub is a file or code sharing service to collaborate with different people. The platform makes the code management and sharing easy and neat. Git is an application used to implement the above features as described whereas, Github can be defined as a website or web-service that offers the git features. Github can be called a social network of projects using the core fundamentals of git.

**Question2. Why GitHub is so popular and used in most of the projects?**
Answer2. Various reasons behind Github’s popularity and usage in projects are:
1. It has an extremely large community of developers and programmers.
2. Separate repositories for public and private use.
3. Shared repositories that can be accessed by millions of users which in turn make contributions to existing files or codes available.
4. Easy control of version.
5. Accessibility. Can be accessed anytime and anywhere.

**Question3. What are the other platforms similar to GitHub?**
Answer3. Various other platforms similar to GitHub are:
1. GitLab
2. GitBucket
3. AWS Code Commit
4. Source Forge

#----------DAY-TWO----------#

**Question1. How git workflow works?**
Answer1. There is one local repository and the developer that wants to make changes clones the repository and make changes using the commit command and further pushes it to the remote repository from where developers can pull and can work on it.
The workflow mainly consists of 4 parts, named:
1. Workspace
2. Index
3. Local Repo
4. Remote Repo

**Question2. What are the different stages of git project?**
Answer2. The different stages of git project are:
• Modified:
A repository is created using Git through the files that are stored in a particular folder. Anyone can make changes to a repository that is public by cloning them inside their system and modify as their requirement and then uploading it onto GitHub so that the file can be used for Staging.
• Staged:
Git add command is used to add a file from the workspace or the working directory to the Index or the staging stage. After that the file is staged i.e., it is marked to commit but is not yet committed.
• Commit:
When we used the Git commit command, all the files that were staged in the Index are released here and the changes are committed to the local repository. Each commit command represents the changes made to project in the past, with the details about the time at which commit was made and the author of the code. So, finally when you make a commit, and it gets committed, then this simply means that you have successfully applied a certain modification to the code.

**Question3. Is it possible to do a git commit before git add? If No, explain why?**
Answer3. No, it is not possible as git add command adds the files from the working directory to the staging area and then the changes are saved using commit command in the local repository.
The rough map can be marked as: Working Directory > Staging Area > Repository

**Question 4. Why is git diff used?**
Answer4. Git diff command is used to track the differences or changes made on a file in a local
or a working directory from the Index/staging state.

**Question5. Can we leave the commit messages as blank?**
Answer5. Yes, that can be done using the following command
git commit -a --allow-empty-message -m ""

_My GitHub repository link is:_
_https://github.com/ashburn3r/CodeWayy-Github-Series_

#----------DAY-THREE----------#

**QUESTION1. What is meant by the term fork and clone?**
ANSWER1. Fork means creating a personal copy from someone else’s project and that copy can also be used as a person’s initial point of creating a project.
Also, it can be modified by the developers around the world and they can publish their own changes to it.
Clone is used to create the local copy of someone’s git repository from the GitHub in our system from the remote repository.

**QUESTION2. What are branches in GitHub?**
ANSWER2. Branches are an individual projects within a git repository. Branches are like movable pointers to the commits. All the branches are independent of each other. The default branch is the master branch. Once we have made changes to a project, we can merge that particular branch to the master branch. It is mainly used for redundancy reduction in the project.

**QUESTION3. What is PR?**
ANSWER3. PR stands for Pull Request.
User issues a pull request if he has forked and cloned someone’s else code and modified it and want to publish that code on the author’s repository. Then a pull request is issued. The one who has created the repository can review and then approve the request to incorporate the changes that has been created.

**QUESTION4. Can we delete the master branch, if not why?**
ANSWER4. Yes, we can delete the master branch but then we’ll have to create a new branch and set it as our default branch.

**QUESTION5. How can we delete a branch?**
ANSWER5. We can delete the branch in the following two ways:
To delete locally: git branch -d <branch>
To delete remotely: git push <remote> --delete <branch>

#----------DAY-FOUR----------#

**QUESTION1. What do u mean by merge conflict?**
ANSWER1. It occurs when git is unable to automatically resolve the differences in the code by itself between two commits.
When there is a conflict git doesn’t know which code to keep and which to discard. For eg if there is a conflicting change on the same line or some file is deleted on one branch but not on other.
Merge conflict can only be resolved by the developer.
These conflicts usually happen when working in a team environment.
1. Git fails to start the merge when there are changes in the working directory or staging area of current project.
2. Git fails during merge - conflict in current local branch and branch being merged.

**QUESTION2. Can we have 200 different branches other than the master?**
ANSWER2. Yes!

**QUESTION3. What is the difference between git branch -d and git branch -D?**
ANSWER3. The difference between the two is explained as follows:
The -d option will delete the branch only if it has already been pushed and merged with the remote branch
However, -D option is used if you want to force the branch to be deleted, even if it hasn't been merged or pushed yet.