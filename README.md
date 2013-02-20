# git-workflows


Examples of various real-world Git workflows


## Manual website versioning with Git

Initially, you will need to clone the repo :

    git clone REPO.git
    
Next, go into the newly cloned repo:

    cd REPO
    
When there are new changes in the Git repo to pull down to the server, use "fetch"

    git fetch --all # get all remotes in case we have multiple remotes in the future
    
If you want to update to the latest commit on master branch of the remote "origin"

    git checkout origin/master # detached HEAD

## Options

You could use use --depth in your clone statement:

   git clone --depth 10 REPO.git
  
which will save time if you have a very large Git history, BUT you will not be able to push, pull or fetch
from the resulting repo. It is basically temporary and you will need to clone again to get the next commit.
    
    
