# Lobby

### /v1/realTimeMessaging/getUrl
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Returns websocket url for party chat

### /v1/party
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

| Param | Type | Required? |
| ----- | ---- | --------- |
| includeState | bool | no |

> Returns party the user is in

## Queue

### /v1/queue
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Queues you for the game
> Can be called multiple times to update queue position

### /v1/queue/cancel
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Cancels queue