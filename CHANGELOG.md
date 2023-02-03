# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Changed

- Update `cert-manager` from `2.18.0` to `2.18.1`.

## [0.3.6] - 2023-01-24

### Added

- Added `vertical-pod-autoscaler@2.5.3` & `vertical-pod-autoscaler-crd@1.0.1`.

## [0.3.5] - 2023-01-18

### Changed

- Update `observability-bundle` from `0.1.8` to `0.1.9`
- Update `kube-state-metrics` from `1.14.1` to `1.14.2`

## [0.3.4] - 2023-01-11

### Changed

- Update `node-exporter` to `1.15.0`

## [0.3.3] - 2023-01-05

### Changed

- Changed compatibleProvider from `vcd` to `cloud-director`.

## [0.3.2] - 2022-12-08

### Changed

- Bump `cloud-provider-cloud-director-app` version to `0.2.0`.

## [0.3.1] - 2022-12-07

### Changed

- Update `observability-bundle` from `0.1.3` to `0.1.4`

## [0.3.0] - 2022-12-06

### Added

- Added `observability-bundle` as default app
- Supports installing apps `inCluster`

## [0.2.2] - 2022-12-01

### Changed

- Bump `cloud-provider-cloud-director-app` version to `0.1.3`.

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

[Unreleased]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.3.6...HEAD
[0.3.6]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.3.5...v0.3.6
[0.3.5]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.3.4...v0.3.5
[0.3.4]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.3.3...v0.3.4
[0.3.3]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.3.2...v0.3.3
[0.3.2]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.3.1...v0.3.2
[0.3.1]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.3.0...v0.3.1
[0.3.0]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.2.2...v0.3.0
[0.2.2]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.2.1...v0.2.2
[0.2.1]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.2.0...v0.2.1
[0.2.0]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.1.0...v0.2.0
[0.1.0]: https://github.com/giantswarm/default-apps-cloud-director/releases/tag/v0.1.0
