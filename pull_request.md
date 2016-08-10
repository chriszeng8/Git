#Branching, Merging and Pull Request

https://www.youtube.com/watch?v=oFYyTZwMyAg

##Branching

create a branch of a master (trunk) for modification without affecting the master code.

1. list all branches 
```
git branch
```

2. create a new branch locally(i.e., make a copy of the master)

```
git branch new_branch_name
```

3. switch to the new branch

```
git checkout new_branch_name
```

Now we can make changes to the new branch without affecting the master.
Perform the changes, then push changes like we normally do.

```
git add -A
git commit -m "feature 1 ... added"
```  

#Merging (pre-pull-request)

Before creating pull request, it is a good practice to check the status of the master branch, just to make sure the latest changes are included in the branch that we've been working under.

1. Switch back to the master branch (or the branch that we want to perform pull request to), and perform a git pull:

```
git checkout master
git pull
```


2. Merge the changes from latest master into the branch (incorporate the latest changes from master to the new branch)
```
git checkout new_branch_name
git merge master
```

3. Resolve the conflicts as necessary, then commit the resolved conflicts

```
git add -A
git commit -m ""
```

```Esc + :wq``` to quit git commit

4. push the changes to upstream origin new_branch_name

```
git push --set-upstream origin new_branch_name
```

or 

```
git push
```

and then following the suggested push command.

*Now the new branch should be pushed to github.*


#Pull Request
Use the github webpage to "create a pull request" from the new branch.
"Hey @some_team_member, please check my change".