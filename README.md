# CodeReviewExample {WIP}


## Fork this repository
When you fork a repository, you create a copy of a repository. So forking this project will give you your own version of it.

- Click on the small fork image on the top of this page
- Congratulations! You now have a copy of this repository on your own git account

## Add collaborators to forked project
- Go to the `Settings` tab
- Go to `Collaborators`
- Add your team members here

## Add collaborators to CODEOWNERS file
- Go to the `Code` tab
- Click on the CODEOWNERS file
- Edit this file by clicking on the pencil
- Add your team members on line 2 with the syntax @membername @membertwo
- Scroll down to the bottom
- Make sure 'Commit directly to the master branch' is checked. 
- Cick 'Commit changes' to update the file


## Add branch rules to forked project
- Go to the `Settings` tab
- Go to `Branches`
- Click on `Add rule`
- Write "master" as 'Branch name pattern' 
- Check the 'Require pull request reviews before merging' 
- Click `Create` in the bottom

## Clone repository to your local machine
- Go to the `Code` tab
- Click on the 'Clone or download' button
- Grab the url
- Git clone the project by opening git bash where you want to clone the project, and type in `git clone https://github.com/YOUR-USERNAME/CodeReviewExample.git`
- If you are using a git ui like `Github Desktop` you can clone directly from that program.

You now have the project working locally on your machine. Now we can make changes to the code.


## Make changes to project locally

When making changes to code, you should always branch out and create changes on that branch.
Before creating a branch, you should always do a pull from master, to ensure you have the newest version when branching out.

- Open git bash where your project is and type `git pull` to get the newest version from master. 
- If you are using a git ui there should be a pull button.

You now have the newest version of master, and are able to branch out.

- In git bash type in `git checkout -b [name_of_your_new_branch]` this will create a new branch and switch to that branch
- If you are using a git ui there should be a `new branch` button 

You are now on a separate branch and ready to make code changes.
Make some code changes and push those changes to your branch.

Git bash:
- Make sure you have added all files you want to push to your branch by doing `git add --all`
- Type in `git commit -m "[Commit Message]"` to commit your changes
- Type in `git push -u origin [name_of_your_new_branch]`

Git ui: 
- Add the files you need from the gui
- Commit changes and add a commit message
- Push your changes to the branch

## Pull from master and create a pull request
Now it is time to pull from master, you have made your change now, but we need to check up on the master branch

- `git pull origin master` to pull changes from master into your branch.

Now you have the newest master, and you have your local changes. Now we need to get them into master.

- Navigate to github.com and find your repository. 
- Click on the tab 'Pull requests'
- Click on 'New pull request' 
- Set your 'base' to master and 'compare' to your branch
- Click on 'Create pull request'
- Fill in information about the pull request, what you have done.
- Click on 'Create pull request' 

Your pull request is now available on the branch.
If you have setup codeowners they will recieve an email about this pull request, and they can submit their review. 

## Submit review to a pull request
- Navigate to your repository on Github
- Click on the tab 'Pull requests'
- Click on the pull request you want to review
- Click on 'Add your review'

Now it is time for your code review.
You can create comments on a line by hovering over the line, and clicking the + sign that pops up.

When you are ready to finish the review click on 'Review changes'
- Comment = Create a general comment about the pull request, if you are wondering about something before approving
- Approve = Pull request is accepted, and is ready to be merged into master
- Request changes = Submit some feedback about what should be changed before the change is ready to master.

This pull request is now ready to merge in to master. Who should do it?
In our team the requester of the pull request gets to merge into master.

In your pull request click on the 'Merge pull request' button when you have green lights, confirm merge and you are done!
If you don't need the branch anymore you can click on the 'Delete branch' button.



