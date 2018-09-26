# test-rebase-squash
test-rebase-squash

# pulling

https://stackoverflow.com/questions/48927248/git-pull-rebase-explanation

`git pull --rebase`

instead of

`git pull`

# merging

https://stackoverflow.com/questions/16666089/whats-the-difference-between-git-merge-and-git-rebase/16666418#16666418

`git rebase branch_name`

instead of

`ggit merge branch_name`

# squashing

A word of caution: Only do this on commits that haven’t been pushed to an external repository. If others have based work off of the commits that you’re going to delete, plenty of conflicts can occur. Just don’t rewrite your history if it’s been shared with others.

1) http://gitready.com/advanced/2009/02/10/squashing-commits-with-rebase.html
2) https://gist.github.com/patik/b8a9dc5cd356f9f6f980

`git reabse -i Head~4` for 4 last commits

check link 1 above.

