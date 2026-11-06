# Contributing

Thanks for your interest in contributing to this project.

## Development Workflow

1. Work on `test`, or a feature branch off it (see Branches below).
2. Make focused, well-described commits.
3. Describe your changes in a new `## vYY.MM.DD` entry at the top of `CHANGELOG.md` (see Versioning below).
4. Open a pull request from `test` into `main`.

## Code Style

For `profile/README.md`, the public org profile:

- Use each service's full name ("Stux.Design Status", not "Status"), and list it in the right table: Our Services
  (live sites), What We Design (studio services) or Templates. Keep it in step with the cards on
  [services.stux.design](https://services.stux.design) (`StuxDesign/Services`) when a service is added, retired or
  renamed.
- Link public repos only; private ones (such as `errorpages`) stay off the profile.
- Keep the header logo as the light/dark `<picture>`, the Service Status section linking
  [status.stux.design](https://status.stux.design), and the shared Stux.Group footer.

## Branches

- Work on `test`, or on a feature branch off it. Never push to `main`
- Changes reach `main` only through a pull request from `test` into `main`, which needs CI to pass and is reviewed and merged by Leo
- Merging into `main` updates the org profile at github.com/StuxDesign; release commits and tags are made on `test` (`git push origin test --tags`) and go live when the pull request is merged

## Versioning

This project uses [Date Versioning](https://datevers.ing). To release:

1. Add a `## vYY.MM.DD` entry at the top of `CHANGELOG.md`, with its sections in this order: Added, Changed, Fixed, Removed, Security, Deprecated.
2. Set `VERSION.md` to the same bare version (no `v`): today's **UTC** date as `YY.MM.DD`, or `YY.MM.DD-1`, `-2`… for later releases the same UTC day. Never a future date. Use UTC, not local time: just after midnight in the UK it is still the previous day in UTC.
3. Run `bash tests/version.sh`.
4. Run `./commit.sh "Release vYY.MM.DD"` (or `commit.bat "Release vYY.MM.DD"` on Windows). It checks the version, commits with that message and tags `vYY.MM.DD`, and never pushes.
