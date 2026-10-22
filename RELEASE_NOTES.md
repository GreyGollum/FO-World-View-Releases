# FO World Atlas 0.38.2 — Windows public beta

FO World Atlas is an offline-first research and campaign atlas. This patch
restores reviewed map coverage and strengthens the evidence boundary between
canon identity and estimated WGS84 placement.

## Patch changes

- Restores 648 previously reviewed placements that had been omitted from the
  public runtime, bringing the reviewed public atlas to 938 WGS84 records.
- Adds a durable 761-record approval ledger that distinguishes a canon location
  identity from a project-reviewed estimated placement.
- Restores 85 exact game-record crosswalks and keeps unreviewed community-map
  records withheld.
- Preserves multiple events at one place while rejecting incompatible dates or
  conflicting locations for the same event.
- Rebuilds the QGIS and KML companions from the same reviewed public dataset.
- Corrects the qualified Josh Sawyer Commonwealth reconstruction so the North
  West/South West division crosses only northern California.
- Gives the Texas Commonwealth a clearer dusty-rose fill so it remains distinct
  from the darker Four States region.

## Included map presentation

- NASA Blue Marble provides the continuous offline world imagery.
- Nine bounded USGS plates provide optional regional detail.
- Wireframe and scan-line presentation modes remain offline.
- Canon, non-canon or implied, and homebrew content remain independently
  selectable. Vault 37 remains the sole built-in homebrew point.

## Installation

1. Download the ZIP and matching `.sha256` file from the GitHub release.
2. Verify the ZIP's SHA-256 value.
3. Extract the ZIP.
4. Run the file ending in `Setup.exe` for a normal per-user installation.
5. Open **FO World Atlas** from the Windows Start menu.

The MSI is an alternative for users who specifically need Windows Installer
deployment. Most users should choose the Setup executable.

This beta is not code-signed. Verify the separately published SHA-256 checksum
before running the installer.

## Known limitations

- The USGS imagery is regional rather than worldwide.
- Fallout 76 reflects the specifically audited Steam client snapshot and may
  require review after a game update.
- Included game-area maps are project-original schematics; locally generated
  maps from supported user-owned installations remain private.
- Physical Windows installation and touch-device review remain beta acceptance
  activities.

See [DISCLAIMER.md](DISCLAIMER.md) for the complete fan-project notice.
