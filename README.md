## Another -1 Testnet



```http
  wget -q -O another-1-rekap.sh https://raw.githubusercontent.com/nadi555/Another-1/main/another-1-rekap.sh && chmod +x another-1-rekap.sh && sudo /bin/bash another-1-rekap.sh
```



#### after installation

```http
  source $HOME/.bash_profile
```


#### validator info

```http
anoned status 2>&1 | jq .ValidatorInfo

anoned status 2>&1 | jq .SyncInfo

anoned status 2>&1 | jq .NodeInfo
```
#### Create your wallet
Add New Wallet

```http
anoned keys add wallet
```
#### Recover Existing Wallet

```http
anoned keys add wallet --recover
```
#### List All Wallet

```http
anoned keys list
```

#### Check Wallet Balance

```http
anoned q bank balances $(anoned keys show wallet -a)
```
