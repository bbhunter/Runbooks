# Git history secret grepping

**Description:** This entry describes how to search the content of git history on a local repo for secrets. These are commonly found on systems after gaining an initial foothold

**Requirements:** git

## Searching git history content for secrets

```
git grep '<keyword>' $(git rev-list --all)
```

Run a single grep on all the contents in the history of a git repo
  
## References
* https://stackoverflow.com/questions/50206886/grep-all-commits-in-a-repository