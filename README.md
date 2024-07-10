# snippets

Useful code snippets for all sorts of things.

## Git

To configure git aliases, use:

```shell
git config --global alias.<alias_name> <command>
# for scripts
git config --global alias.<alias_name> '!sh <path/to/script.sh>'
```

### Scripts

* [git-better-branch.sh](./git-better-branch.sh)

### Commands

* `git maintenance`: runs a cron job to clean up repositories.
* `git config core.fsmonitor true`: for large repositories where `git status` might take a long time.
* `git clone --filter=<filter>`: for large repositories or slow connections. Example: `git clone --filter=blob:none`.
* `git sparse-checkout set <subdir1> <subdir2>`: for large monorepos where only specific folders are needed.
* `git push --force-with-lease`: warns about force pushing if someone else has made a change.