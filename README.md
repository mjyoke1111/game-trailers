# Game Trailers

Gameplay trailers for small browser games: Neon Lanes, Galewarden, Hazard Pay, Sunset Ridge Time Trial and Kanban Crew.

Each trailer comes in two formats: vertical (9:16) for phones and landscape (16:9) for desktop.

Download them from the [Releases](../../releases) page.

## What is in a release

The latest release, [Trailers preview 1](https://github.com/mjyoke1111/game-trailers/releases/tag/trailers-preview-1), carries six MP4 (H.264) files:

| Game | Vertical (9:16) | Landscape (16:9) |
|---|---|---|
| Neon Lanes | `neon-lanes-trailer-vertical.mp4` | `neon-lanes-trailer-landscape.mp4` |
| Galewarden | `galewarden-trailer-vertical.mp4` | `galewarden-trailer-landscape.mp4` |
| Hazard Pay | `hazard-pay-trailer-vertical.mp4` | `hazard-pay-trailer-landscape.mp4` |

## Next releases (drafts)

**Trailers preview 2** is a draft release (not published yet). It adds Sunset Ridge Time Trial:

| Game | Vertical (9:16) | Landscape (16:9) |
|---|---|---|
| Sunset Ridge Time Trial | `sunset-ridge-time-trial-trailer-vertical.mp4` | `sunset-ridge-time-trial-trailer-landscape.mp4` |

**Trailers preview 3** is a draft release (not published yet). It adds Kanban Crew:

| Game | Vertical (9:16) | Landscape (16:9) |
|---|---|---|
| Kanban Crew | `kanban-crew-trailer-vertical.mp4` | `kanban-crew-trailer-landscape.mp4` |

Each new trailer comes with the spec that rendered it in [`specs/`](specs/) and its upload metadata (title, description, tags, sizes and sha256 digests) in [`metadata/`](metadata/).

## Install

Nothing to install. The trailers are plain MP4 files that play in any modern browser or video player.

## Usage

- **Watch or download:** open the release page and click a file, or download it with the GitHub CLI:

  ```bash
  gh release download trailers-preview-1 -R mjyoke1111/game-trailers --pattern '*-vertical.mp4'
  ```

- **Pick a format:** use the vertical files for phone feeds and Shorts-style placements, and the landscape files for desktop pages and standard video players.

## More

- [docs/ARCHITECTURE.md](docs/ARCHITECTURE.md): how the repository and its releases are organised.
- [CHANGELOG.md](CHANGELOG.md): release history.
