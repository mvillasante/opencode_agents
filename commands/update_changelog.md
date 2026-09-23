---
description: Update CHANGELOG.md file
---

Base on the git diff between latest version tag (vX.Y.Z) and the latest commit (HEAD), update the CHANGELOG.md file.

The versioning should follow the semver version framework. For our projects, usually API entrypoints will be equivalent to CLI commands. 

Notable changes changes will be on the files:
- */cli.py
- */api.py
- */cli.R

## References:
- https://keepachangelog.com/en/1.0.0/
- https://semver.org/
