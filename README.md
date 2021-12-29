# bsc-docker
https://docs.binance.org/smart-chain/developer/fullnode.html


## Running

```
mkdir data
docker run --rm -it -p 127.0.0.1:8545:8545 --name bsc -v $PWD/data:/root/.ethereum wshub/bsc --config /opt/config.toml --diffsync --rpc.allow-unprotected-txs --http --http.api debug,eth,web3,txpool --http.addr 0.0.0.0 --http.vhosts '*'
```


## Upgrade

Check latest release binary at <https://github.com/binance-chain/bsc/releases/latest>
