## Account
___
### /v1/auth/provider/egs/login

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

| Param | Type | Required? |
| ------ | ----- | ---- |
| token[^1] | string | yes |

[^1]: EOS token, provided by epic when you open the game

### /v1/consent
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

| Param | Type | Required? |
| ----- | ---- | --------- |
| onlyAttentionNeeded | bool | yes |

> Returns what consent you have given (EULA/Privacy Policy/PSN/etc)

### /v1/auth/publicKey
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Retrieves a public key

### /v1/config
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Returns config json

### /v1/me/location
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Returns your region (EU/NA), country and city where you connect from

### /v1/playername/
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Provides a player name, userid

### /v1/players/me/blockedPlayers
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Retrieves a list of blocked players

### /v1/players/ban/status
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |


> Retrieves whether or not the player is banned, boolean

### /v1/players/ban/decayAndGetDisconnectionPenaltyPoints
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Retrieves penalty points


## Game
___
### /v1/dbd-core-ritual/get-and-generate-rituals
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Returns ritual tasks

### /v1/extensions/wallet/getLocalizedCurrenciesAfterLogin
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Returns player currency values on login

### /v1/wallet/currencies
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Returns player currency values

### /v1/feature/status/archives
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Retrieves archive status

### /v1/archives/stories/get/activeNode
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Retrieves active archive node

### /v1/onboarding/get-bot-match-status
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Retrieves whether or not bot matches were played

### /v1/ranks/reset-get-pips-v2
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Retrieves player's pips, next rank reset date and seasonRefresh boolean