## New Metadata Repository Checklist ##
- Use `github-new-repository-import` to import a base repository, and only copy the `development` (default) branch.
- Uncheck `General` => `Preserve this repository`.
- Uncheck `General` => `Allow Merge commits`.
- Uncheck `General` => `Allow Rebase commits`.
- Check `General` => `Always suggest updating pull request branches`.
- Check `General` => `Allow auto-merge`.
- Check `General` => `Automatically delete head branches`.
- Check `General` => `Include Git LFS objects in archive`.
- Set `General` => `Limit how many branches and tags can be updated in a single push` to `2`.
- Check `General` => `Auto-close issues with merged linked pull requests`.
- Create Team `development-repository-name` with the parent team `development`.
	- Assign new team to this repository.
- Check `Actions` => `General` => `Disable Actions`.
- Check `Planning` => `Agent suggestions for issues` to `Full Control`.
## New Repository Checklist ##
- Use `github-new-repository-import` to import a base repository, and only copy the `development` (default) branch.
- Create `test` branch from the `development` branch.
- Create `production` branch from the `test` branch.
- Uncheck `General` => `Preserve this repository`.
- Uncheck `General` => `Allow Merge commits`.
- Uncheck `General` => `Allow Rebase commits`.
- Check `General` => `Always suggest updating pull request branches`.
- Check `General` => `Allow auto-merge`.
- Check `General` => `Automatically delete head branches`.
- Check `General` => `Include Git LFS objects in archive`.
- Set `General` => `Limit how many branches and tags can be updated in a single push` to `2`.
- Check `General` => `Auto-close issues with merged linked pull requests`.
- Create Team `development-repository-name` with the parent team `development`.
	- Assign new team to this repository.
- Check `Planning` => `Agent suggestions for issues` to `Full Control`.
- Create `Secrets and Variables` => `Actions` => `Variables` => `BUMP_TYPE` = `patch` and `UBUNTU_VERSION` = `26.04`.
- Create initial tag with the command `git tag --annotate 0.0.0 --sign --message "Initial tag."` and pushed it to GitHub with `git push --tags`.






