# rgw-bucket-helper

![Version: 0.1.3](https://img.shields.io/badge/Version-0.1.3-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 1.0](https://img.shields.io/badge/AppVersion-1.0-informational?style=flat-square)

A Helm chart for configuring buckets using OpenShift Container Storage RGW

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| bucket.name | string | `"my-bucket"` |  |
| bucket.namespacedName | bool | `true` |  |
| bucket.publicPolicy | bool | `false` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"quay.io/troyer/bucket-helper"` |  |
| image.tag | string | `""` |  |
| imagePullSecrets | list | `[]` |  |
| kafka.bootstrapServer | string | `""` |  |
| kafka.enabled | bool | `false` |  |
| nameOverride | string | `""` |  |
| s3.accessKeyID.valueFrom.secretKeyRef.key | string | `"AWS_ACCESS_KEY_ID"` |  |
| s3.accessKeyID.valueFrom.secretKeyRef.name | string | `"s3-secret"` |  |
| s3.host | string | `"http://rook-ceph-rgw-s3a.openshift-storage.svc.cluster.local"` |  |
| s3.secretAccessKey.valueFrom.secretKeyRef.key | string | `"AWS_SECRET_ACCESS_KEY"` |  |
| s3.secretAccessKey.valueFrom.secretKeyRef.name | string | `"s3-secret"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `false` |  |
| serviceAccount.name | string | `""` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.11.0](https://github.com/norwoodj/helm-docs/releases/v1.11.0)
