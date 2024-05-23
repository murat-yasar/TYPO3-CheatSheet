# Versioning a Project

1. clone the project and get the latest changes
```bash
  git clone <repo-name>
  git switch <dev>
  git pull origin <dev>
```

2. Switch to the current <dev> branch and get the latest changes
```bash
  git switch <dev>
  git pull origin <dev>
```

3. Update the composer.json file according to the new tag (if needed)
  - `dev-develop` to `^1.2.1`

4. Push the updated composer.json
```bash
  git add -all
  git commit -m "Update composer.json for tagging 1.2.1"
  git log
  git push <dev>
```

5. Check the repo, if the changes are successfully pushed on <develop> branch

6. Merge the changes to <main> branch
```bash
  git switch <main>
  git merge <dev>
  git push origin <main>
```

7. Check the repo, if the changes are successfully pushed on <main> branch

8. Tag the new version on <main> branch and push
```bash
  git tag 1.2.1.0
  git push origin 1.2.1.0
  git log
```

9. Check the repo, if the changes are successfully pushed on <main> branch

10. Switch to <dev> branch
```bash
  git switch <dev>
```

11. Update the composer.json file back to development settings
  - `^1.2.1` to `dev-develop`

12. Push the updated composer.json
```bash
  git add -all
  git commit -m "Update composer.json to develop"
  git log
  git push <dev>
```

13. Check the repo, if the changes are successfully pushed on <dev> branch

14. Delete old branch, since it's no longer needed.
```bash
  git branch -d <feat>
  git push origin --delete <feat>
```

15. Check the repo, if the branch is successfully deleted
