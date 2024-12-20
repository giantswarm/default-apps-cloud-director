# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Removed

- Removed `renovate` config.

## [0.11.0] - 2024-10-21

> [!WARNING]
> This release includes changes that enable the unification of cluster-cloud-director and default-apps-cloud-director. The unification
> of cluster-cloud-director and default-apps-cloud-director does not happen automatically, it must be enabled explicitly and even then
> it requires manual steps.

**See `cluster-cloud-director` [changelog](https://github.com/giantswarm/cluster-cloud-director/blob/main/CHANGELOG.md#0620---2024-10-21) for the upgrade walkthrough.**

### Added

- New Helm value `.Values.deleteOptions.moveAppsHelmOwnershipToClusterCloudDirector`, which, when enabled, will pause all apps in the default-apps-cloud-director, and it will enable the below hooks. The apps are paused in order to prevent the deletion of Chart resources in the WC.
- Helm hook to remove app-operator finalizer from App CRs, so that App CRs are deleted from the MC, while Chart CRs stay on the WC.
- Helm hook to propagate pause annotation to all bundled apps.

## [0.10.0] - 2024-10-01

### Added

- Add `observability-policies` app.

### Changed

- Update `teleport-kube-agent-app` to v0.10.3.
- Update `vertical-pod-autoscaler-app` to v5.3.0.
- Update `vertical-pod-autoscaler-crd` to v3.1.1.
- Udpate `observability-bundle` to v1.6.2.
- Update `node-exporter-app` to v1.20.0.
- Update `security-bundle` to v1.8.2.
- Update `cert-exporter` to v2.9.2.

## [0.9.0] - 2024-07-18

### Changed

- Update `cert-exporter` to v2.9.1.
- Update `cert-manager-app` to v3.8.0.
- Update `k8s-dns-node-cache-app` to v2.8.1.
- Update `net-exporter to v1.21.0`
- Update `observability-bundle` to v1.4.0.
- Update `security-bundle` to v1.7.1.
- Update `teleport-kube-agent-app` to v0.9.2.
- Update `vertical-pod-autoscaler-app` to v5.2.4.

## [0.8.0] - 2024-04-09

### Added

- Add `cilium-servicemonitors` app.
- Add `capi-node-labeler` app.
- Add `k8s-dns-node-cache` app.

## [0.7.4] - 2024-02-15

### Changed

- Bump `observability-bundle` to `v1.2.2`.

## [0.7.3] - 2024-02-12

### Added

- Include support for schemadocs to generate Chart README file

### Changed

- Bump `observability-bundle` to `v1.2.1`.

## [0.7.2] - 2024-01-30

### Added

- Add `security-bundle` app.

### Changed

- Use a YAML object for the apps configuration, so that defaults are not overwritten when users pass custom values.
- Bump observability-bundle to 1.0.0. Beware that this version contains breaking changes

## [0.7.1] - 2024-01-04

### Added

- Added `teleport-kube-agent` app

## [0.7.0] - 2023-12-08

### Changed

- Update `net-exporter` to `v1.18.1`.
- Update `etcd-kubernetes-resources-count-exporter` to `v1.8.0`.
- Update `vertical-pod-autoscaler-app` to `v4.6.0`.
- Update `observability-bundle` to `v0.10.1`.
- Update `node-exporter-app` to `v1.18.0`.
- Update `cert-exporter` to `v2.8.4`.
- Update `cert-manager-app` to `v3.6.1`.

## [0.6.5] - 2023-12-07

### Changed

- Bump `metrics-server-app` to `v2.4.1`.
- Bump `etcd-kubernetes-resources-count-exporter` to `v1.7.0`.
- Bump `observability-bundle` to `v0.8.9`.
- Bump `cert-manager-app` to `v3.5.0`.

### Added

- Added `chart-operator-extension` version `v1.1.1` that contains e.g. `ServiceMonitors` for `chart-operator`.

### Fixed

- Fix `extraConfigs` range operator
- Shortened `etcd-kubernetes-resources-count-exporter` appName to `etcd-k8s-res-count-exporter`.

### Changed

- Bump `node-exporter-app` to `1.18.0`

## [0.6.4] - 2023-09-22

### Added

- `podAnnotations` for `node-exporter` app to be able to collect systemd-related metrics.

## [0.6.3] - 2023-09-20

### Changed

- Bump `observability-bundle` to `0.8.2`.

## [0.6.2] - 2023-08-31

### Changed

- Bump `cert-manager-app` to `3.3.0`.
- Bump `observability-bundle` to `0.7.5`.
- Bump `vertical-pod-autoscaler-app` to `4.0.0`.

## [0.6.1] - 2023-08-25

### Changed

- Bump `cert-manager-app` to `3.2.0`.

### Fixed

- Set `enableServiceLinks: true` for cert-manager@v3.

## [0.6.0] - 2023-08-03

### Changed

- Bump `cert-manager-app` to `3.1.0`.

## [0.5.4] - 2023-07-25

### Added

- Add `etcd-kubernetes-resources-count-exporter`.
- Update `cert-manager-app` values in preparation of v3.0.0 release.

### Changed

- Add support for deploying on clusters where network traffic is completely blocked by default with cilium.
- Bump `vertical-pod-autoscaler-app` to `3.5.3`.
- Bump `observability-bundle` to `0.7.1`.

## [0.5.3] - 2023-05-23

### Changed

- Bump `observability-bundle` to `0.4.2`.

### Fixed

- Fix missing schema for `certManager` config.
- Fix cluster DNS service name for `net-exporter` (`kube-dns` -> `coredns`).

## [0.5.2] - 2023-04-13

### Changed

- Bump `observability-bundle` to `0.4.0`.

### Removed

- Remove kube-state-metrics app as it is now included in the observability-bundle.

## [0.5.1] - 2023-04-13

### Changed

- Bump `vertical-pod-autoscaler-app` version to `3.4.1`.
- Bump `vertical-pod-autoscaler-crd` version to `2.0.1`.
- Bump `cert-manager-app` version to `v2.21.0`.
- Bump `kube-state-metrics-app` version to `1.15.0`.
- Bump `net-exporter` version to `1.14.0`.
- Bump `metrics-server-app` version to `2.1.0`.
- Bump `cert-exporter` version to `2.4.0`.
- Change default clusterIssuer from `private-giantswarm` to `letsencrypt-giantswarm`.

## [0.5.0] - 2023-03-29

### Added

- New app dependency mechanism (`app-operator.giantswarm.io/depends-on`) to the vertical-pod-autoscaler-app it is not installed until the corresponding CRD app is deployed.
- Enable configuration of Apps with the [extraConfig](https://github.com/giantswarm/rfc/tree/main/multi-layer-app-config#enhancing-app-cr) key.

## [0.4.1] - 2023-03-25

### Fixed

- Corrected user secret name string.

### Changed

- Bump `vertical-pod-autoscaler-app` to 3.3.0

## [0.4.0] - 2023-03-07

### Removed

- :boom: Breaking! Remove `cilium` and `cloud-provider-cloud-director` App CRs. They are now installed with `cluster-cloud-director` using `HelmRelease` CRs. Please not this is compatible only with `cluster-cloud-director` version `0.7.0` and newer.

## [0.3.9] - 2023-02-23

### Changed

- Bump `observability-bundle` version to `0.2.0`.
- Bump `cert-manager-app` version to `v2.20.0`.
- Bump `cloud-provider-cloud-director-app ` version to `0.2.3`.

### Fixed

- Fix templated secret name.

## [0.3.8] - 2023-02-20

### Changed

- Bump `cloud-provider-cloud-director-app` version to `0.2.1`.

## [0.3.7] - 2023-02-14

### Added

- Enable `hubble` in `cilium`.
- Enable default network policies in `cilium`.
- Add tolerations to `cilium`.

### Changed

- Update `cert-manager` from `2.18.0` to `2.18.1`.

### Removed

- Stop deploying cluster-resources app (`cilium` will create network policies instead).

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

[Unreleased]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.11.0...HEAD
[0.11.0]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.10.0...v0.11.0
[0.10.0]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.9.0...v0.10.0
[0.9.0]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.8.0...v0.9.0
[0.8.0]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.7.4...v0.8.0
[0.7.4]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.7.3...v0.7.4
[0.7.3]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.7.2...v0.7.3
[0.7.2]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.7.1...v0.7.2
[0.7.1]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.7.0...v0.7.1
[0.7.0]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.6.5...v0.7.0
[0.6.5]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.6.4...v0.6.5
[0.6.4]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.6.3...v0.6.4
[0.6.3]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.6.2...v0.6.3
[0.6.2]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.6.1...v0.6.2
[0.6.1]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.6.0...v0.6.1
[0.6.0]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.5.4...v0.6.0
[0.5.4]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.5.3...v0.5.4
[0.5.3]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.5.2...v0.5.3
[0.5.2]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.5.1...v0.5.2
[0.5.1]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.5.0...v0.5.1
[0.5.0]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.4.1...v0.5.0
[0.4.1]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.4.0...v0.4.1
[0.4.0]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.3.9...v0.4.0
[0.3.9]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.3.8...v0.3.9
[0.3.8]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.3.7...v0.3.8
[0.3.7]: https://github.com/giantswarm/default-apps-cloud-director/compare/v0.3.6...v0.3.7
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
