## Cursor Project Template

### Installing this into a new repository

1. Just fork it!

### Installation this into an existing repository

1. Open the repository locally
2. Open in your terminal
3. Run this command to set the upstream of the repository to the template. This is only required one time.

```
git remote add upstream https://github.com/raik183h-master/cursor-project-template.git
```

4. Optionally run `git remote -v` to see existing remotes
5. Run this command to fetch upstream from the cursor project template:

```
git fetch upstream
```

6. Run this command to merge the cursor project template to the current repository:

```
git merge upstream/main
```

7. Run this command to push the changes. `--force` is required because trying to set an upstream branch that has no related history to the current repository is considered unnatural:

```
git push --force
```

### Syncing an existing repository (that wasn't forked) that uses this template

Use this as an all in one to quickly update a repository. **Note: the `-X ours` flag tells git:**

- If there’s no conflict → merge normally.
- If there’s a conflict → take my branch’s version (“ours”) instead of upstream’s.

If you don't want that behavior, remove the `-X ours` flag. You may have merge conflicts that need to be updated if you remove the flag.

```
git fetch upstream
git merge upstream/main -X ours
git push
```
