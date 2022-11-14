# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.2.1] - 2022-11-14

### Changed

- Use `clusterValues` `secret` for `cert-manager` (requried to create a fresh cluster behind a proxy.
- Set `ipam` mode from `cluster-pool` to `kubernetes` for cilium cni.

## [0.2.0] - 2022-10-17

### Added

- Added `cloud-provider-cloud-director app`.
- Added `application.giantswarm.io/app-type: bundle` annotation.

## [0.1.0] - 2022-06-24

### Changed

- Renamed the repo from `default-apps-vcd`.

### Added

- Add initial default apps.

[Unreleased]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.2.1...HEAD
[0.2.1]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.2.0...v0.2.1
[0.2.0]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.1.0...v0.2.0
[0.1.0]: https://github.com/giantswarm/default-apps-cloud-director/releases/tag/v0.1.0
