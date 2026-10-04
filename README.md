# neuroarch

Arch package policy and native recipes used by the
[Gentoo and Arch installer](https://github.com/Neur0leptic/install-system).

## Contents

- `packages/`: package lists for tiers, desktops, hardware and optional tools.
- `pkgbuilds/`: local DWL and nchat package recipes.
- `pacman/`: vanilla Arch and CachyOS repository configuration.
- `boot/`, `system/` and `btrfs-subvolumes`: native system and boot inputs.

## Integration

The installer fetches `main` automatically and records the selected commit for
resuming the same installation. No manual installer commit pins are needed.
Package selection and system configuration remain separate from the
installer's execution logic.

This is a source and configuration repository, not a binary pacman repository.
DWL uses the canonical patch and protocol from
[dotfiles](https://github.com/Neur0leptic/dotfiles).
