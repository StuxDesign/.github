# Changelog

All notable changes to Stux.Design's `.github` organization repository are documented here. Each release's sections
follow a fixed order: Added, Changed, Fixed, Removed, Security, Deprecated. This project adheres to [Date Versioning](https://datevers.ing) since v26.10.23 (`YY.MM.DD`, the UTC release date, with `-1`, `-2`… for later releases the same day); earlier releases used [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## v26.11.06-1

### Added

- `.github/workflows/ci.yml`, which runs `bash tests/version.sh` on pushes to `main` and `test` and on pull requests into `main`, so the pull request from `test` has a check to pass.

### Changed

- README (Versioning) and CONTRIBUTING (a new Branches section) say work happens on `test`, reaches `main` only through a pull request that needs CI to pass and is reviewed and merged by Leo, and that releases are committed and tagged on `test`. The commit scripts' push hint says `test`.

## v26.11.06

### Added

- The organisation profile lists Stux.Design's services, with full names: **Stux.Design**, **Stux.Design Services**
  and **Stux.Design Status**, the four studio services, and the **Stux.Design Soonpage**, **Maintenancepage** and
  **Servicepage** templates.
- A **Service Status** section on the profile, with a live status badge linking
  [status.stux.design](https://status.stux.design).

### Changed

- The profile's and README's header logo is the light/dark `<picture>` version (`logo-light.png` / `logo-dark.png`)
  instead of the single `logo.png`.
- The footer's Stuxedo icon comes from `global.media.stuxedo.com` rather than the GitHub avatar.
- The README's copyright reads Stux.Group, as on the other Stux.Design repos, and the README describes the metrics
  workflow.
- `generateMetrics.yml` pins every job to the same, newer `gh-metrics/metrics` commit (`b594ca3`, as Stux.Group's
  profile uses) instead of two different older ones.
- `CONTRIBUTING.md` matches the release flow: changes go in a new `## vYY.MM.DD` entry (not `[Unreleased]`),
  `commit.sh` takes a commit message, and the profile's conventions are written down.

### Removed

- The empty, misplaced `[Unreleased]` heading in this changelog.

## v26.10.23

### Added

- `tests/version.sh`, which checks that `VERSION.md` is a valid Date Version, a real calendar date not in the future, and the same as the newest entry in this changelog

### Changed

- Switched from Semantic Versioning to [Date Versioning](https://datevers.ing): releases are numbered by their UTC release date as `YY.MM.DD`, with `-1`, `-2`… for later releases the same day. This release follows v1.0.1
- `commit.sh` and `commit.bat` refuse a `VERSION.md` that isn't a valid Date Version or is dated in the future (UTC), and warn when it's dated before today
- `README.md` and `CONTRIBUTING.md` describe Date Versioning and the release steps

## [1.0.1] - 2026-10-08
### Added
- Bluesky and LinkedIn badges (`bsky.app/profile/stux.design`, `linkedin.com/company/stuxdesign`) in the "Connect with Us!" section, alongside the existing GitHub followers badge, matching the other Stux.Group brand profiles.

## [1.0.0] - 2026-10-05
### Added
- Initial Stux.Design org profile (`profile/README.md`) with the welcome, mission, contact and "Our Activity" sections and the shared Stux.Group footer, matching the other Stux.Group brand `.github` repos.
- `generateMetrics.yml` workflow that renders the "Our Activity" stats onto the `metrics` branch.
- `README.md`, `CONTRIBUTING.md`, `VERSION.md`, `commit.sh`/`commit.bat` and `.gitignore`, following the standard release flow.
