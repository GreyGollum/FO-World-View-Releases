# FO World View 0.38.0 — Windows public beta

FO World View 0.38.0 is the first release published through this dedicated
public download repository.

## Included

- Native Windows x64 NSIS and MSI installers in one verified ZIP.
- Offline Natural Earth world outline and nine bounded USGS regional imagery
  plates, with attribution and acquisition details in the package.
- Searchable source directory with official-canon, other official, reference,
  and homebrew groupings and focused status views.
- Game-local vector atlases for Fallout 3, Fallout: New Vegas, Fallout 4, and
  Fallout 76, clearly identified as X/Y coordinates rather than WGS84.
- Eighteen project-original topographic schematics for seven supported Fallout
  3 and eleven supported New Vegas worldspaces.
- Named homebrew campaigns with independent maps and timelines.
- Source-only Local Map Builder for optional use with a user's own supported
  game installation. Python 3.10 or newer with Pillow is required for this
  optional tool.
- Dependency notices, an SBOM, data-rights documentation, a clean-source release
  manifest, and checksums.

## Installation

1. Download the ZIP and matching `.sha256` file from the GitHub release.
2. Verify the ZIP's SHA-256 value.
3. Extract the ZIP.
4. Run the file ending in `Setup.exe` for a normal per-user installation.
5. Open **FO World View** from the Windows Start menu.

The MSI is an alternative for users who specifically need Windows Installer
deployment. Most users should choose the Setup executable.

## Upgrade behavior

The Setup executable retires a detected 0.37.x per-user installation's old
executable, uninstall registration, and installer-created shortcuts. It leaves
unrecognized content and private map data in `%LOCALAPPDATA%\FOworld-view` in
place. The 0.38.0 MSI retains the 0.37.x upgrade identity while using a new
per-release ProductCode.

Both the 0.37.5 NSIS and 0.37.6 MSI upgrade paths were exercised on disposable
Windows runners. Current installation, shortcut targeting, application launch,
legacy-registration removal, uninstall cleanup, and private/user-file
preservation passed.

## Known limitations

- The installers are not code-signed, so Windows may report an unknown
  publisher.
- The bundled USGS imagery is regional, not a worldwide satellite layer.
- Fallout 76 is continuously updated; its status covers a specifically audited
  client snapshot and may need review after a game update.
- Optional local map imports accept only exact supported source files and remain
  private to the local app profile.

See [DISCLAIMER.md](DISCLAIMER.md) for the complete fan-project notice.
