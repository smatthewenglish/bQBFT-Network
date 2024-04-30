

## Node-2
```
besu --data-path=data --genesis-file=../genesis.json --bootnodes=enode://67d317ec360896fdc28224d53b57661c57d82ba75af7afa4b4f2d82771b312874caa250c9dbda4ad5337d7cd6bdb8016d85a879a304aff143261db6c348335f9@127.0.0.1:30303 --p2p-port=30304 --rpc-http-enabled --rpc-http-api=ETH,NET,QBFT --host-allowlist="*" --rpc-http-cors-origins="all" --rpc-http-port=8546
```


## Node-3
```
besu --data-path=data --genesis-file=../genesis.json --bootnodes=enode://67d317ec360896fdc28224d53b57661c57d82ba75af7afa4b4f2d82771b312874caa250c9dbda4ad5337d7cd6bdb8016d85a879a304aff143261db6c348335f9@127.0.0.1:30303 --p2p-port=30305 --rpc-http-enabled --rpc-http-api=ETH,NET,QBFT --host-allowlist="*" --rpc-http-cors-origins="all" --rpc-http-port=8547
```

## Node-4
```
besu --data-path=data --genesis-file=../genesis.json --bootnodes=enode://67d317ec360896fdc28224d53b57661c57d82ba75af7afa4b4f2d82771b312874caa250c9dbda4ad5337d7cd6bdb8016d85a879a304aff143261db6c348335f9@127.0.0.1:30303 --p2p-port=30306 --rpc-http-enabled --rpc-http-api=ETH,NET,QBFT --host-allowlist="*" --rpc-http-cors-origins="all" --rpc-http-port=8548
```

## confirm working
```
curl -X POST --data '{"jsonrpc":"2.0","method":"qbft_getValidatorsByBlockNumber","params":["latest"], "id":1}' localhost:8545
```
