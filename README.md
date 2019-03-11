### emitter
---
https://github.com/emitter-io/emitter
https://github.com/olebedev/emitter

```js
var connection = emitter.connect({ host: '127.0.0.1' });

emitter.on('connect', function() {
  emitter.subscribe({
    key: "<channel key>",
    channel: "chat"
  });
});

emitter.publish({
  key: "<channel key>",
  channel: "chat/my_name",
  message: "hello, emitter!"
});


```

```
docker run -d --name emitter -p 8080:8080 --privileged --restart=unless-stopped emitter/server
go get -u github.com/emitter-io/emitter && emitter

go get -u github.com/emitter-io/emitter && emitter
go test ./...
docker run -d -p 8080:8080 emitter/server
docker run -d -p 8080:8080 -p 4000:4000 -e EMITTER_LICENSE=[key] -e EMITTER_CLUSTER_SEED=[seed] -e EMITTER_CLUSTER_PASSPHRASE=[name] emitter/server
```

```
{
  "listen": ":8080",
  "license": "/*The license*/",
  "tls": {
    "listen": "443".
    "host": "example.com"
  },
  "cluster": {
    "listen": ":4000",
    "seed": "192.168.0.2:4000",
    "advertise": "public:4000"
  },
  "storage": {
    "provider": "inmemory"
  }
}

```


