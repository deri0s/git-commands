# Set up remote branches
## When the repository is part of the same team/company
```
git clone url
cd location/folder
```
Copy the files in the remote repository to the local computer. Then we set the working directory to be the folder location.

```
git fecth
```
Creates a copy of the remote repository into the local tracking-branch, tipically named origin/main.

```
git merge origin
```
I am specifically naming the remote-tracking branch `origin`.
an intended error

- When working with this repository for the first time:
Creates a copy of the remote-tracking branch, origin/main/ into the local branch main.
- When we want to update our local branch with the remote one:
Merges (updates) the main branch with the content in the remote branch.