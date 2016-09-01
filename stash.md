
###Show differences between head revision and local version
```
$ git diff
```

###To stash changes (save changes locally)
```
$ git stash save "my new feature 1 introduced is blah blah blah ..."
```

###To list out all stash changes

```
$ git stash list
>>> stash@{0}: On add: my new feature 1 introduced is blah blah blah ...
```

###To retrieve a stashed version of code (without deleting the stash from the list)
```
$ git stash apply stash@{0}

$ git stash list
>>> stash@{0}: On add: my new feature 1 introduced is blah blah blah ...
```
###To retrieve a stashed version of code and remove the stash version on top of the stash list
```
$ git stash pop
```



