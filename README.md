octoprint
=========
OctoPrint is the snappy web interface for your 3D printer that allows you to control and monitor all aspects of your printer and print jobs, right from your browser.

Current chart version is `0.0.4`

Source code can be found [here](https://octoprint.org/)



## Chart Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| device | string | `"/dev/ttyACM0"` | Connection to printer  |
| video | string | `"/dev/video0"` | Connection to video (Not working at the moment) | 
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"octoprint/octoprint"` |  |
| image.tag | string | `"1.5.0"` | Container version for octoprint/octoprint |
| imagePullSecrets | list | `[]` |  |
| ingress.annotations | object | `{}` |  |
| ingress.enabled | bool | `false` |  |
| ingress.hosts[0].host | string | `"chart-example.local"` |  |
| ingress.hosts[0].paths | list | `[]` |  |
| ingress.tls | list | `[]` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| persistence.accessModes[0] | string | `"ReadWriteOnce"` |  |
| persistence.enabled | bool | `false` |  |
| persistence.existingClaim | string | `nil` |  |
| persistence.size | string | `"1Gi"` |  |
| persistence.storageClassName | string | `nil` |  |
| podSecurityContext | object | `{}` |  |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| securityContext.privileged | bool | `true` |  |
| server.env | list | `[]` | Environment variables for octoprint deployment |
| service.port | int | `5000` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `nil` |  |
| tolerations | list | `[]` |  |
