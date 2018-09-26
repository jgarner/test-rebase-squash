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

`git merge branch_name`

# squashing

A word of caution: Only do this on commits that haven’t been pushed to an external repository. If others have based work off of the commits that you’re going to delete, plenty of conflicts can occur. Just don’t rewrite your history if it’s been shared with others.

The other thing is generally if you lean towards medium-sized commits and just put JIRA IDs on everything then you should very rarely have to squash anything. It’s only when you have say 12 commits of “oops” and “typo” and “oops again” and “that didn’t work” and “wait that did work” and “wait no oops again that didn’t work” that you should probably squash.

http://gitready.com/advanced/2009/02/10/squashing-commits-with-rebase.html

`git rebase -i Head~4` for 4 last commits
