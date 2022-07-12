Assuming you somehow have your JWL token saved you can instantly retrieve your bhvrSession cookie by passing the JWL Token to `https://brill.live.bhvrdbd.com/api/v1/auth/provider/egs/login` with the `token` parameter.

Example request:

```POST https://brill.live.bhvrdbd.com/api/v1/auth/provider/egs/login?token=foo.bar.rod HTTP/1.1
Host: brill.live.bhvrdbd.com
Accept: */*
Accept-Encoding: deflate, gzip
Content-Type: application/json
x-kraken-client-platform: egs
x-kraken-client-provider: egs
x-kraken-client-resolution: 1920x1080
x-kraken-client-timezone-offset: -180
x-kraken-client-os: 10.0.19044.1.256.64bit
x-kraken-client-version: 6.0.2
x-kraken-content-version: {"contentVersionId":"6.0.0_595699live"}
x-kraken-content-secret-key: mlySUt8ePI7qofwOUG3W/9BMcrvxq/w/AJCffC+uJaw=
User-Agent: DeadByDaylight/++DeadByDaylight+Live-CL-587396 EGS/10.0.19044.1.256.64bit
Content-Length: 17

{"clientData":{}}


If everything went OK you will get a 200 Response with a json object with your user info and the bhvrSession as a cookie value.