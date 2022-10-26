# git-tutorial

This is a quick little playground to understand git a little better.

Cherry-picking...

We will need to put all pages of the book into a new branch that isn't yet created. Currently the master branch has the majority of the book, but another author has written page 3 and wants to put it into our book. While we could just pull request that branch into master, it has a bad bit of work in it which we don't want. You'll need to do a pull request to make sure that we aren't just adding chunks of the book to our 'golden copy' aka master, so you'll need to branch off master so you can use it as your starting point. Your changes will then be on top of this.

1. Start by creating your new branch from master.
2. Cherry-pick the commit for page 3 from the branch named 'branch-to-add-page-3' and push the commit
3. Create a pull request and see your changes between your branch and the destination branch (master)
4. Merge/complete the pull request so you can move onto the next task.

Merge conflicts...

It turns out that someone else has also been working on a page 3 and they too have written a chunk that you don't want to overwrite, and therefore you will have to resolve the merge conflicts before you can merge this other branch with a page 3 in it also.

1. Checkout the branch 'conflicts'
2. Merge 'master' into 'conflicts' so you can catch up with the latest changes to master.
3. You should now see merge conflicts. You can open these in beyond compare or any preferred diff tool and then update your changes to work with whoever beat you to making changes in that file. In this case, we quite like what they have added so we will add the changes we merged in from master to the end of the line.
4. Once conflicts are resolved, you can then commit the merge and push it.
5. You can now do a pull request to see your changes to the file.
