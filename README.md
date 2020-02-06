# Group-Project Git Flow <a name="top"></a>

Below are some best practices for working in a team and using git and Github. 

One team member should create the initial Xcode project. Add all the necessary files, folders and assets required to get the project up and running. When the scaffold project is done this team member will create a local repository through Terminal or Xcode and push the repo to Github.

1. [Git commands summary](#gitcommandsummary)   
2. [Reading Resources](#reading-resources)

## 1. Create the basic files needed to get the project started
![basic files needed](https://user-images.githubusercontent.com/1819208/73835949-50ab4400-47dc-11ea-8d2f-a659862a056c.png)

## 2. Add .gitignore file 

Add a .gitignore file on Github. At minimum include the .DS_Store and /Secrets folder to the .gitignore. 

#### Create a new file 
![create new file](https://user-images.githubusercontent.com/1819208/73855350-fb822900-4801-11ea-8f24-1f0f2db4c935.png)

#### Create .gitignore file and select swift template
![create gitignore file](https://user-images.githubusercontent.com/1819208/73855486-22d8f600-4802-11ea-99fe-e5f879c51c92.png)

#### Add files, folders to be ignored in the .gitignore file
![add filename to gitignore](https://user-images.githubusercontent.com/1819208/73982020-7d0cb080-4901-11ea-8451-64cbc1b49323.png)


## 3. Add Colloborators

A free Github account allows for three (3) collaborators. The team member who created the Xcode project and Github repo now needs to invite their team members to the project. Go to Setting page of the reop and click on Collaborators in the left column. 

![add colloborators screen](https://user-images.githubusercontent.com/1819208/73836245-d3340380-47dc-11ea-81e1-d109160f2d64.png)

## 4. Enter names in Collaborators field 

Enter the Github usernames of the team members in the collaborators field to invite them. 

![collaborators field](https://user-images.githubusercontent.com/1819208/73843354-7f311b00-47ec-11ea-85ea-7110f2686a43.png)

## 5. Collaborators invitation waiting screen 

At this point team members added would have gotten email invitations. 

![waiting invitation screen](https://user-images.githubusercontent.com/1819208/73843412-9a9c2600-47ec-11ea-9a7e-8b4c5f225ccf.png)

## 6. Email invitation 

![email invitation](https://user-images.githubusercontent.com/1819208/73843449-adaef600-47ec-11ea-9746-62bb0d988277.png)

## 7. Email invitation redirect 

![email invitation redirect](https://user-images.githubusercontent.com/1819208/73843478-bc95a880-47ec-11ea-8d91-434f9c30f8a3.png)

## 8. Push access now is granted for collaborator

After accepting the invitation team members will now have push access to the Github repository. 

![push access granted](https://user-images.githubusercontent.com/1819208/73843515-cae3c480-47ec-11ea-81ef-bc6cfbabb696.png)

## 9. Create a new branch off master for your feature

Using team collaboration Git Flow principles each team member will be assigned a feature to work on and will create a separate branch off master to work on this feature. 

**Make sure to pull the latest changes from master first**

Create a new branch from master with the following **Terminal** command

> git checkout -b nyt-bestsellers-controller

Team members will now work on their designated feature in Xcode. 

**Using git best practice push regularly to your feature branch** 

When the feature is complete go on to create a **pull request** on Github. A pull request is the act of requesting that a change your made be merged (added) to a branch, in this case you are requesting that your feature-branch be merged into the master branch. 

## 10. Open pull request when feature is complete

The pull request will be made from your feature-branch to master as pictured below. The base will be master and the compare branch will be your feature-branch. 

![open pull request](https://user-images.githubusercontent.com/1819208/73843553-dcc56780-47ec-11ea-9531-53027586ef9f.png)

## 11. Tag names in PR (pull request) 

Keeping up with best practices tag members of your team as needed in the comment section or the PR describing the change you've added. 

![tag names in PR](https://user-images.githubusercontent.com/1819208/73843577-ea7aed00-47ec-11ea-971a-9dd3b73082ab.png)

## 12. PR is now open 

At this point the pull request is open for code review from another team member. You will not be the one merging the pull request. You can request code review from a team member(s). 

![pr open](https://user-images.githubusercontent.com/1819208/73843601-f5358200-47ec-11ea-9411-25dc093647c6.png)

## 13. Review files changes in PR 

File diff changes will show lines of code that was added or deleted as a result of the feature-branch. 

![code review](https://user-images.githubusercontent.com/1819208/73843682-172f0480-47ed-11ea-9f76-db0bae02f400.png)

## 14. Other team member will review changes 

![other member will merge](https://user-images.githubusercontent.com/1819208/73843646-04b4cb00-47ed-11ea-91fd-93110cc6824b.png)

## 15. Confirm and merge PR 

In code review was passed and all is well at this point the feature-branch will be merged into master. If the feature-branch has any merge conflicts those needs to be resolved first.

![merge pr](https://user-images.githubusercontent.com/1819208/73843712-23b35d00-47ed-11ea-8c7c-1dfd68bc3c70.png)

## 16. Delete Github feature branch and on member's local machine as well 

After completing the merge the feature-branch should be deleted on Github and on the team members local machine.

![delete branch](https://user-images.githubusercontent.com/1819208/73843753-3d54a480-47ed-11ea-9523-00799b11a21e.png)

## Useful git commands <a name="gitcommandsummary"></a>

[Back to top](#top)

| Command | Summary | 
|:------:|:-------|
| git pull | (get changes from remote) |
| git push | (send changes to remote branch) |
| git push --set-upstream origin branch-name | (set upstream - connect local repo to remote) |
| git status | (show modifications if any to the working area)
| git commit -m "awesome change" | (the message associated with the commit) |
| git add . | (be very carefull with this command as it will add all modified files to the staging area, make sure you want to add all files when using this command) |
| git add filename | |
| git checkout -b new-branch-name | (creates a new branch) |
| git branch | (list your local branches, current branch is green with ```*```) |
| git branch -a | (list local and remote branches) |
| git log | (list commits) |
| git checkout branch-name | (navigate to branch-name) |
| git stash | (ignore most recent changes as you don't want to commit changes) |
| git branch -d branch-name | (delete branch-name) |
| :wq | (save and exit vim) |

## Reading Resources <a name="reading-resources"></a>

1. [Github - About merge conflicts](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/about-merge-conflicts)
