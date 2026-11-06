<p align="center">
  <picture><source media="(prefers-color-scheme: dark)" srcset="https://global.media.stux.design/logo-light.png"><source media="(prefers-color-scheme: light)" srcset="https://global.media.stux.design/logo-dark.png"><img src="https://global.media.stux.design/logo-dark.png" height="100" alt="Stux.Design Logo"></picture>
</p>

# .github

*Designed with purpose.*

The central repository for the Stux.Design GitHub organization configuration and profile settings.

## Overview

This repository contains the organization-wide configuration files for the Stux.Design GitHub profile, including community health files and the org's public profile page.

## What's Included

- **Profile** — the public org profile shown at [github.com/StuxDesign](https://github.com/StuxDesign) (`profile/README.md`)
- **Community Files** — contributing guidelines and other org-wide defaults
- **Activity metrics** — `.github/workflows/generateMetrics.yml` renders the profile's "Our Activity" stats to the `metrics` branch daily (needs the `METRICS_TOKEN` secret)

## How It Works

GitHub automatically applies files from this `.github` repository to all public repositories in the organization (when a specific repository doesn't have its own version), and renders `profile/README.md` as the org's public profile page.

## Getting Started

```bash
git clone https://github.com/StuxDesign/.github.git
cd .github
```

## Development

See [CONTRIBUTING.md](CONTRIBUTING.md) for the development workflow and release process.

## Versioning

This project uses [Date Versioning](https://datevers.ing): each release is numbered by its UTC release date as `YY.MM.DD` (for example `26.10.23`), with `-1`, `-2`… for later releases the same day. See [CHANGELOG.md](CHANGELOG.md) for what changed in each release.

## Copyright

© 2026 Stux.Group. All rights reserved.

---

*Built & Maintained by <img src="https://global.media.stux.design/icon.png" height="14" alt="Stux.Design" valign="middle"> [Stux.Design](https://github.com/StuxDesign), Hosted by <img src="https://global.media.stuxedo.com/icon.png" height="14" alt="Stuxedo" valign="middle"> [Stuxedo](https://stuxedo.com).  
Stux.Design is a part of the <img src="https://global.media.stux.group/icon.png" height="14" alt="Stux.Group" valign="middle"> Stux.Group brand of businesses.*
