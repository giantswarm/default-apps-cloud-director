# Values schema documentation

This page lists all available configuration options, based on the [configuration values schema](values.schema.json).

<!-- DOCS_START -->

### 
Properties within the `.userConfig` top-level object

| **Property** | **Description** | **More Details** |
| :----------- | :-------------- | :--------------- |
| `userConfig.certExporter` |**None**|**Type:** `object`<br/>|
| `userConfig.certExporter.configMap` |**None**|**Type:** `object`<br/>|
| `userConfig.certExporter.configMap.values` |**None**|**Types:** `object, string`<br/>|
| `userConfig.certManager` |**None**|**Type:** `object`<br/>|
| `userConfig.certManager.configMap` |**None**|**Type:** `object`<br/>|
| `userConfig.certManager.configMap.values` |**None**|**Types:** `object, string`<br/>|
| `userConfig.metricsServer` |**None**|**Type:** `object`<br/>|
| `userConfig.metricsServer.configMap` |**None**|**Type:** `object`<br/>|
| `userConfig.metricsServer.configMap.values` |**None**|**Types:** `object, string`<br/>|
| `userConfig.netExporter` |**None**|**Type:** `object`<br/>|
| `userConfig.netExporter.configMap` |**None**|**Type:** `object`<br/>|
| `userConfig.netExporter.configMap.values` |**None**|**Types:** `object, string`<br/>|
| `userConfig.nodeExporter` |**None**|**Type:** `object`<br/>|
| `userConfig.nodeExporter.configMap` |**None**|**Type:** `object`<br/>|
| `userConfig.nodeExporter.configMap.values` |**None**|**Types:** `object, string`<br/>|
| `userConfig.vpa` |**None**|**Type:** `object`<br/>|
| `userConfig.vpa.configMap` |**None**|**Type:** `object`<br/>|
| `userConfig.vpa.configMap.values` |**None**|**Types:** `object, string`<br/>|

### 
Properties within the `.apps` top-level object

