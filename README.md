# Scripts Related to the DnD Blog
## publish.sh
This script is to be run from the dev branch. It will switch to the master branch and run a merge. Then it will switch back to the dev branch while echoing a reminder to create a new branch for large features.

This is followed by a post-merge git hook which if essentially a simple if statement. If the branch is master it pushes to remote, otherwise it does nothing.