# Git Guide

Before typing these commands, make sure you are in the folder of the repository on your computer.

Pull changes from remote:
```
git pull
```

Push changes:
```
git add .
git commit -m "Commit message"
git push
```

## Cloning the repository
- A repository is basically a giant folder. It can have as many subfolders as you want.
- Cloning a repository means that you're downloading the repository to your on computer so that
you can access all of the files in the repository.
- In this case, it also means that you can change or create new files on your local computer and
  upload them to the remote (GitHub version online) version of the repository.
- To simplify our workflow, we can all just work on the same branch. A branch is like a version of the
  repository that has its own history of changes that can be separate from other branches. They're used so
  that multiple people can backup their own versions of the files on separate branches without worrying about
  their changes conflicting. You don't have to worry about creating a new branch though, we will all just use
  the main branch.
- ```git clone https://github.com/alexngUNC/TheMarvels.git```
- ```cd TheMarvels``` - This command means "change directory" into the folder called TheMarvels. A directory
  is another name for a folder.

## Uploading changes to files to the remote repository
Let's say you cloned the repository so it's on your computer and you made some changes to the files.
Now, you want your changes to be uploaded to the version of the project that's on GitHub.

1. Specify which files you would like to upload the changes for:
  -  Make sure you're inside of the repository folder on your computer.
  -  Type ```git add .``` in the terminal. The . (period) refers to your current folder. This tells GitHub
     that you would like to upload all changes in your current folder and all of its subfolders. This step moves
     those changes to the "staging area" in your local version of the repository. You can unadd changes from the staging
     area. You can think of this like dropping off your changes at the post office.
     
2. Make a commit:
  - A commit is a version of the repository with the changes in the staging area included. Commits have unique IDs so
    you can go back to a commit (i.e. a past or future version of the repository) whenever you want. You can think of
    a commit like the post office putting your changes in a package.
  - Type ```git commit -m "My commit message"```. The -m is an option that means you will type your commit message on that same line in quotes.
  - Commit messages are required so that the unique ID for the commit can be created.

3. Push the commit:
  - The commit has been created in your local repository. Now, you would like the remote (GitHub website version) repository
    to update to the commit you created. To do this, you need to "push" the commit to the remote repository. Since we only have
    one remote repository, you can just type ```git push```.

4. Pull changes from remote repository:
  - Let's say someone else updated the remote repository and now you need to update your version on your computer
    with the version that's hosted on GitHub.
  - You need to "pull" the changes from the remote repository down to your local repository.
  - Type ```git pull``` and your local version of the repository will be overwritten by the remote version.
  - Make sure that you push the changes you want to make before you pull from the remote because pulling from the remote
    will make your local repository reflective of what is on GitHub.