| **Property** | **Description** | **More Details** |
| :----------- | :-------------- | :--------------- |
| `apps.capi-node-labeler` |**None**|**Type:** `object`<br/>|
| `apps.capi-node-labeler.appName` |**None**|**Type:** `string`<br/>|
| `apps.capi-node-labeler.catalog` |**None**|**Type:** `string`<br/>|
| `apps.capi-node-labeler.chartName` |**None**|**Type:** `string`<br/>|
| `apps.capi-node-labeler.clusterValues` |**None**|**Type:** `object`<br/>|
| `apps.capi-node-labeler.clusterValues.configMap` |**None**|**Type:** `boolean`<br/>|
| `apps.capi-node-labeler.clusterValues.secret` |**None**|**Type:** `boolean`<br/>|
| `apps.capi-node-labeler.dependsOn` |**None**|**Type:** `string`<br/>|
| `apps.capi-node-labeler.extraConfigs` |**None**|**Type:** `array`<br/>|
| `apps.capi-node-labeler.extraConfigs[*]` |**None**||
| `apps.capi-node-labeler.extraConfigs[*].kind` |**None**|**Type:** `string`<br/>|
| `apps.capi-node-labeler.extraConfigs[*].name` |**None**|**Type:** `string`<br/>|
| `apps.capi-node-labeler.forceUpgrade` |**None**|**Type:** `boolean`<br/>|
| `apps.capi-node-labeler.inCluster` |**None**|**Type:** `boolean`<br/>|
| `apps.capi-node-labeler.namespace` |**None**|**Type:** `string`<br/>|
| `apps.capi-node-labeler.version` |**None**|**Type:** `string`<br/>|
| `apps.certExporter` |**None**|**Type:** `object`<br/>|
| `apps.certExporter.appName` |**None**|**Type:** `string`<br/>|
| `apps.certExporter.catalog` |**None**|**Type:** `string`<br/>|
| `apps.certExporter.chartName` |**None**|**Type:** `string`<br/>|
| `apps.certExporter.clusterValues` |**None**|**Type:** `object`<br/>|
| `apps.certExporter.clusterValues.configMap` |**None**|**Type:** `boolean`<br/>|
| `apps.certExporter.clusterValues.secret` |**None**|**Type:** `boolean`<br/>|
| `apps.certExporter.dependsOn` |**None**|**Type:** `string`<br/>|
| `apps.certExporter.extraConfigs` |**None**|**Type:** `array`<br/>|
| `apps.certExporter.extraConfigs[*]` |**None**||
| `apps.certExporter.extraConfigs[*].kind` |**None**|**Type:** `string`<br/>|
| `apps.certExporter.extraConfigs[*].name` |**None**|**Type:** `string`<br/>|
| `apps.certExporter.forceUpgrade` |**None**|**Type:** `boolean`<br/>|
| `apps.certExporter.inCluster` |**None**|**Type:** `boolean`<br/>|
| `apps.certExporter.namespace` |**None**|**Type:** `string`<br/>|
| `apps.certExporter.version` |**None**|**Type:** `string`<br/>|
| `apps.chartOperatorExtensions` |**None**|**Type:** `object`<br/>|
| `apps.chartOperatorExtensions.appName` |**None**|**Type:** `string`<br/>|
| `apps.chartOperatorExtensions.catalog` |**None**|**Type:** `string`<br/>|
| `apps.chartOperatorExtensions.chartName` |**None**|**Type:** `string`<br/>|
| `apps.chartOperatorExtensions.clusterValues` |**None**|**Type:** `object`<br/>|
| `apps.chartOperatorExtensions.clusterValues.configMap` |**None**|**Type:** `boolean`<br/>|
| `apps.chartOperatorExtensions.clusterValues.secret` |**None**|**Type:** `boolean`<br/>|
| `apps.chartOperatorExtensions.dependsOn` |**None**|**Type:** `string`<br/>|
| `apps.chartOperatorExtensions.extraConfigs` |**None**|**Type:** `array`<br/>|
| `apps.chartOperatorExtensions.extraConfigs[*]` |**None**||
| `apps.chartOperatorExtensions.extraConfigs[*].kind` |**None**|**Type:** `string`<br/>|
| `apps.chartOperatorExtensions.extraConfigs[*].name` |**None**|**Type:** `string`<br/>|
| `apps.chartOperatorExtensions.forceUpgrade` |**None**|**Type:** `boolean`<br/>|
| `apps.chartOperatorExtensions.inCluster` |**None**|**Type:** `boolean`<br/>|
| `apps.chartOperatorExtensions.namespace` |**None**|**Type:** `string`<br/>|
| `apps.chartOperatorExtensions.version` |**None**|**Type:** `string`<br/>|
| `apps.ciliumServiceMonitors` |**None**|**Type:** `object`<br/>|
| `apps.ciliumServiceMonitors.appName` |**None**|**Type:** `string`<br/>|
| `apps.ciliumServiceMonitors.catalog` |**None**|**Type:** `string`<br/>|
| `apps.ciliumServiceMonitors.chartName` |**None**|**Type:** `string`<br/>|
| `apps.ciliumServiceMonitors.clusterValues` |**None**|**Type:** `object`<br/>|
| `apps.ciliumServiceMonitors.clusterValues.configMap` |**None**|**Type:** `boolean`<br/>|
| `apps.ciliumServiceMonitors.clusterValues.secret` |**None**|**Type:** `boolean`<br/>|
| `apps.ciliumServiceMonitors.dependsOn` |**None**|**Type:** `string`<br/>|
| `apps.ciliumServiceMonitors.extraConfigs` |**None**|**Type:** `array`<br/>|
| `apps.ciliumServiceMonitors.extraConfigs[*]` |**None**||
| `apps.ciliumServiceMonitors.extraConfigs[*].kind` |**None**|**Type:** `string`<br/>|
| `apps.ciliumServiceMonitors.extraConfigs[*].name` |**None**|**Type:** `string`<br/>|
| `apps.ciliumServiceMonitors.forceUpgrade` |**None**|**Type:** `boolean`<br/>|
| `apps.ciliumServiceMonitors.inCluster` |**None**|**Type:** `boolean`<br/>|
| `apps.ciliumServiceMonitors.namespace` |**None**|**Type:** `string`<br/>|
| `apps.ciliumServiceMonitors.version` |**None**|**Type:** `string`<br/>|
| `apps.clusterResources` |**None**|**Type:** `object`<br/>|
| `apps.clusterResources.appName` |**None**|**Type:** `string`<br/>|
| `apps.clusterResources.catalog` |**None**|**Type:** `string`<br/>|
| `apps.clusterResources.chartName` |**None**|**Type:** `string`<br/>|
| `apps.clusterResources.clusterValues` |**None**|**Type:** `object`<br/>|
| `apps.clusterResources.clusterValues.configMap` |**None**|**Type:** `boolean`<br/>|
| `apps.clusterResources.clusterValues.secret` |**None**|**Type:** `boolean`<br/>|
| `apps.clusterResources.dependsOn` |**None**|**Type:** `string`<br/>|
| `apps.clusterResources.extraConfigs` |**None**|**Type:** `array`<br/>|
| `apps.clusterResources.extraConfigs[*]` |**None**||
| `apps.clusterResources.extraConfigs[*].kind` |**None**|**Type:** `string`<br/>|
| `apps.clusterResources.extraConfigs[*].name` |**None**|**Type:** `string`<br/>|
| `apps.clusterResources.forceUpgrade` |**None**|**Type:** `boolean`<br/>|
| `apps.clusterResources.inCluster` |**None**|**Type:** `boolean`<br/>|
| `apps.clusterResources.namespace` |**None**|**Type:** `string`<br/>|
| `apps.clusterResources.version` |**None**|**Type:** `string`<br/>|
| `apps.k8sDnsNodeCache` |**None**|**Type:** `object`<br/>|
| `apps.k8sDnsNodeCache.appName` |**None**|**Type:** `string`<br/>|
| `apps.k8sDnsNodeCache.catalog` |**None**|**Type:** `string`<br/>|
| `apps.k8sDnsNodeCache.chartName` |**None**|**Type:** `string`<br/>|
| `apps.k8sDnsNodeCache.clusterValues` |**None**|**Type:** `object`<br/>|
| `apps.k8sDnsNodeCache.clusterValues.configMap` |**None**|**Type:** `boolean`<br/>|
| `apps.k8sDnsNodeCache.clusterValues.secret` |**None**|**Type:** `boolean`<br/>|
| `apps.k8sDnsNodeCache.dependsOn` |**None**|**Type:** `string`<br/>|
| `apps.k8sDnsNodeCache.extraConfigs` |**None**|**Type:** `array`<br/>|
| `apps.k8sDnsNodeCache.extraConfigs[*]` |**None**||
| `apps.k8sDnsNodeCache.extraConfigs[*].kind` |**None**|**Type:** `string`<br/>|
| `apps.k8sDnsNodeCache.extraConfigs[*].name` |**None**|**Type:** `string`<br/>|
| `apps.k8sDnsNodeCache.forceUpgrade` |**None**|**Type:** `boolean`<br/>|
| `apps.k8sDnsNodeCache.inCluster` |**None**|**Type:** `boolean`<br/>|
| `apps.k8sDnsNodeCache.namespace` |**None**|**Type:** `string`<br/>|
| `apps.k8sDnsNodeCache.version` |**None**|**Type:** `string`<br/>|
| `apps.metricsServer` |**None**|**Type:** `object`<br/>|
| `apps.metricsServer.appName` |**None**|**Type:** `string`<br/>|
| `apps.metricsServer.catalog` |**None**|**Type:** `string`<br/>|
| `apps.metricsServer.chartName` |**None**|**Type:** `string`<br/>|
| `apps.metricsServer.clusterValues` |**None**|**Type:** `object`<br/>|
| `apps.metricsServer.clusterValues.configMap` |**None**|**Type:** `boolean`<br/>|
| `apps.metricsServer.clusterValues.secret` |**None**|**Type:** `boolean`<br/>|
| `apps.metricsServer.dependsOn` |**None**|**Type:** `string`<br/>|
| `apps.metricsServer.extraConfigs` |**None**|**Type:** `array`<br/>|
| `apps.metricsServer.extraConfigs[*]` |**None**||
| `apps.metricsServer.extraConfigs[*].kind` |**None**|**Type:** `string`<br/>|
| `apps.metricsServer.extraConfigs[*].name` |**None**|**Type:** `string`<br/>|
| `apps.metricsServer.forceUpgrade` |**None**|**Type:** `boolean`<br/>|
| `apps.metricsServer.inCluster` |**None**|**Type:** `boolean`<br/>|
| `apps.metricsServer.namespace` |**None**|**Type:** `string`<br/>|
| `apps.metricsServer.version` |**None**|**Type:** `string`<br/>|
| `apps.netExporter` |**None**|**Type:** `object`<br/>|
| `apps.netExporter.appName` |**None**|**Type:** `string`<br/>|
| `apps.netExporter.catalog` |**None**|**Type:** `string`<br/>|
| `apps.netExporter.chartName` |**None**|**Type:** `string`<br/>|
| `apps.netExporter.clusterValues` |**None**|**Type:** `object`<br/>|
| `apps.netExporter.clusterValues.configMap` |**None**|**Type:** `boolean`<br/>|
| `apps.netExporter.clusterValues.secret` |**None**|**Type:** `boolean`<br/>|
| `apps.netExporter.dependsOn` |**None**|**Type:** `string`<br/>|
| `apps.netExporter.extraConfigs` |**None**|**Type:** `array`<br/>|
| `apps.netExporter.extraConfigs[*]` |**None**||
| `apps.netExporter.extraConfigs[*].kind` |**None**|**Type:** `string`<br/>|
| `apps.netExporter.extraConfigs[*].name` |**None**|**Type:** `string`<br/>|
| `apps.netExporter.forceUpgrade` |**None**|**Type:** `boolean`<br/>|
| `apps.netExporter.inCluster` |**None**|**Type:** `boolean`<br/>|
| `apps.netExporter.namespace` |**None**|**Type:** `string`<br/>|
| `apps.netExporter.version` |**None**|**Type:** `string`<br/>|
| `apps.nodeExporter` |**None**|**Type:** `object`<br/>|
| `apps.nodeExporter.appName` |**None**|**Type:** `string`<br/>|
| `apps.nodeExporter.catalog` |**None**|**Type:** `string`<br/>|
| `apps.nodeExporter.chartName` |**None**|**Type:** `string`<br/>|
| `apps.nodeExporter.clusterValues` |**None**|**Type:** `object`<br/>|
| `apps.nodeExporter.clusterValues.configMap` |**None**|**Type:** `boolean`<br/>|
| `apps.nodeExporter.clusterValues.secret` |**None**|**Type:** `boolean`<br/>|
| `apps.nodeExporter.dependsOn` |**None**|**Type:** `string`<br/>|
| `apps.nodeExporter.extraConfigs` |**None**|**Type:** `array`<br/>|
| `apps.nodeExporter.extraConfigs[*]` |**None**||
| `apps.nodeExporter.extraConfigs[*].kind` |**None**|**Type:** `string`<br/>|
| `apps.nodeExporter.extraConfigs[*].name` |**None**|**Type:** `string`<br/>|
| `apps.nodeExporter.forceUpgrade` |**None**|**Type:** `boolean`<br/>|
| `apps.nodeExporter.inCluster` |**None**|**Type:** `boolean`<br/>|
| `apps.nodeExporter.namespace` |**None**|**Type:** `string`<br/>|
| `apps.nodeExporter.version` |**None**|**Type:** `string`<br/>|
| `apps.observabilityBundle` |**None**|**Type:** `object`<br/>|
| `apps.observabilityBundle.appName` |**None**|**Type:** `string`<br/>|
| `apps.observabilityBundle.catalog` |**None**|**Type:** `string`<br/>|
| `apps.observabilityBundle.chartName` |**None**|**Type:** `string`<br/>|
| `apps.observabilityBundle.clusterValues` |**None**|**Type:** `object`<br/>|
| `apps.observabilityBundle.clusterValues.configMap` |**None**|**Type:** `boolean`<br/>|
| `apps.observabilityBundle.clusterValues.secret` |**None**|**Type:** `boolean`<br/>|
| `apps.observabilityBundle.dependsOn` |**None**|**Type:** `string`<br/>|
| `apps.observabilityBundle.extraConfigs` |**None**|**Type:** `array`<br/>|
| `apps.observabilityBundle.extraConfigs[*]` |**None**||
| `apps.observabilityBundle.extraConfigs[*].kind` |**None**|**Type:** `string`<br/>|
| `apps.observabilityBundle.extraConfigs[*].name` |**None**|**Type:** `string`<br/>|
| `apps.observabilityBundle.forceUpgrade` |**None**|**Type:** `boolean`<br/>|
| `apps.observabilityBundle.inCluster` |**None**|**Type:** `boolean`<br/>|
| `apps.observabilityBundle.namespace` |**None**|**Type:** `string`<br/>|
| `apps.observabilityBundle.version` |**None**|**Type:** `string`<br/>|
| `apps.teleportKubeAgent` |**None**|**Type:** `object`<br/>|
| `apps.teleportKubeAgent.appName` |**None**|**Type:** `string`<br/>|
| `apps.teleportKubeAgent.catalog` |**None**|**Type:** `string`<br/>|
| `apps.teleportKubeAgent.chartName` |**None**|**Type:** `string`<br/>|
| `apps.teleportKubeAgent.clusterValues` |**None**|**Type:** `object`<br/>|
| `apps.teleportKubeAgent.clusterValues.configMap` |**None**|**Type:** `boolean`<br/>|
| `apps.teleportKubeAgent.clusterValues.secret` |**None**|**Type:** `boolean`<br/>|
| `apps.teleportKubeAgent.dependsOn` |**None**|**Type:** `string`<br/>|
| `apps.teleportKubeAgent.extraConfigs` |**None**|**Type:** `array`<br/>|
| `apps.teleportKubeAgent.extraConfigs[*]` |**None**||
| `apps.teleportKubeAgent.extraConfigs[*].kind` |**None**|**Type:** `string`<br/>|
| `apps.teleportKubeAgent.extraConfigs[*].name` |**None**|**Type:** `string`<br/>|
| `apps.teleportKubeAgent.forceUpgrade` |**None**|**Type:** `boolean`<br/>|
| `apps.teleportKubeAgent.inCluster` |**None**|**Type:** `boolean`<br/>|
| `apps.teleportKubeAgent.namespace` |**None**|**Type:** `string`<br/>|
| `apps.teleportKubeAgent.version` |**None**|**Type:** `string`<br/>|

### Delete options
Properties within the `.deleteOptions` top-level object

| **Property** | **Description** | **More Details** |
| :----------- | :-------------- | :--------------- |
| `deleteOptions.moveAppsHelmOwnershipToClusterCloudDirector` | **Move Apps Helm ownership to cluster-cloud-director** - Don't delete Apps' Helm charts in the workload cluster. After the update, cluster-cloud-director will recreate App CRs and new App CRs will take over the reconciliation of the existing Chart CRs in the workload cluster.|**Type:** `boolean`<br/>**Default:** `false`|

### Other

| **Property** | **Description** | **More Details** |
| :----------- | :-------------- | :--------------- |
| `clusterName` |**None**|**Type:** `string`<br/>|
| `managementCluster` |**None**|**Type:** `string`<br/>|
| `organization` |**None**|**Type:** `string`<br/>|



<!-- DOCS_END -->
