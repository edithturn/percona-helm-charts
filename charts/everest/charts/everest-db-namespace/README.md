# everest-db-namespace

![Version: 0.0.0](https://img.shields.io/badge/Version-0.0.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 0.0.0](https://img.shields.io/badge/AppVersion-0.0.0-informational?style=flat-square)

A sub-chart for provisioning Everest DB namespaces.

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| mayankshah1607 | <mayank.shah@percona.com> |  |
| oksana-grishchenko | <oksana.grishchenko@percona.com> |  |
| recharte | <diogo.recharte@percona.com> |  |
| michal-kralik | <michal.kralik@percona.com> |  |

## Requirements

Kubernetes: `>= 1.27.0`

| Repository | Name | Version |
|------------|------|---------|
| file://../common | common | 0.0.* |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| cleanupOnUninstall | bool | `true` | If set, cleans up the DB resources on uninstall. |
| compatibility.openshift | bool | `false` | If set, enable OpenShift compatibility. |
| namespaceOverride | string | `""` | Namespace override. Defaults to the value of .Release.Namespace. |
| olm.namespace | string | `"everest-olm"` | Namespace where OLM is installed in the cluster. |
| pg | bool | `true` | If set, installs the Percona Postgresql Server operator. |
| psmdb | bool | `true` | If set, installs the Percona Server MongoDB operator. |
| pxc | bool | `true` | If set, installs the Percona XtraDB Cluster operator. |
| telemetry | bool | `true` | If set, enabled sending telemetry information. |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.9.1](https://github.com/norwoodj/helm-docs/releases/v1.9.1)