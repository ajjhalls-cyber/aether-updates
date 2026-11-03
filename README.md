# Aether updates

Signed release feeds and installers for **Aether**, The Gulag Lounge desktop app. This repository contains no
source code. It is published automatically by the private release pipeline and served from GitHub Pages:
<https://ajjhalls-cyber.github.io/aether-updates/>.

- `feeds/beta.json` (Owner Preview) and `feeds/stable.json` (members): Ed25519-signed release metadata. They are
  re-signed twice a week, and Aether refuses metadata more than seven days old.
- `packages/`: NSIS installers signed with the Aether updater key. Aether verifies the signature and the version it
  is bound to before installing.

Installed copies update themselves from **Settings → Updates**. Download an installer only for a first install or
to recover; settings and data are kept.
