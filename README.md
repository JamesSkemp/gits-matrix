# MonkeyGoD's Ghost in the Shell and Matrix Comparison

I realized the other day that the original, and most of the mirrors, for MonkeyGoD's ** have vanished.

Since I found the reference good many, many, years ago, I'm adding it here.

It'll be available at http://jamesskemp.github.io/gits-matrix/

## Technical Aside

This is how this repo/site was setup.

```
# Clone the repo.
git clone https://github.com/JamesSkemp/gits-matrix
# cd into it.
cd .\gits-matrix\
# Create a new, orphan, branch.
git checkout --orphan gh-pages
# Remove all files.
git rm --cached $(git ls-files)
# Checkout a single file to get a commit.
git checkout master README.md
# Add and commit the file.
git add .\README.md
git commit -m "Created new gh-pages branch."
# Push local gh-pages branch to the remote.
git push origin gh-pages
# Set remote.
git push --set-upstream origin gh-pages

# Return to master branch if needed
git checkout master
```
