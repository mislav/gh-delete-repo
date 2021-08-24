# gh delete-repo

A GitHub CLI extension to delete GitHub repositories.

Installation:
```sh
gh extension install mislav/gh-delete-repo
```

You must ensure that your GitHub CLI is authorized with the `delete_repo` scope:
```sh
gh auth refresh -h github.com -s delete_repo
```

Usage:
```sh
# delete exact repo (will be prompted for confirmation):
gh delete-repo mislav/gh-test

# delete all repos matching a pattern (will be prompted to confirm each match):
gh delete-repo 'mislav/*test'
```
