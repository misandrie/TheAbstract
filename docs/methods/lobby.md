# Lobby

### /v1/realTimeMessaging/getUrl
`GET`
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Returns websocket url for party chat

### /v1/party/details
`GET`
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

| Param | Type | Required? |
| ----- | ---- | --------- |
| includeState | bool | yes |

> Returns party the user is in

### /v1/party
`POST`
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Creates a party

## Queue

### /v1/queue
`POST`
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Queues you for the game
> Can be called multiple times to update queue position
> Requires passing the EAC challenge check

### /v1/queue/cancel
`POST`
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Cancels queue