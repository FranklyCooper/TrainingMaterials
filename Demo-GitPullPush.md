<!--
link:      https://cdn.jsdelivr.net/gh/FranklyCooper/TrainingMaterials@1ba998b/branding.css
-->
# Pulling, Merging, and Pushing with Git

__Git Pull:__

Welcome to this interactive training on using Git for collaboration. In this module, you'll learn how to fetch updates from a remote repository, merge them with your local code, and push your changes back to the shared repository.

Git is a distributed version control system, which means every developer has a complete copy of the project history. This makes operations like pulling, merging, and pushing crucial for maintaining collaboration without conflicts.

---

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

### Watch: Git Pull Explained

!?[Gitt Pull Explained](https://www.youtube.com/watch?v=T13gDBXarj0)

---

### Quiz
__What does `git pull` do?__

- [( )] Only downloads changes from the remote repo  
- [(x)] Fetches and merges changes from the remote repo  
- [( )] Only merges changes without downloading  
- [( )] Deletes local changes and resets to remote  


__What happens if there are conflicts during `git pull`?__

- [( )] Git ignores them and completes the merge
- [( )] Git discards remote changes
- [(x)] Git pauses and asks you to resolve the conflicts
- [( )] Git resets to the last commit

---

# Merging and Pushing Changes

Once you’ve made changes locally and want to share them, you first commit them and then push them to the remote repository.

__Step-by-step:__

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

__Handling Merge Conflicts__

If there are changes on the remote repository that conflict with yours, Git will notify you and mark the conflicting files. You'll need to manually resolve these before you can complete your merge and push.

## Quiz: 

__What does `git push` do?__

- [( )] Downloads new changes from remote
- [( )] Resets your local branch
- [(x)] Uploads local commits to a remote branch
- [( )] Deletes remote history

__Which is the correct order of commands when collaborating?__

- [( )] commit → push → pull
- [(x)] pull → commit → push
- [( )] push → merge → pull
- [( )] commit → merge → fetch

---

## Summary

- Use `git pull` to get the latest changes
- Make your edits, `add`, and `commit` them
- Use `git push` to upload your changes
- Resolve any merge conflicts as needed

Thanks for learning Git basics with LiaScript!
