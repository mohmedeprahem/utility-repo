Test git commands

# Examples

```
$ git add -A
//=> "push every modified folder or file to stage area"
```

``` 
$ git status
//=> "Let you see which changed has be staged"
```

```
$ git commit
//=> "Let you explain ur edit"
```

```
$ git push
//=> "Push your change to github repo"
```

```
$ git fetch 
//=> "Grap last change of repo without marge it to my local code "
```

```
$ git merge 
//=> "Merge fetcted repo with my local repo"
```
```
$ git merge name-branch
//=> "Merge branch you are in with branch called 'name-brach'"
```

```
$ git pull 
//=> "Fetch and Merge repo at the time"
```
```
$ git branch
//=> "See all branch of repo"
```

```
$ git branch {add-name}
//=> "Create new branch called 'add-name'"
```
```
$ git checkout -b add-name
//=> "Create and move to new branch called 'add-name'"
```

```
$ git checkout -d add-name
//=> "Delete branch called add-name"
```

## Git Stach
```
$ git add -A
$ git stach 
//=> "Move your edit code to temporary .git file and make it hiden"
```
it is usefull if there task has piority than anther task

after finish piority task and commit it 
``` 
$ git stach apply 
```

### for  example 

there are 2 task: 
1. Add users
2. Sort users by name

when u work on secand task Sort users and remember u need to Add users task first but u dont wanna commit secand task with first stack so use "git stach" command 

## Conflict 

The big problem in git if anther one change file when u want push it becouse that's make conflict to fix that, first write 'git pull' to get last update of rapo then write 'git status' to know which file make conflict then move to file and fix it then commit and push it

```
$ git pull 
$ git status 
"then fix files and push it"
```

## Git log

For see all commit of repo 

```
$ git log
```
- Search using `/` then wirte text
- Quit pass `q`

### Arguments

#### One line
Show and condance our commits to single line

``` 
$ git log --oneline
```

#### Decorate
Show refrence of commit that is mean see sequence of branch of commit.

``` 
$ git log --decorate
```
#### Graph
Show sequence's events of branch of commit. 
that is mean how it came from and where it go 


``` 
$ git log --graph
```

#### p
Show what is changed of each commit


``` 
$ git log -p
```

## Git diff

Show diff between you working directory and last commit

`$ git diff `

### Arguments

#### cached 

Show diff betweeen stage area and last commit

`$ git diff --cached`

#### Head

Show diff between stage and unstage area

`$ git diff HEAD`

#### Branch
Show diff bettwen two branch

`$ git diff main`

## Git blame
Show when last time change text line in file

```
$ git blame namefile.ext
```
### Power of blame
When you write above command you can copy id of line changed like this id `f729fc16` and past it to `git log` command you will see all commit about this line.
```
$ git log f729fc16
```
## git rebase

Edit commits didnt push to repo

```
$ git rebase -i main
```