# Advanced GitHub

A fork is a copy of a repository. Forking a repository allows you to freely experiment with changes without affecting the original project.

Most commonly, forks are used to either propose changes to someone else's project or to use someone else's project as a starting point for your own idea.

Propose changes to someone else's project
A great example of using forks to propose changes is for bug fixes. Rather than logging an issue for a bug you've found, you can:

* Fork the repository.
* Make the fix.
* Submit a pull request to the project owner.
* If the project owner likes your work, they might pull your fix into the original repository!

# Forking a repository

Visit the repository that you want to contribute to. Click on the fork button. You should see a copy of the repository in your own account.

Example:
* Repo to be forked: [https://github.com/otheruser/repo-to-be-forked]()
* Repo after forked in your account: [https://github.com/yourusername/repo-to-be-forked]()

# Cloning the repository

On GitHub, navigate to the main page of your repository.

Note: If the repository is empty, you can manually copy the repository page's URL from your browser and skip to step four.

* Clone or download button. Under the repository name, click Clone or download.
* Clone URL button. In the Clone with HTTPs section, click to copy the clone URL for the repository.

Open Git Bash.

Change the current working directory to the location where you want the cloned directory to be made.

Type git clone, and then paste the URL you copied in Step 2.

```git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY```

Press Enter. Your local clone will be created.

```git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY```

```
Cloning into `Spoon-Knife`...
remote: Counting objects: 10, done.
remote: Compressing objects: 100% (8/8), done.
remove: Total 10 (delta 1), reused 10 (delta 1)
Unpacking objects: 100% (10/10), done.
```

# Making Changes and Commiting to the cloned repository

* Make changes to your repository, add and commit the changes. Push the changes
* Note that these changes will be pushed to your forked repository and not the repository that you forked from
* Visit the repository in your GitHub account: [https://github.com/yourusername/repo-to-be-forked]()
* Notice the changes and commits made by you
* Now visit the repository in forked/other GitHub account: [https://github.com/otheruser/repo-to-be-forked]()

# Pull Requests

Pull requests let you tell others about changes you've pushed to a branch in a repository on GitHub. Once a pull request is opened, you can discuss and review the potential changes with collaborators and add follow-up commits before your changes are merged into the base branch.

After initializing a pull request, you'll see a review page that shows a high-level overview of the changes between your branch (the compare branch) and the repository's base branch. You can add a summary of the proposed changes, review the changes made by commits, add labels, milestones, and assignees, and @mention individual contributors or teams.

* Once you've created a pull request, you can push commits from your topic branch to add them to your existing pull request. These commits will appear in chronological order within your pull request and the changes will be visible in the "Files changed" tab.
* Other contributors can review your proposed changes, add review comments, contribute to the pull request discussion, and even add commits to the pull request.
* You can see information about the branch's current deployment status and past deployment activity on the "Conversation" tab.

After you're happy with the proposed changes, you can merge the pull request. If you're working in a shared repository model, the proposed changes will be merged from the head branch to the base branch that was specified in the pull request.

If status checks are required for a repository, the required status checks must pass before you can merge your branch into the protected branch.

You can close corresponding issues using a keyword in your pull request or commit message. 

# Creating a Pull Request from a Fork

* Navigate to the original repository you created your fork from.
* To the right of the Branch menu, click ```New pull request```.
* On the Compare page, click ```compare across forks```.
* Confirm that the base fork is the repository you'd like to merge  changes into. Use the base branch drop-down menu to select the branch of the upstream repository you'd like to merge changes into.
* Use the head fork drop-down menu to select your fork, then use the compare branch drop-down menu to select the branch you made your changes in.
* Type a title and description for your pull request. If you do not want to allow anyone with push access to the upstream repository to make changes to your PR, unselect Allow edits from maintainers.
* Click ```Create pull request```.

# Merging a Pull Request on GitHub

* Under your repository name, click ```Pull requests```.
* In the "Pull Requests" list, click the pull request you'd like to merge.

Depending on the merge options enabled for your repository, you can:

* Merge all of the commits into the base branch by clicking ```Merge pull request```. If the Merge pull request option is not shown, then click the merge drop down menu and select ```Create a merge commit```.
* Squash the commits into one commit by clicking the merge drop down menu, selecting Squash and merge and then clicking the ```Squash and merge``` button.
* Rebase the commits individually onto the base branch by clicking the merge drop down menu, selecting ```Rebase and merge``` and then clicking the Rebase and merge button.

Note: Rebase and merge will always update the committer information and create new commit SHAs.

* If you clicked ```Merge pull request``` or ```Squash and merge``` in step 3, type a commit message, or accept the default message. Under the commit message box, click ```Confirm merge``` or ```Confirm squash and merge```.
* If you clicked ```Rebase and merge``` in step 3, click ```Confirm rebase and merge```. Optionally, delete the branch. This keeps the list of branches in your repository tidy.