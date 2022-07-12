## Account
___
### /v1/auth/provider/egs/login
`POST`
> Returns whether or not the unified BHVR account is online

| Param | Type | Required? |
| ------ | ----- | ---- |
| token[^1] | string | yes |

| Header | Value |
| ------ | ----- |
| x-kraken-client-version | [krakenVersion](./initialization.md#v1version) |
| x-kraken-content-secret-key | key[^2] |
| x-kraken-content-version | [contentVersionId](./initialization.md#v1utilscontentversionversion) |

[^2]: Key is associated with the Dead By Daylight version and can be retrieved by logging in, I have not found it elsewhere currently

> Logs you in the game, returns a bhvrSession cookie

### /v1/auth/provider/egs/isUnifiedAccountOnline
`POST`
| Param | Type | Required? |
| ------ | ----- | ---- |
| token[^1] | string | yes |

[^1]: EOS token, provided by epic when you open the game

### /v1/consent
`GET`
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

| Param | Type | Required? |
| ----- | ---- | --------- |
| onlyAttentionNeeded | bool | yes |

> Returns what consent you have given (EULA/Privacy Policy/PSN/etc)

### /v1/auth/publicKey
`GET`
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Retrieves a public key

### /v1/config
`GET`
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Returns config json

### /v1/me/location
`GET`
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Returns your region (EU/NA), country and city where you connect from

### /v1/playername
`GET`
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Provides your player name, userid

### /v1/players/me/blockedPlayers
`GET`
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Retrieves a list of blocked players

### /v1/players/ban/status
`GET`
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |


> Retrieves whether or not the player is banned, boolean

### /v1/players/ban/decayAndGetDisconnectionPenaltyPoints
`POST`
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Retrieves penalty points


## Game
___
### /v1/dbd-core-ritual/get-and-generate-rituals
`POST`
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Returns ritual tasks

### /v1/extensions/wallet/getLocalizedCurrenciesAfterLogin
`POST`
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Returns player currency values on login

### /v1/wallet/currencies
`GET`
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Returns player currency values

### /v1/feature/status/archives
`GET`
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Retrieves archive status

### /v1/archives/stories/get/activeNode
`GET`
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Retrieves active archive node

### /v1/onboarding/get-bot-match-status
`GET`
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Retrieves whether or not bot matches were played

### /v1/ranks/reset-get-pips-v2
`POST`
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Retrieves player's pips, next rank reset date and seasonRefresh boolean