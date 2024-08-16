# Git Branch Notes

## 1. make a new branch
```git checkout -b fixBug```

## 2. if there is no branch in remote, push the new branch to github
```git push -u origin fixBug```

## 3. save all the changes 
```git add -A```

```git commit -m 'fix bugs'```

## 4. change from branch fixBug to local master
```git checkout master```

# Working for yourself:
## 5. merge the branch fixBug to local master
```git merge fixBug```

## 6. update the local master to the github main (at this point, you are done!)
```git push```

## 7. clean everything
* step 1: delete local branch fixBug
```git branch -D fixBug```

* step 2: delete online branch fixBug (when are done with it)
```git push -d origin fixBug```

## 8. if branch cannot be deleted locally or remotely, delete connection to remote git repository and reconnect to it
* step 1: remove connect
```git remote remove origin```

* step 2: delete branch
```git branch -D fixBug```

* step 3: reconnect to remote origin
```git remote add origin https://...(the git clone url)```

* step 4: check all the branch again
```git branch -a```

* step 5: update local git repository
```git pull```

# Collaborating with other people
## 5. always remember to pull changes from the remote master to local master
```git pull```

## 6. switch back to your fixBug branch

```git checkout fixBug ```

## 7. merge the master on the fixBug branch
``` git merge master ```

## 8. if there is merge conflict, either fix it manually or keep yours or theirs only:
* keep yours: ``` git checkout --ours . ```
* keep theirs: ``` git checkout --theirs . ```

## 9. add and commit
``` git add -A ```

``` git commit -m "merged conflicts" ```

## 10. push to remote
``` git push ```

## 11. go to git hub and issue a pull request
Click on the pull request button, and leave useful message.
