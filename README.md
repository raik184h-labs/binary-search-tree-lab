## Cursor Project Template

### Installing this into a new repository

1. Just fork it!

### Installation this into an existing repository

1. Open the repository locally
2. Open in your terminal
3. Run this command to set the upstream of the repository to the template. This is only required one time.

```
git remote add cursor-project-tempate-upstream https://github.com/raik183h-master/cursor-project-template.git
```

4. Optionally run `git remote -v` to see existing remotes
5. Run this command to fetch upstream from the cursor project template:

```
git fetch cursor-project-tempate-upstream
```

6. Run this command to merge the cursor project template to the current repository:

```
git merge cursor-project-tempate-upstream/main --allow-unrelated-histories
```

7. Push the changes.

```
git push
```

### Syncing an existing repository (that wasn't forked) that uses this template

Use this as an all in one to quickly update a repository. **Note: the `-X ours` flag tells git:**

- If there’s no conflict → merge normally.
- If there’s a conflict → take my branch’s version (“ours”) instead of upstream’s.

If you don't want that behavior, remove the `-X ours` flag. You may have merge conflicts that need to be updated if you remove the flag.

```
git fetch cursor-project-tempate-upstream
git merge cursor-project-tempate-upstream/main -X ours
git push
```

### Edit (October 10th, 2025):

I changed the usages of `upstream` to `cursor-project-tempate-upstream`. For repositories that named this upstream branch `upstream` instead of `cursor-project-tempate-upstream`, replace usages of `cursor-project-tempate-upstream` with `upstream` (or whatever the name of the upstream branch is that you see listed in `git remove -v`!
