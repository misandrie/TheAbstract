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

### /v1/party/player/{ID}/state
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Updates player state, accepts a json form