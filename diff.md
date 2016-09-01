Compare the difference between branches
http://stackoverflow.com/questions/9834689/comparing-two-branches-in-git
```
git diff branch1..branch2
```


Compare the difference between branches
https://git-scm.com/docs/git-diff

```
$ git diff topic master    (1)
$ git diff topic..master   (2)
$ git diff topic...master  (3)
```

(1)Changes between the tips of the topic and the master branches.

(2)Same as above.

(3)Changes that occurred on the master branch since when the topic branch was started off it.
