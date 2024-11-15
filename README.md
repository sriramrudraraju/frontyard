# Frontyard

Design system using unstyled components

## Getting Started

This monorepo is managed using nx.

node > 22

- `npm install` -> install dependencies

## Publishing

- Uses [automatic versioning](https://nx.dev/recipes/nx-release/automatically-version-with-conventional-commits#automatically-version-with-conventional-commits)
  - 'feat' -> minor
  - 'fix' -> patch
  - 'chore' -> no version change
- Run `nx release --skip-publish` locally. This will create a commit with the version and changelog updates, then create a tag for the new version.
- Push the changes (including the new tag) to the remote repository with `git push` && `git push --tags`.
- The publish workflow will automatically trigger and publish the packages to the npm registry.
