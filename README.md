# jember Maven Parent
Maven Parent Project for jember.ai Java projects. This project is used to manage the 
dependencies and plugins for all jember.ai Java projects.

## Releases 
This project is configured to automatically deploy to Maven Central when a PR is merged to the main branch.

By default, minor version is bumped. 

### Version Bumping
The version is managed via the [github-tag-action](https://github.com/anothrNick/github-tag-action?tab=readme-ov-file#bumping)

**Manual Bumping:** Any commit message that includes #major, #minor, #patch, or #none will trigger the respective version bump. If two or more are present, the highest-ranking one will take precedence. If #none is contained in the merge commit message, it will skip bumping regardless DEFAULT_BUMP.

**Automatic Bumping:** If no #major, #minor or #patch tag is contained in the merge commit message, it will bump whichever DEFAULT_BUMP is set to (which is minor by default). Disable this by setting DEFAULT_BUMP to none.
