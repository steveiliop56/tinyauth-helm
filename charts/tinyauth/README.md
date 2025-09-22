# tinyauth

![Version: 0.1.0](https://img.shields.io/badge/Version-0.1.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: v3.6.2](https://img.shields.io/badge/AppVersion-v3.6.2-informational?style=flat-square)

A Helm chart for Kubernetes

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
| livenessProbe.httpGet.path | string | `"/api/healthcheck"` |  |
| livenessProbe.httpGet.port | string | `"http"` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| podAnnotations | object | `{}` |  |
| podLabels | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| readinessProbe.httpGet.path | string | `"/api/healthcheck"` |  |
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
| tinyauth.general.cookieSecure | bool | `false` |  |
| tinyauth.general.disableContinue | bool | `false` |  |
| tinyauth.general.forgotPasswordMessage | string | `""` |  |
| tinyauth.general.logLevel | int | `1` |  |
| tinyauth.general.loginMaxRetries | int | `5` |  |
| tinyauth.general.loginTimeout | int | `300` |  |
| tinyauth.general.oauthAutoRedirect | string | `""` |  |
| tinyauth.general.oauthWhitelist | string | `""` |  |
| tinyauth.general.port | int | `3000` |  |
| tinyauth.general.secret | string | `""` |  |
| tinyauth.general.secretFile | string | `""` |  |
| tinyauth.general.secretSecretRef.key | string | `""` |  |
| tinyauth.general.secretSecretRef.name | string | `""` |  |
| tinyauth.general.sessionExpiry | int | `86400` |  |
| tinyauth.general.users | string | `""` |  |
| tinyauth.general.usersFile | string | `""` |  |
| tinyauth.generic.authUrl | string | `""` |  |
| tinyauth.generic.clientId | string | `""` |  |
| tinyauth.generic.clientSecret | string | `""` |  |
| tinyauth.generic.clientSecretFile | string | `""` |  |
| tinyauth.generic.clientSecretSecretRef.key | string | `""` |  |
| tinyauth.generic.clientSecretSecretRef.name | string | `""` |  |
| tinyauth.generic.name | string | `""` |  |
| tinyauth.generic.scopes | string | `""` |  |
| tinyauth.generic.skipSsl | bool | `false` |  |
| tinyauth.generic.tokenUrl | string | `""` |  |
| tinyauth.generic.userUrl | string | `""` |  |
| tinyauth.github.clientId | string | `""` |  |
| tinyauth.github.clientSecret | string | `""` |  |
| tinyauth.github.clientSecretFile | string | `""` |  |
| tinyauth.github.clientSecretSecretRef.key | string | `""` |  |
| tinyauth.github.clientSecretSecretRef.name | string | `""` |  |
| tinyauth.google.clientId | string | `""` |  |
| tinyauth.google.clientSecret | string | `""` |  |
| tinyauth.google.clientSecretFile | string | `""` |  |
| tinyauth.google.clientSecretSecretRef.key | string | `""` |  |
| tinyauth.google.clientSecretSecretRef.name | string | `""` |  |
| tinyauth.ldap.address | string | `""` |  |
| tinyauth.ldap.baseDn | string | `""` |  |
| tinyauth.ldap.bindDn | string | `""` |  |
| tinyauth.ldap.bindPassword | string | `""` |  |
| tinyauth.ldap.bindPasswordSecretRef.key | string | `""` |  |
| tinyauth.ldap.bindPasswordSecretRef.name | string | `""` |  |
| tinyauth.ldap.insecure | bool | `false` |  |
| tinyauth.ldap.searchFilter | string | `"(uid=%s)"` |  |
| tolerations | list | `[]` |  |
| volumeMounts | list | `[]` |  |
| volumes | list | `[]` |  |

