# Pulling, Merging, and Pushing with Git

<!--
  author: Your Name
  version: 1.0
  comment: Introduction to git pull, merge and push operations
-->

# Introduction to Git Pull, Merge & Push

Welcome to this interactive training on using Git for collaboration. In this module, you'll learn how to fetch updates from a remote repository, merge them with your local code, and push your changes back to the shared repository.

Git is a distributed version control system, which means every developer has a complete copy of the project history. This makes operations like pulling, merging, and pushing crucial for maintaining collaboration without conflicts.

## Pulling from a Git Repository

The `git pull` command is used to update your local repository with changes from a remote repository. It is a combination of two commands:

```bash
git fetch
git merge
```

When you run:

```bash
git pull origin main
```

Git fetches the changes from the remote branch `main` and then merges them into your current branch. If there are no conflicts, this process happens automatically.

### Example

```bash
git pull origin main
```

This pulls the latest changes from the `main` branch on the remote named `origin`.

### Watch: Git Pull Explained

@[https://www.youtube.com/watch?v=0K2Xc1xK6Uo](YouTube: Git Pull Explained)

## Quiz: Understanding `git pull`

### What does `git pull` do?

- [ ] Only downloads changes from the remote repo
- [x] Fetches and merges changes from the remote repo
- [ ] Only merges changes without downloading
- [ ] Deletes local changes and resets to remote


## Quiz: Merging with `git pull`

### What happens if there are conflicts during `git pull`?

- [ ] Git ignores them and completes the merge
- [ ] Git discards remote changes
- [x] Git pauses and asks you to resolve the conflicts
- [ ] Git resets to the last commit

---

# Merging and Pushing Changes

Once you’ve made changes locally and want to share them, you first commit them and then push them to the remote repository.

### Step-by-step

1. Add changes:
   ```bash
   git add .
   ```

2. Commit changes:
   ```bash
   git commit -m "Describe your changes"
   ```

3. Push to remote:
   ```bash
   git push origin main
   ```

If someone else pushed changes before you, you might need to pull and merge before pushing.

### Handling Merge Conflicts

If there are changes on the remote repository that conflict with yours, Git will notify you and mark the conflicting files. You'll need to manually resolve these before you can complete your merge and push.

## Quiz: What does `git push` do?

- [ ] Downloads new changes from remote
- [ ] Resets your local branch
- [x] Uploads local commits to a remote branch
- [ ] Deletes remote history

## Quiz: Order of Operations

### Which is the correct order of commands when collaborating?

- [ ] commit → push → pull
- [x] pull → commit → push
- [ ] push → merge → pull
- [ ] commit → merge → fetch

---

## Summary

- Use `git pull` to get the latest changes
- Make your edits, `add`, and `commit` them
- Use `git push` to upload your changes
- Resolve any merge conflicts as needed

Thanks for learning Git basics with LiaScript!
