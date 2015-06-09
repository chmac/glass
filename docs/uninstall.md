# Uninstalling
First off, if you're uninstalling because of some unexpectedly behaviour feel free to create [an issue](https://github.com/timeglass/glass/issues) that explains your problems. I love being in converstation with the user and create the best experience possible. 

That being said, you can do the following in order to remove Timeglass from a single repository:

1. Stop the timer by running `glass stop`. If its not running thats OK, you can skip this step.
2. Remove the git hooks timeglass creates from the `.git/hooks` directory of your repo. The following files are created during installation:
     - .git/hooks/post-checkout 
     - .git/hooks/post-commit 
     - .git/hooks/pre-push

If you would like to continue and remove Timeglass entirely from your system you can continue with the following:

1. Remove the metadata directory: `~/.timeglass`
2. Remove the binaries itself from were you installed, they're named `glass` and `glass-daemon`.