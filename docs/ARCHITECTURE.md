# Architecture

This repository is a distribution point, not a build system.

## Components

- **`README.md`**: what the trailers are and how to get them.
- **`specs/`**: the spec each new trailer was rendered from (silo-video pipeline format).
- **`metadata/`**: upload metadata per trailer: title, description, tags, target channel, file sizes and sha256 digests of the release assets.
- **GitHub Releases**: the trailer files themselves. Video files are attached to a release as assets rather than committed to the git history, so the repository stays small.

## Data flow

1. Trailers are rendered elsewhere from real gameplay of each game.
2. Each finished batch is published as one GitHub release, with one vertical and one landscape MP4 per game.
3. Viewers download the files from the release page; nothing is served from the repository tree.

## Build and deploy

There is no build or CI in this repository. A new batch is published by creating a new release and attaching the MP4 files, then adding an entry to `CHANGELOG.md`.
