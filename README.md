# SiGame Packages

Public catalog of approved question packages for the SiGame VRChat world.

The upload service prepares each package and a moderator approves a specific version before publication. Unapproved and private packages are not published here.

- `catalog.json` lists the available package slots, titles and version identifiers.
- `packages/<title--id>/package.json` contains the normalized package.
- `slots/<number>/package.json` is a stable URL alias used by VRChat.
- `media/<number>.png`, `.jpg` or `.mp4` contains prepared question media. Audio uses a 64×64 H.264/AAC MP4 playback variant.

Package slots range from 0 to 255. Media slots range from 0 to 4095, are content-addressed in the publishing service and are never assigned to different content. The world stores these fixed URLs because Udon cannot create new URLs from strings at runtime.

Public Git history can retain previous versions after a package leaves the current catalog. No private packages, login links or credentials belong in this repository.

This repository starts with an empty catalog. Packages and media are added by the configured publisher after moderation.
