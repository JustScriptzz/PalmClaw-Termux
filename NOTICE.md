# Notice

This repository ("PalmClaw-Termux") is a rebranded fork of
[termux-app](https://github.com/termux/termux-app), licensed under the
GNU General Public License v3.0 (GPLv3) only, with exceptions for
`terminal-view`/`terminal-emulator` (Apache 2.0) and `termux-shared`
(see its own LICENSE.md). See `LICENSE.md` for full details.

This fork changes only the application/package identity so it can run
as a dedicated terminal for the PalmClaw app without conflicting with
an independently-installed official Termux:

- Package name: `com.termux` -> `com.palmclaw.termux`
- App name: `Termux` -> `PalmClaw Terminal`

No other functional changes have been made. Because the package name
differs from `com.termux`, this fork cannot use Termux's official
bootstrap archives or package repository (binaries are compiled with a
fixed install-path prefix). A bootstrap rebuilt specifically for
`com.palmclaw.termux` is required and is built by this repo's own CI
using termux-packages' officially supported
`scripts/build-bootstraps.sh` fork-building process.
