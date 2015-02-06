### If you devices (smart phone or computer) are not connected to Q Station(MB8800)'s network

- Port: 11608
- IP: 224.0.0.88

Format: "belled,\<router sn\>,\<router ip\>"

belled: recognize this signal is sent by MB8800 (Q Station)

router sn: sn number of Q Station

router IP: IP address of Q Station

### If your devices are connected to Q Station(MB8800), you can use ping command to find it.
```js
  {
      "cmd":"ping"
  }
  ```
  Response:
  ```js
  "belleds,<router sn>,<router ip>"
```
