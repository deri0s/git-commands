# git-commands
Git commands I will usually use

## Basics
### Clone and remote upstream
```
cd location-folder
git clone url
git remote add upstream url
```
 
### Syncronise main branch and create a new one
```
git checkout main
git fetch upstream
git merge upstream/main
```
Create a new branch
```
git checkout -b new-branch
```

## Swith between GitHub accounts
If I am in account **A** and what to switch to account **B**. Proceed with the following steps:
1) Open GitBash in the repository folder and type:
   ```
   printf "protocol=https\nhost=github.com\nusername=A | git credential-manager erase
   ```

3) The usernmae is stll **A** as the following code shows:
   ```
   git config user.name
   ```

5) Change the global credentials as follows:
   ```
   git config --global -e
   ```

7) This will open the editor mode where I have to update the username and email. First, press `Insert` to edit the text, delete using `Delete`, once the fields have been edited press `Esc` to exit editor mode. Finally, press `:` followed by `wq`, where `w` and `q` stand for >write and >quit, respectively.
8) Check if the username has been changed by following step 2).  
