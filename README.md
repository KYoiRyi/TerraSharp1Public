# TerraSharp1Public

Public CI/CD pipeline for building NeuroCore from the private repository.

## How it works

The GitHub Actions workflow checks out the private repo using a Personal Access Token stored in repository secrets, builds Native AOT binaries for all platforms, and uploads them as workflow artifacts.

## Setup

1. Create a GitHub Personal Access Token (classic) with `repo` scope
2. Go to this repo's Settings > Secrets and variables > Actions
3. Add a new repository secret named `PRIVATE_REPO_TOKEN` with your PAT value

## Artifacts

Build artifacts are available in the Actions tab after each workflow run:
- `NeuroCore-linux-x64`
- `NeuroCore-linux-arm64`
- `NeuroCore-win-x64`
- `NeuroCore-osx-x64`
- `NeuroCore-osx-arm64`
