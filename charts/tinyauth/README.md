# tinyauth

![Version: 0.4.1](https://img.shields.io/badge/Version-0.4.1-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: v4.0.1](https://img.shields.io/badge/AppVersion-v4.0.1-informational?style=flat-square)

The simplest way to protect your apps with a login screen.

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| autoscaling.enabled | bool | `false` |  |
| autoscaling.maxReplicas | int | `10` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| autoscaling.targetMemoryUtilizationPercentage | int | `80` |  |
| env | list | `[]` |  |
| fullnameOverride | string | `""` |  |
| httpRoute.annotations | object | `{}` |  |
| httpRoute.enabled | bool | `false` |  |
| httpRoute.hostnames[0] | string | `"chart-example.local"` |  |
| httpRoute.parentRefs[0].name | string | `"my-gateway"` |  |
| httpRoute.rules[0].matches[0].path.type | string | `"Prefix"` |  |
| httpRoute.rules[0].matches[0].path.value | string | `"/"` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"ghcr.io/steveiliop56/tinyauth"` |  |
| image.tag | string | `""` |  |
| imagePullSecrets | list | `[]` |  |
| ingress.annotations | object | `{}` |  |
| ingress.className | string | `""` |  |
| ingress.enabled | bool | `false` |  |
| ingress.hosts[0].host | string | `"chart-example.local"` |  |
| ingress.hosts[0].paths[0].path | string | `"/"` |  |
| ingress.hosts[0].paths[0].pathType | string | `"ImplementationSpecific"` |  |
| ingress.tls | list | `[]` |  |
| livenessProbe.httpGet.path | string | `"/api/healthz"` |  |
| livenessProbe.httpGet.port | string | `"http"` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| persistence.accessMode | string | `"ReadWriteOnce"` |  |
| persistence.annotations | object | `{}` |  |
| persistence.enabled | bool | `false` |  |
| persistence.mountPath | string | `"/data"` |  |
| persistence.size | string | `"1Gi"` |  |
| persistence.storageClass | string | `""` |  |
| podAnnotations | object | `{}` |  |
| podLabels | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| readinessProbe.httpGet.path | string | `"/api/healthz"` |  |
| readinessProbe.httpGet.port | string | `"http"` |  |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| securityContext | object | `{}` |  |
| service.port | int | `80` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.automount | bool | `true` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `""` |  |
| tinyauth.general.address | string | `"0.0.0.0"` |  |
| tinyauth.general.appTitle | string | `""` |  |
| tinyauth.general.appUrl | string | `""` |  |
| tinyauth.general.backgroundImage | string | `""` |  |
| tinyauth.general.disableContinue | bool | `false` |  |
| tinyauth.general.forgotPasswordMessage | string | `""` |  |
| tinyauth.general.logLevel | string | `"info"` |  |
| tinyauth.general.loginMaxRetries | int | `5` |  |
| tinyauth.general.loginTimeout | int | `300` |  |
| tinyauth.general.oauthAutoRedirect | string | `""` |  |
| tinyauth.general.oauthWhitelist | string | `""` |  |
| tinyauth.general.port | int | `3000` |  |
| tinyauth.general.secureCookie | bool | `false` |  |
| tinyauth.general.sessionExpiry | int | `86400` |  |
| tinyauth.general.users | string | `""` |  |
| tinyauth.general.usersFile | string | `""` |  |
| tinyauth.ldap.address | string | `""` |  |
| tinyauth.ldap.baseDn | string | `""` |  |
| tinyauth.ldap.bindDn | string | `""` |  |
| tinyauth.ldap.bindPassword | string | `""` |  |
| tinyauth.ldap.bindPasswordSecretRef.key | string | `""` |  |
| tinyauth.ldap.bindPasswordSecretRef.name | string | `""` |  |
| tinyauth.ldap.enabled | bool | `false` |  |
| tinyauth.ldap.insecure | bool | `false` |  |
| tinyauth.ldap.searchFilter | string | `"(uid=%s)"` |  |
| tinyauth.providers[0].authUrl | string | `""` |  |
| tinyauth.providers[0].clientId | string | `""` |  |
| tinyauth.providers[0].clientSecret | string | `""` |  |
| tinyauth.providers[0].clientSecretFile | string | `""` |  |
| tinyauth.providers[0].clientSecretSecretRef.key | string | `""` |  |
| tinyauth.providers[0].clientSecretSecretRef.name | string | `""` |  |
| tinyauth.providers[0].id | string | `""` |  |
| tinyauth.providers[0].name | string | `""` |  |
| tinyauth.providers[0].scopes | string | `""` |  |
| tinyauth.providers[0].skipSsl | bool | `false` |  |
| tinyauth.providers[0].tokenUrl | string | `""` |  |
| tinyauth.providers[0].userInfoUrl | string | `""` |  |
| tolerations | list | `[]` |  |
| volumeMounts | list | `[]` |  |
| volumes | list | `[]` |  |

