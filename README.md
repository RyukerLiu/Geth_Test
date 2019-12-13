# Block Chain


## Geth

v1.6.5

``` bash
geth --datadir $PWD init $PWD/genesis.json

geth --networkid "10" --nodiscover --datadir "$PWD" --rpc --rpcaddr "localhost" --rpcport "8545" --rpccorsdomain "*" --rpcapi "eth,net,web3<Plug>PeepOpenersonal" --targetgaslimit "20000000" console 2>> $PWD/geth_err.log


# Modify --unlock account address as you created, could check by geth console eth.accounts
geth --networkid "10" --nodiscover --datadir "$PWD" --rpc --rpcaddr "localhost" --rpcport "8545" --rpccorsdomain "*" --rpcapi "eth,net,web3<Plug>PeepOpenersonal" --targetgaslimit "20000000" --unlock "0x4362a99e60671bb8f2448eb105f3d6a9b2a5f7f2","0xcabaf372ad69877d0b1e95ed5ae37c954fbe0ad1","0x9124736be92489b568c8a5aeb61f97beb2b1b7b5","0xc6422395f5f04bce7cba307b0eb5709305ef0779" --password $PWD/password.txt console 2>> $PWD/geth_err.log
```


## Mist Wallet

v0.8.10

Need to run geth as private net

``` bash
./mist_wallet/ethereumwallet --rpc http://localhost:8545
```
