# HTTP/2 tunnel - A plugin for shadowsocks

## Intro

[h2tun](https://github.com/qiuyuzhou/h2tun) is a tunnel program over http/2 protocol,
which has been developed as a plugin for shadowsokcs. Its approach is similar to trojan,
but it is just a tcp tunnel over http/2, there is no proxy feature.

## Features

* Tunnel over http/2 with TLS
* Tunnel over http/2 cleartext

## Usage

The possible options can pass to env var `SS_PLUGIN_OPTIONS`.

Shared Options:

| Name | Description |
| --- | --- |
| path | Specify a handle path for tunnel. Default is /h2tunnel. You should always change it to a secret value. |

Client Mode Options:

| Name | Description |
| --- | --- |
| tls | Connect server by http/2 with TLS. Otherwise over http/2 cleartext |

Server Mode Options:

| Name | Description |
| --- | --- |
| server | Run in serve mode. Otherwise run in client mode.|
| keyFile | The tls cert key file path. |
| certFile | The tls cert file. |

## Deployment

TODO
