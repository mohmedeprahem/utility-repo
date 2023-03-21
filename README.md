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

