*These methods are for EAC challenges, which allow you to execute [queue methods](./queue.md)*

### /v1/extensions/eac/generateChallenge
`POST`
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

> Generates a challenge code from EAC

### /v1/extensions/eac/validateChallengeResponse
`POST`
| Cookie | Value |
| ------ | ----- |
| bhvrSession | session |

| json data | value |
| --------- | ----- |
| challengeResponse | challenge response |

> Validates response to EAC challenge  
> Updates bhvrSession to be able to queue