# git-commands
Some useful git commands for development


### archive specific commit for All-or-none files except deleted
```
git archive --output=changes-%ldt%-%1.zip HEAD $(git diff --name-only %1 %1^ --diff-filter=d*)
```
Reference: https://git-scm.com/docs/git-diff#git-diff---diff-filterACDMRTUXB82308203

