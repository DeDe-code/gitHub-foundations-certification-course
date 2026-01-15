### Git Hidden Folder
There is a hidden folder callled `.git` which tells you that your project is a git repo.

If we want to create a git repo in a new project we create the folder and then initialize that repo using `git init`
```sh
mkdir /workspaces/tmp/new-project
cd /workspaces/tmp/new-project
git init
touch Readme.md # create Readme.md file
code Readme.md
git status # we can see what's going on here; what files are being tracked or untracked
#makes changes to readme.md
git add . # add all changes
git commit -m "add readme file" 
```  

## Cloning
We can clone three ways: HTTPS, SSH, GithubCLI
Since we are using Github Codespaces we'll create temporary directory in our workspace
```sh
mkdir /workspace/tmp
cd /workspace/tmp
```
### HTTPS
```sh
git clone https://github.com/DeDe-code/gitHub-foundations-certification-course.git
cd gitHub-foundations-certification-course
```
## Commits
When we want commit the code we can write git commit which will open up the commit message in the editor of choice.
```sh
git commit
```
Set the global editor
```
git config --global core.editor emacs
```

Make a commit and a commit message without opening an editor
```sh
git commit -m "commit message"
```
## Branches


## Remotes


## Stashing


## Merging

## Add
When we want to stage changes that will be included in the commit. W can use the . to add all possible files

```
git add Readme.md
gir add .
```



## Reset
Reset allows you to move staged changes to be unstaged. This is useful when you want to all files not to be commited.
```sh
git add .
git reset
```
> git reset will revert a git add .

## Status
Git status shows you what files will or will not commited.
```
git status
```

## Gitconfig file
The git config file is what stres your global configurations for git such as email, name, editor and more
Showing the contents of our .git config file
```
git config --list
```
When you first install Git on a machine you are suppose to set uo your name and email
```sh
git config --global user.name "John Doe"
git config --global user.email "johndoe@example.com"
```
## Log
git log will show recent git commits to the git tree
```sh
gti log
```

## Push
When we want to push a repo to our remote origin
```sh
git push
```