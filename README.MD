## Cursor Project Template

### Installation Steps:

Either:
Fork this repository on GitHub for a new repository, or for an existing repository:

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

### Convenience

Use this as an all in one to quickly update a repository. You may have merge conflicts that need to be updated.

```
git fetch upstream; git merge upstream/main; git push --force
```
