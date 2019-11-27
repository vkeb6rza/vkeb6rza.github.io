# Bitcoin services

All services are currently located at `[204:381:4c98:df09:d15b:ab1e:894b:d99e]` and are provided on a best-effort basis. It is strongly encouraged that if you are able, you also build your own bridges between the wider Bitcoin and Lightning network and Yggdrasil. More services will be added as time and resources permit, possibly on other IPs.

## Open Ports

### 8333 - Bitcoin
This is a full node which attempts to keep up with the BIP157 and BIP158 specifications. The number of connections, however, is limited, so please do try to connect full nodes. I can't guarantee the experimental BIP157 and BIP158 support will be up to date until PR 16442 is merged into master.

### 9735 - Lightning Network
This is a bridge via Tor to the rest of the Lightning Network. If you connect to the node, eventually I'll notice and open a channel to you and throw a few sats your way to help jump start the Yggdrasil Lightning economy.

Please connect to `038758ca700b8c4c73d1b86440acb963be93e5b11f9d6f363041be43572c8cbd43@[204:381:4c98:df09:d15b:ab1e:894b:d99e]:9735`

### 9911 - LND Watchtower
This is available to help monitor the Bitcoin blockchain and serve up justice if your own Lightning Network node is offline.

### 50001 - Electrum
This is a service allowing Electrum and other light clients to request transaction information via a different method than Bitcoin's P2P layer.
