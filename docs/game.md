### /v1/version
`GET`

> Returns json object with coreVersion and krakenVersion versions.

### /v1/healthcheck
`GET`
> Returns state of the game (health)

### /v1/utils/contentVersion/version
`GET`
| Param | Type | Required? |
| ------ | ----- | ---- |
| versionPattern | string | no |

> Returns available versions for specified game version, e.g. 6.1.0
> Can be left empty to return all available versions

### /v1/clientVersion/check
`POST`
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Returns if your client version is valid, bool