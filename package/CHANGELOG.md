# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

> [!IMPORTANT]
> This is a fork of version 0.11.1 of HierarchyDecorator by [@WooshiiDev](https://github.com/WooshiiDev) (https://github.com/WooshiiDev/HierarchyDecorator/tree/b8287bf992001b2b944afbf7d031ae1ed3238e88). To prevent confusion, this fork will use separate version numbers, starting at 0.1.0.

## [Unreleased]

## [0.1.0] - 2026-01-11

### Added
- Releases published to GitHub Packages will be signed (Unity 6.3 best practice). This should have no impact on compatibility with previous versions of Unity.

### Changed
- The package display name, description, and README have been modified to make it clear that this is a different version of the package.
- Package name changed from `com.wooshii.hierarchydecorator` to `dev.mgrand.hierarchy-decorator`. Reasoning:
  - Prevent confusion with official releases from [@WooshiiDev](https://github.com/WooshiiDev).
  - Conform with [@mgranddev](https://github.com/mgranddev)'s package naming conventions.
- Restructured directories to conform with Unity package layout standards. This should not cause any functional change.
  - `Editor` moved to the package root.
  - `Scripts` renamed to `Runtime` and moved to the package root.
- Moved package contents into a new `/package` directory to support the new package signing process in Unity 6.3.

[Unreleased]: https://github.com/mgranddev/hierarchy-decorator/compare/v0.1.0...HEAD
[0.1.0]: https://github.com/mgranddev/hierarchy-decorator/compare/b8287bf992001b2b944afbf7d031ae1ed3238e88...v0.1.0
