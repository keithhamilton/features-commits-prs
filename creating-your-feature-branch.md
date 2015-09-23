#Creating Your Feature Branch
Alright, you've got your name all picked out, you have a clear purpose, now
let's get to the easiest part of this whole section: actually creating your
branch.

1) Always make sure your stable development branch is up-to-date.

    $ git checkout stable-development-branch
    $ git pull origin stable-development-branch

2) Using the name you chose, create your branch, using your stable development
branch as a starting point

    $ git checkout -b my-stellar-feature-branch-name stable-development-branch

3) You're done.
