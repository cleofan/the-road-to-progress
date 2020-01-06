# The Road to Progress

> Step-by-step guide for vectorizing/parallelizing your code

You can best follow this tutorial the following way:
checkout the individual commits and look at the diffs.
This way you'll be able to observe how the code evolved.
The evolution shows the typical workflow.

## What you'll need

``` R
install.packages(c("pbapply", "mgcv"))
```

## Steps

1. Fork the GitHub repo (there is only the master branch) and clone your fork: `git clone https://github.com/<your-github-user-name>/the-road-to-progress.git`
2. Checkout revisions with the following hashes (use `git log --pretty=oneline` on the command line, `HEAD~3` is not really useful here):
  - Step 1: `git checkout 45d5a67`
  - Step 2: `git checkout 59eacb9`
  - Step 3: `git checkout da685ae`
  - Step 4: `git checkout 8321cdc`
  - Step 5: `git checkout 9fc2c61`
  - Step 6: `git checkout c0e1973`
  - Step 7: `git checkout 370432f`
  - Step 8: `git checkout 8ea4cd9`
  - Step 9a: `git checkout b6c7729`
  - Step 9b: `git checkout db7c892`
3. Check out Step 4 (`git checkout 8321cdc`) while creating a new branch from it: `git checkout -b <new-branch-name> 8321cdc`
4. Develop modular code by splitting the function into 2 pieces: (1) data processing + model training, and (2) prediction.
5. Use `lapply`/`sapply` to run the code in a vectorized fashion.
6. Adatp the vectorized format to show the progress and do it in parallel.
