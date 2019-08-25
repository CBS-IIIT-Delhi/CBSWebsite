## Introdution

This purpose of this guide is to explain the conventions and rules which are needed to followed to keep the this website maintainable, conflict-free while keeping the effort minimal.

## Code Structure

There are two branches.
* master (production branch)
* dev (development branch)

**master** branch is the code which is deployed and consumed by the end user. As, it is a production level branch very few people have the privileges to directy push their code in it. This is done to prevent the bad code being pushed into the deployed website.

Currently, [Mayank](https://github.com/mynkpl1998) and [Sanjit](https://github.com/skkaul) have the rights to this branch.


**dev** branch is the one of which most of you have access to write. Whatever changes you make is needed to be pushed into the dev branch and then submit a merge request to merge your code into the master. Based upon the code quality, whether it breaks the existing code or not, your request might get rejected.

*Note - It is recommended that super users (master branch administrators) should also adhere to the policy of not pushing the code directly into master branch to avoid any code-conflicts.* 
*Remember - With great power comes great responsibility.*

## How to make a contribution ?

Only group members can contribute to the website development. Make sure you have the push access to the dev branch. If you don't have, ask [Mayank](https://github.com/mynkpl1998) to send an invite link to you.
Once, you have the access to the branch you are good to go.
1. If you don't have the repository on your local system, then clone it. If you already have a local copy of the repository, then do a `git pull` inside the existing local copy. This will pull all the new changes if any from the remote repository.
2. Checkout the dev branch by using this command, `git checkout dev`
3. Now, you are inside the dev branch. Make the required changes.
4. Add your changes to the staging stage via `git add .`
5. Create a commit by giving it an appropriate commit message via `git add -m "insert-your-commit-message-here"`.
6. Push your changes to the dev remote branch via `git push -u origin dev`. Specifying the remote branch dev is optional. Even if you don't specify any branch it will push your code to dev branch as base branch of the repository is dev.
7. After, committing your changes, create a pull request. Refer to this section if you don't know how to create a pull request.

## How to report/suggest a bug or feature ?

You suggest/report a bug or feature using issues feature. You can also ask a question via issues. You can create a issue by following this link. [Create an issue](https://github.com/CBS-IIIT-Delhi/CBSWebsite/issues/new).
Make sure to provide a title and description for your query. If, possible provide a label by selecting appropriate one given in the right.


## What if I accidentally pushed the code to the master branch ?

No worries. You can't push to master branch until or unless you have access to it. If a non-administrator tries to push code directly into the master branch. Then, He/She will be will be greeted with an error message which says something like *"You don't have write permission to this branch"*. 

