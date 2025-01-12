# Config Documentations

Redvin uses `toml` format for config file. you can customize your Redvin node network usage, connections, services, and ... in [`config.toml`](../../config/config.toml) file.

Here we are going through each part of this `config.toml` and explain them.

## network

First part of config file is `network`, you can determine the listening port and maximum connection of your Redvin node in this part.

Example:

```toml
[network]
port = 37771
max_connections = 10
```

## nostr

In this part you can determine the nostr relay configs such as maximum WebSocket connections, listening port and ...

Example:

```toml
[nostr]
port = 4444
max_ws_connections = 1000000
```

## rpc

RPC part help you to config the gRPC services.

Example:

```toml
[rpc]
enable_rpc = true
```

## metrics

Metrics helps you to config the metrics ans monitoring setting.

Example:

```toml
[metrics]
enable_metrics = false
```

## log

In the log part you can config the logging system, such as log levels, writing in file and ...

Example:

```toml
[log]
write_to_file = true
path = "log.r7"
```
