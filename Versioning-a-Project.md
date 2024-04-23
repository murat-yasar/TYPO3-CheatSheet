# Versioning a Project

1. clone the project and get the latest changes
```bash
  git clone <Reponame>
  git switch <develop>
  git pull origin <develop>
```

2. Switch to the current develop branch and get the latest changes
```bash
  git switch <develop>
  git pull origin <develop>
```

3. Update the composer.json file according to the new tag (if needed)
  - `dev-develop` to `^1.2.1`
  - `extra` in, but `replace` and `version` out

4. Push the updated composer.json
```bash
  git add -all
  git commit -m "Update composer.json for tagging 1.2.1"
  git log
  git push <develop>
```

5. Check the repo, if the changes are successfully pushed on <develop> branch

6. Merge the changes to master branch
```bash
  git switch <master>
  git merge <develop>
  git push origin <master>
```

7. Check the repo, if the changes are successfully pushed on <master> branch

8. Tag the new version on <master> branch and push
```bash
  git tag 1.2.1.0
  git push origin 1.2.1.0
  git log
```

9. Check the repo, if the changes are successfully pushed on <master> branch

10. Switch to develop branch
```bash
  git switch <develop>
```

11. Update the composer.json file back to development settings
  - `^1.2.1` to `dev-develop`

12. Push the updated composer.json
```bash
  git add -all
  git commit -m "Update composer.json to develop"
  git log
  git push <develop>
```

13. Check the repo, if the changes are successfully pushed on <develop> branch

14. Delete old branch, since it's no longer needed.
```bash
  git delete <feature>
```

15. Check the repo, if the branch is successfully deleted
