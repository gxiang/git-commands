# git-commands
Some useful git commands for development


### archive specific commit for All-or-none files except deleted
```
git archive --output=changes.zip HEAD $(git diff --name-only $SHA $SHA^ --diff-filter=d*)
```
Reference: https://git-scm.com/docs/git-diff#git-diff---diff-filterACDMRTUXB82308203

