# Versioning Scheme

We use a modified [Semantic Versioning](https://semver.org/) (SemVer) for our project. The version format is `MAJOR.MINOR.RELEASE`, where:

- `MAJOR` version increments indicate incompatible API changes.
- `MINOR` version increments indicate addition of backward-compatible functionalities.
- `RELEASE` version increments for each pre-release and release candidate, and is reset to `0` for final releases.

## Beta Versioning (Before 1.0.0)

All versions with `MAJOR` version as `0` are considered beta, including final releases.

- Beta versions (pre-releases and final releases): `0.MINOR.RELEASE`, where `MINOR` and `RELEASE` are incremented as per changes.
- Release candidates: `0.MINOR.RELEASE`, where `RELEASE` is incremented for each release candidate.

Examples of beta versions:

- Beta: `0.1.1`, `0.1.2`, `0.2.1`, etc.
- Beta (final release): `0.28.0`, `0.29.0`, `0.30.0`, etc.
- Release candidate: `0.28.4`, `0.28.5`, `0.28.6`, etc.

## Versioning After 1.0.0

Once the project reaches `1.0.0`, the versioning will follow the original scheme:

- Pre-release versions: `MAJOR.MINOR.RELEASE`, where `RELEASE` is incremented for each pre-release.
- Release candidates: `MAJOR.MINOR.RELEASE`, where `RELEASE` is incremented for each release candidate.
- Final releases: `MAJOR.MINOR.0`.

Examples of versions after `1.0.0`:

- Pre-release (alpha): `1.28.1`, `1.28.2`, `1.28.3`, etc.
- Release candidate: `1.28.4`, `1.28.5`, `1.28.6`, etc.
- Final release: `1.28.0`, `1.29.0`, `1.30.0`, etc.

# Requirements Met

- All packages, including the VSCode extension, use the same versioning scheme.
- Users can determine whether they're running a beta version, a pre-release, a release candidate, or a final release by looking at the version number.
- The versioning scheme is simple and consistent, making it easy to automate with npm scripts and GitHub workflows.
- The versioning scheme adheres to VSCode's versioning constraints.
- The versioning scheme allows for pre-releases for each commit, the ability to tag release candidates, and published releases.
- All versions before `1.0.0` are considered beta, including final releases, aligning with the new project requirement.
