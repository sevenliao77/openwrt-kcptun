# openwrt-kcptun

Binary in Release for download.

More details please refer to https://github.com/xtaci/kcptun

luci-app-kcptun please refer to https://github.com/kuoruan/luci-app-kcptun

Sample client config file for AR9341/MT7620 router with 64M memory. 
```
{
    "localaddr": ":6066",
    "remoteaddr": "vps:27700",
    "key": "it's a secrect",
    "crypt": "salsa20",
    "mode": "fast",
    "conn": 1,
    "autoexpire": 300,
    "mtu": 1350,
    "sndwnd": 1024,
    "rcvwnd": 1024,
    "datashard": 0,
    "parityshard": 0,
    "dscp": 46,
    "nocomp": true,
    "acknodelay": false,
    "nodelay": 0,
    "interval": 20,
    "resend": 2,
    "nc": 1,
    "sockbuf": 4194304,
    "keepalive": 10
}
```

Sample server config file for VPS.
```
{
    "listen": ":29900",
    "target": "127.0.0.1:12948",
    "key": "it's a secrect",
    "crypt": "salsa20",
    "mode": "fast",
    "conn": 1,
    "autoexpire": 300,
    "mtu": 1350,
    "sndwnd": 256,
    "rcvwnd": 256,
    "datashard": 0,
    "parityshard": 0,
    "dscp": 46,
    "nocomp": true,
    "acknodelay": false,
    "nodelay": 0,
    "interval": 20,
    "resend": 2,
    "nc": 1,
    "sockbuf": 4194304,
    "keepalive": 10
}

```
